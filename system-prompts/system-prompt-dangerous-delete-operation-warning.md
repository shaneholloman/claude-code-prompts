# System Prompt: dangerous-delete-operation-warning

- Source: inline

## Summary

Block auto-approval when … would delete a critical system directory, requiring explicit consent.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Dangerous \\.\pipe\claude-mcp-browser-bridge-default operation detected: '${EXPR_1}'

This command would remove a critical system directory. This requires explicit approval and cannot be auto-allowed by permission rules.
