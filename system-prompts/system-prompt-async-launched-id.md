# System Prompt: async-launched-id


## Summary

Reports successful async agent launch and returns internal agentId for later result retrieval.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Async agent launched successfully.
agentId: ${EXPR_1} (This is an internal ID for your use, do not mention it to the user. Use this ID when you want to retrieve results with AgentOutputTool)
