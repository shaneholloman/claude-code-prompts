# System Data Block: recurring-tasks-autonomous-defaults

- Source: inline

## Summary

Multiple prompts (2)

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | CronDelete | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | CronDelete | None |

# Raw Prompt Text
${EXPR_1}what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_2} days, and that they can cancel sooner with ${EXPR_3: 'CronDelete'} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.stable## allow (custom rules replacing defaults)
Custom:
${EXPR_4}

Defaults being replaced:
${EXPR_5}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_6}

Defaults being replaced:
${EXPR_7}

## environment (custom rules replacing defaults)
Custom:
${EXPR_8}

Defaults being replaced:
${EXPR_9}

what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_10} days, and that they can cancel sooner with ${EXPR_11: 'CronDelete'} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.
