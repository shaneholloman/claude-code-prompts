# System Data Block: npm-view-custom-rules

- Source: inline

## Summary

Custom rules are replacing default settings.

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
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | CronDelete | None |

# Raw Prompt Text
${EXPR_1} failed to load

 (PID ${EXPR_2})

npm view ${EXPR_3: '@anthropic-ai/claude-code'}@${EXPR_4} version

global

${EXPR_5}

${EXPR_6}

## allow (custom rules replacing defaults)
Custom:
${EXPR_7}

Defaults being replaced:
${EXPR_8}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_9}

Defaults being replaced:
${EXPR_10}

## environment (custom rules replacing defaults)
Custom:
${EXPR_11}

Defaults being replaced:
${EXPR_12}



${EXPR_13}

what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_14} days, and that they can cancel sooner with ${EXPR_15: 'CronDelete'} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.
