# Agent Prompt: mcp-servers-found-desktop

- Agent Type: null
- When to use: unknown
- Model: null
- Source: plugin
- Color: The user doesn't want to proceed with this tool use. The tool use was rejected (eg. if it was a file edit, the new_string was NOT written to the file). STOP what you are doing and wait for the user to tell you how to proceed.

Note: The user's next message may contain a correction or preference. Pay close attention — if they explain what went wrong or how they'd prefer you to work, consider saving that to memory for future sessions.

## Summary

Report count of MCP servers found in Claude Desktop, followed by details.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | 0 | None |

# Raw Prompt Text
Found ${EXPR_1: 0} MCP servers in Claude Desktop.

${NUM}
