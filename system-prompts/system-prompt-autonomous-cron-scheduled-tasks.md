# System Prompt: autonomous-cron-scheduled-tasks

- Source: inline

## Summary

Details on autonomous scheduled tasks and cron expressions.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | CronDelete | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_1} days, and that they can cancel sooner with ${EXPR_2: 'CronDelete'} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.

${EXPR_3} failed to load
