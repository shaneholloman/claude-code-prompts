# System Data Block: custom-defaults-rules-replacing-13

- Source: inline

## Summary

Manage custom rules to override default settings.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | @anthropic-ai/claude-code | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |

# Raw Prompt Text
${EXPR_1}

${EXPR_2}

${EXPR_3} loaded with errors

${EXPR_4}

stable

npm view ${EXPR_5: '@anthropic-ai/claude-code'}@${EXPR_6} version

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

global

@anthropic-ai${PATH}

${EXPR_14}
