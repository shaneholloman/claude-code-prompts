# System Prompt: background-task-running-notice

- Source: inline

## Summary

Informs background task started, gives monitoring path/ID, and resume command format.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | unknown | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
<background-task-output>This task is now running in the background.
Monitor it with ${PATH} or at mcp__${EXPR_1: 'unknown'}__

Or, resume it later with: ${EXPR_2}<${PATH}>
