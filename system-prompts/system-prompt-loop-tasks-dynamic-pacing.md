# System Prompt: loop-tasks-dynamic-pacing

- Source: inline

## Summary

Execute tasks with dynamic pacing for the user.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
# ${PATH} — loop.md tasks with dynamic pacing

The user invoked `${PATH}` with no prompt and no interval and has a loop-tasks file at `${EXPR_1}`. Run those tasks now, then self-pace the next iteration via ScheduleWakeup — no cron.
