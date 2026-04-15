# System Data Block: npm-view-version-replacing-defaults

- Source: inline

## Summary

Multiple prompts (2)

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | @anthropic-ai/claude-code | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |

# Raw Prompt Text
${EXPR_1}

npm view ${EXPR_2: '@anthropic-ai/claude-code'}@${EXPR_3} version

 (PID ${EXPR_4})

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



stable

${EXPR_11}

global

${EXPR_12}

@anthropic-ai${PATH}
