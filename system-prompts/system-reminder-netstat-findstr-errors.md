# System Reminder: netstat-findstr-errors

- Source: inline

## Summary

Check netstat for loaded errors.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
netstat -ano | findstr :${EXPR_1} loaded with errors
