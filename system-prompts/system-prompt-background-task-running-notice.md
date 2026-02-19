# System Prompt: background-task-running-notice

- Source: inline

## Summary

Informs background task started, gives monitoring path/ID, and resume command format.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
<background-task-output>This task is now running in the background.
Monitor it with ${PATH} or at ${NUM}

Or, resume it later with: ${EXPR_1}${EXPR_2}<${PATH}>
