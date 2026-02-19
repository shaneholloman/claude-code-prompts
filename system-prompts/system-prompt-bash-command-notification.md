# System Prompt: bash-command-notification

- Source: inline

## Summary

Notifies background shell task completion status and provides output file for results.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
<bash-notification>
<shell-id>\\.\pipe\claude-mcp-browser-bridge-default<${PATH}>
<output-file>${EXPR_1}<${PATH}>
<status>${EXPR_2}<${PATH}>
<summary>Background command "${EXPR_3}" ${EXPR_4}.<${PATH}>
Read the output file to retrieve the output.
<${PATH}>
