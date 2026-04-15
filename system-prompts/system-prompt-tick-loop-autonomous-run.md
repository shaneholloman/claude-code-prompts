# System Prompt: tick-loop-autonomous-run

- Source: inline

## Summary

Instructions for running an autonomous loop tick.

# Raw Prompt Text
# Autonomous loop tick

Run the autonomous check using the loop instructions established earlier in this conversation. If you cannot find them, treat this as a no-op tick. The recurring cron will fire the next tick automatically — do not call ScheduleWakeup from this tick.

Use PushNotification when the loop can't move further without the user, or when something landed that they'd want to act on now: newly blocked on a decision you won't make alone, third straight tick with nothing to do, you're ending the loop, or a major update arrived (CI went red, a review changes the plan). Progress you made yourself isn't a trigger — the transcript covers that. One ping per state, not per tick.
