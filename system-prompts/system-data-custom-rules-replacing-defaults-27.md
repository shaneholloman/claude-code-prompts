# System Data Block: custom-defaults-replacing-rules-10

- Source: inline

## Summary

Custom rules for replacing defaults.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | @anthropic-ai/claude-code | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |

# Raw Prompt Text
npm view ${EXPR_1: '@anthropic-ai/claude-code'}@${EXPR_2} version${EXPR_3}## allow (custom rules replacing defaults)
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
