# System Prompt: remote-task-output-retrieval

- Source: inline

## Summary

Announce remote_agent task completion and instruct retrieving output via TaskOutputTool task_id.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
<task-notification>
<task-id>\\.\pipe\claude-mcp-browser-bridge-default<${PATH}>
<task-type>remote_agent<${PATH}>
<status>${EXPR_1}<${PATH}>
<summary>Remote task "${EXPR_2}" completed successfully.<${PATH}>
Use TaskOutputTool with task_id="\\.\pipe\claude-mcp-browser-bridge-default" to retrieve the output.
<${PATH}>
