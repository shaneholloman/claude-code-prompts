# System Prompt: background-task-running-output

- Source: inline

## Summary

Background task notice with commands to monitor status or resume later via placeholder

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | false | None |

# Raw Prompt Text
<background-task-output>This task is now running in the background.
Monitor it with ${PATH} or at unknown

Or, resume it later with: ${EXPR_1: false}<${PATH}>
