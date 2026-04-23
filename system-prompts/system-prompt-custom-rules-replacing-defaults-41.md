# System Data Block: dangerous-operation-detected

- Source: inline

## Summary

Detects dangerous operations with custom rules.

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

# Raw Prompt Text
Dangerous ${EXPR_1} operation detected: '## allow (custom rules replacing defaults)
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

'

This command would remove a critical system directory. This requires explicit approval and cannot be auto-allowed by permission rules.
