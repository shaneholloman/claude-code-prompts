# System Data Block: and-custom-rules

- Source: inline

## Summary

Explains custom rules that override defaults.

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

# Raw Prompt Text
Tool: ${EXPR_1}
Description: ${EXPR_2}

Input:
npm view ${EXPR_3: '@anthropic-ai/claude-code'}@${EXPR_4} version

Recent conversation context:
## allow (custom rules replacing defaults)
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



Explain this command in context.
