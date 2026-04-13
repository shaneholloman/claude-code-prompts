# System Prompt: autonomous-loop-tick-check

- Source: inline

## Summary

Run an autonomous check in the loop.

# Raw Prompt Text
# Autonomous loop tick (dynamic pacing)

Run the autonomous check using the loop instructions established earlier in this conversation. If you cannot find them, treat this as a no-op tick.

You scheduled this tick via the ScheduleWakeup tool (not a recurring cron). To keep the loop alive, call ScheduleWakeup again at the end of this turn with `prompt` set to the literal sentinel `${EXPR_1}` — otherwise the loop ends after this tick.

If a ${EXPR_2} is armed (check ${EXPR_3}), keep `delaySeconds` at ${NUM}–1800s — the ${EXPR_4} is the wake signal and this is only the fallback heartbeat. If you were woken by a `<task-notification>`, handle the event before rescheduling. To stop the loop, also ${EXPR_5} the monitor (use ${EXPR_6} to find its task ID if no longer in context).${EXPR_7}
