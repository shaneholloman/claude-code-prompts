# System Prompt: resume-metadata


## Summary

Provides agent resume metadata: agentId, token usage, tool uses, and duration.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
agentId: ${EXPR_1} (for resuming to continue this agent's work if needed)
<usage>total_tokens: ${EXPR_2}
tool_uses: ${EXPR_3}
duration_ms: ${EXPR_4}<${PATH}>
