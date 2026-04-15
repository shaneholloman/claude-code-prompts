# System Reminder: scheduled-tasks-recurring-deletion

- Source: inline

## Summary

Deleting aged out recurring tasks after final fire.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | stream-json | None |
| `EXPR_3` | true | None |

# Raw Prompt Text
[ScheduledTasks] recurring task ${EXPR_1} aged out (${EXPR_2: 'stream-json'}_${EXPR_3: true}h since creation), deleting after final fire
