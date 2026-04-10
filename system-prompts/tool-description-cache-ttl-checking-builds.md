# Tool Prompt: cache-ttl-checking-builds

- Name: ScheduleWakeup

## Summary

Guidelines for optimal cache usage during builds.

# Raw Prompt Text
${EXPR_1}

## Picking delaySeconds

The Anthropic prompt cache has a ${NUM}-minute TTL. Sleeping past ${NUM} seconds means the next wake-up reads your full conversation context uncached — slower and more expensive. So the natural breakpoints:

- **Under ${NUM} minutes (60s–270s)**: cache stays warm. Right for active work — checking a build, polling for state that's about to change, watching a process you just started.
- **${NUM} minutes to ${NUM} hour (300s–3600s)**: pay the cache miss. Right when there's no point checking sooner — waiting on something that takes minutes to change, or genuinely idle.

**Don't pick 300s.** It's the worst-of-both: you pay the cache miss without amortizing it. If you're tempted to "wait ${NUM} minutes," either drop to 270s (stay in cache) or commit to 1200s+ (one cache miss buys a much longer wait). Don't think in round-number minutes — think in cache windows.

For idle ticks with no specific signal to watch, default to **1200s–1800s** (${NUM}–${NUM} min). The loop checks back, you don't burn cache ${NUM}× per hour for nothing, and the user can always interrupt if they need you sooner.

Think about what you're actually waiting for, not just "how long should I sleep." If you kicked off an ${NUM}-minute build, sleeping 60s burns the cache ${NUM} times before it finishes — sleep ~270s twice instead.

The runtime clamps to [${NUM}, ${NUM}], so you don't need to clamp yourself.

## The reason field

One short sentence on what you chose and why. Goes to telemetry and is shown back to the user. "checking long bun build" beats "waiting." The user reads this to understand what you're doing without having to predict your cadence in advance — make it specific.
