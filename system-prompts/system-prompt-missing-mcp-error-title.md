# System Prompt: missing-mcp-error-title

- Source: inline

## Summary

Report missing MCP tool and request a short title for the given conversation.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
Error: MCP tool ${EXPR_1} (passed via --permission-prompt-tool) not found. Available MCP tools: Please write a ${NUM}-${NUM} word title the following conversation:

${EXPR_2}
, Respond with the title for the conversation and nothing else.
