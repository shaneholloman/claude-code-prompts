# System Prompt: loop-check-schedule-wakeup

- Source: inline

## Summary

Manage loop execution and wake scheduling.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | Monitor | None |
| `EXPR_3` | TaskList | None |
| `EXPR_4` | Monitor | None |
| `EXPR_5` | TaskStop | None |
| `EXPR_6` | TaskList | None |
| `EXPR_7` | None | None |

# Raw Prompt Text
# ${PATH} tick — loop.md absent (dynamic pacing)

loop.md is not currently present. Run the autonomous check using the loop instructions established earlier in this conversation.

You scheduled this tick via the ScheduleWakeup tool (not a recurring cron). To keep the loop alive — and to pick up loop.md if it is recreated — call ScheduleWakeup again at the end of this turn with `prompt` set to the literal sentinel `${EXPR_1}` — otherwise the loop ends after this tick.

If a ${EXPR_2: 'Monitor'} is armed (check ${EXPR_3: 'TaskList'}), keep `delaySeconds` at ${NUM}–1800s — the ${EXPR_4: 'Monitor'} is the wake signal and this is only the fallback heartbeat. If you were woken by a `<task-notification>`, handle the event before rescheduling. To stop the loop, also ${EXPR_5: 'TaskStop'} the monitor (use ${EXPR_6: 'TaskList'} to find its task ID if no longer in context).${EXPR_7}
