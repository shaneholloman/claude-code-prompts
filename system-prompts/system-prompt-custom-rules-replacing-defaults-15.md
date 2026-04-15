# System Data Block: custom-defaults-replacing-rules-5

- Source: inline

## Summary

Multiple prompts (3)

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | CronDelete | None |

# Raw Prompt Text
${EXPR_1}## allow (custom rules replacing defaults)
Custom:
${EXPR_2}

Defaults being replaced:
${EXPR_3}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_4}

Defaults being replaced:
${EXPR_5}

## environment (custom rules replacing defaults)
Custom:
${EXPR_6}

Defaults being replaced:
${EXPR_7}

what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_8} days, and that they can cancel sooner with ${EXPR_9: 'CronDelete'} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.
