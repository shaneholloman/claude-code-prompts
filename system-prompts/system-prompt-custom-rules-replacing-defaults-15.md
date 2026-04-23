# System Data Block: custom-rules-replacing-defaults-15

- Source: native-reference-match

## Summary

System Data Block: custom-rules-replacing-defaults-… - Source: native-reference-match Summary System Data Block: recurring-tasks-autonomous-defaults - Source…

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
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |

# Raw Prompt Text
# System Data Block: custom-rules-replacing-defaults-${NUM}

- Source: native-reference-match

## Summary

System Data Block: recurring-tasks-autonomous-defaults - Source: inline Summary Multiple prompts (…) Placeholder Hints (source-backed) | Expression | Hint |…

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
| `EXPR_9` | None | None |

# Raw Prompt Text
# System Data Block: recurring-tasks-autonomous-defaults

- Source: inline

## Summary

Multiple prompts (${EXPR_1})

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
${EXPR_2}## allow (custom rules replacing defaults)
Custom:
${EXPR_3}

Defaults being replaced:
${EXPR_4}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_5}

Defaults being replaced:
${EXPR_6}

## environment (custom rules replacing defaults)
Custom:
${EXPR_7}

Defaults being replaced:
${EXPR_8}

what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_9} days, and that they can cancel sooner with ${EXPR_10} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.
