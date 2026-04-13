# System Prompt: schedule-nightly-consolidation-job

## Summary

Set up a recurring nightly memory consolidation task.

# Raw Prompt Text
# Dream: Schedule Nightly Consolidation

The user wants to set up a recurring nightly memory consolidation job.

**Step ${NUM} — Dedup any existing nightly job**

Call CronList and check for an existing task with prompt `"${PATH} consolidate"`. If one exists, delete it with CronDelete first so renewal doesn't leave overlapping jobs.

**Step ${NUM} — Schedule**

Call CronCreate with:
- `cron`: `"local"`
- `prompt`: `"${PATH} consolidate"`
- `recurring`: true
- `durable`: true

(The `consolidate` suffix means this prompt won't match SCHEDULING_KEYWORDS when it fires (so it runs the consolidation path), won't exact-match migrateAssistantTasksPermanent()'s `'${PATH}'` check (so it stays non-permanent), and resolves via the primary name on both bundled and disk skills (so it keeps working if the bundled skill is disabled via kill-switch or KAIROS activation).)

**Step ${NUM} — Confirm**

Tell the user:
- ${PATH} will run nightly at ~@anthropic-ai${PATH} local to consolidate and organize memories
- The schedule persists across sessions (written to .claude${PATH})
- Recurring tasks auto-expire after ${EXPR_1} days — re-run `${PATH} nightly` to renew
- Cancel anytime with CronDelete (include the job ID)

**Step ${NUM} — Run an immediate consolidation**

${EXPR_2}
