# System Data Block: task-notification-output-file

- Source: inline

## Summary

Browser bridge task notification with pipe task-id, output path, status, and result file pointer.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
<task-notification>
<task-id>\\.\pipe\claude-mcp-browser-bridge-default<${PATH}>
<output-file>${EXPR_1}<${PATH}>
<status>${EXPR_2}<${PATH}>
<summary>[${EXPR_3}] [Claude Chrome Native Host] ${EXPR_4}${EXPR_5}
<${PATH}>
<${PATH}>
Read the output file to retrieve the result: ${EXPR_6}
