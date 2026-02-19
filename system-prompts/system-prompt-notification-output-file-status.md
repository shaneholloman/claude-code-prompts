# System Prompt: notification-output-file-status

- Source: inline

## Summary

Agent notification XML emitting output file path, status code, and brief summary text.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
<agent-notification>
<agent-id>\\.\pipe\claude-mcp-browser-bridge-default<${PATH}>
<output-file>${EXPR_1}<${PATH}>
<status>${EXPR_2}<${PATH}>
<summary>${EXPR_3}<${PATH}>
Read the output file to retrieve the full result.
<${PATH}>
