# System Prompt: async-output-polling


## Summary

Instructs how to poll or wait for an async agent using AgentOutputTool.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Async agent launched successfully.
agentId: ${EXPR_1} (This is an internal ID for your use, do not mention it to the user. Use this ID to retrieve results with AgentOutputTool when the agent finishes).
The agent is currently working in the background. If you have other tasks you you should continue working on them now. Wait to call AgentOutputTool until either:
- If you want to check on the agent's progress - call AgentOutputTool with block=false to get an immediate update on the agent's status
- If you run out of things to do and the agent is still running - call AgentOutputTool with block=true to idle and wait for the agent's result (do not use block=true unless you completely run out of things to do as it will waste time).
