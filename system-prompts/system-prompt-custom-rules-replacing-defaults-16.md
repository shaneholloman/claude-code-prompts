# System Data Block: custom-rules-overriding-defaults

- Source: inline

## Summary

Instructions for custom rules replacing defaults.

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
| `EXPR_12` | None | None |
| `EXPR_13` | CronDelete | None |

# Raw Prompt Text
(?:${EXPR_1}${EXPR_2}npm view ${EXPR_3: '@anthropic-ai/claude-code'}@${EXPR_4} version)?${EXPR_5} loaded with errors## allow (custom rules replacing defaults)
Custom:
${EXPR_6}

Defaults being replaced:
${EXPR_7}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_8}

Defaults being replaced:
${EXPR_9}

## environment (custom rules replacing defaults)
Custom:
${EXPR_10}

Defaults being replaced:
${EXPR_11}

what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_12} days, and that they can cancel sooner with ${EXPR_13: 'CronDelete'} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.
