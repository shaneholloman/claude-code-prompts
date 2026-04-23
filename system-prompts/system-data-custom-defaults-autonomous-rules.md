# System Data Block: custom-defaults-autonomous-rules

- Source: inline

## Summary

Instructions for custom rules replacing defaults.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | CronDelete | None |
| `EXPR_4` | @anthropic-ai/claude-code | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | CronDelete | None |

# Raw Prompt Text
${EXPR_1}what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_2} days, and that they can cancel sooner with ${EXPR_3: 'CronDelete'} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.npm view ${EXPR_4: '@anthropic-ai/claude-code'}@${EXPR_5} version## allow (custom rules replacing defaults)
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

${EXPR_12} loaded with errorswhat's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_13} days, and that they can cancel sooner with ${EXPR_14: 'CronDelete'} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.
