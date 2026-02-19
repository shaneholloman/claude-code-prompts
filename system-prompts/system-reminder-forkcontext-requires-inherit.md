# System Reminder: forkcontext-requires-inherit

- Source: inline

## Summary

Warn that forkContext requires model inherit and the model was overridden.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Agent file ${EXPR_1} has forkContext: true but model is not 'inherit'. Overriding to 'inherit'. Agents with forkContext must use model: inherit to avoid context length mismatch.
