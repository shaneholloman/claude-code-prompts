# Tool Prompt: monitor-script-events-stream

## Summary

Streams events from a long-running script's stdout.

# Raw Prompt Text
Start a background monitor that streams events from a long-running script. Each stdout line is an event — you keep working and notifications arrive in the chat. Events arrive on their own schedule and are not replies from the user, even if one lands while you're waiting for the user to answer a question.

Monitor is for the **streaming** case: "tell me every time X happens." For one-shot "wait until X is done," use Bash with run_in_background instead — you'll get a completion notification when it exits.

Your script's stdout is the event stream. Each line becomes a notification. Exit ends the watch.

  # Each matching log line is an event
  tail -f ${PATH} | grep --line-buffered "ERROR"

  # Each file change is an event
  inotifywait -m --format '%e %f' ${PATH}

  # Poll GitHub for new PR comments and emit one line per new comment
  last=$(date -u +%Y-%m-%dT%H:%M:%SZ)
  while true; do
    now=$(date -u +%Y-%m-%dT%H:%M:%SZ)
    gh api "repos${PATH}?since=$last" --jq '.[] | "\(.user.login): \(.body)"'
    last=$now; sleep ${NUM}
  done

  # Node script that emits events as they arrive (e.g. WebSocket listener)
  node watch-for-events.js

**Script quality:**
- Always use `grep --line-buffered` in pipes — without it, pipe buffering delays events by minutes.
- In poll loops, handle transient failures (`curl ... || true`) — one failed request shouldn't kill the monitor.
- Poll intervals: 30s+ for remote APIs (rate limits), ${NUM}-1s for local checks.
- Write a specific `description` — it appears in every notification ("errors in deploy.log" not "watching logs").
- Only stdout is the event stream. Stderr goes to the output file (readable via Read) but does not trigger notifications.

**Output volume**: Every stdout line becomes a message in the conversation, so write selective filters. Never pipe raw logs — use `grep --line-buffered`, `awk`, or a wrapper that only emits the events you care about. Redirect progress you don't need to `>${PATH}`. Monitors that produce too many events are automatically stopped; restart with a tighter filter if this happens.

Stdout lines within 200ms are batched into a single notification, so multiline output from a single event groups naturally.

The script runs in the same shell environment as Bash. Exit ends the watch (exit code is reported). Timeout → killed. Set `persistent: true` for session-length watches (PR monitoring, log tails) — the monitor runs until you call TaskStop or the session ends. Use TaskStop to cancel early.
