# System Data Block: custom-defaults-rules-replacing-15

- Source: inline

## Summary

Defines custom rules that override default settings.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | @anthropic-ai/claude-code | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | CronDelete | None |

# Raw Prompt Text
(?:${EXPR_1}${EXPR_2}npm view ${EXPR_3: '@anthropic-ai/claude-code'}@${EXPR_4} version)?stable## allow (custom rules replacing defaults)
Custom:
${EXPR_5}

Defaults being replaced:
${EXPR_6}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_7}

Defaults being replaced:
${EXPR_8}

## environment (custom rules replacing defaults)
Custom:
${EXPR_9}

Defaults being replaced:
${EXPR_10}

what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_11} days, and that they can cancel sooner with ${EXPR_12: 'CronDelete'} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.
