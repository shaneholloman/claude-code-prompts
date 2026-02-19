# System Reminder: task-with-prior-context

- Source: inline

## Summary

System reminder framing a task with optional local prior conversation context summary.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Task: ${EXPR_1}

  Prior conversation context (may or may not be relevant to the task above):
  local

  Note: The above summary represents what was being worked on before this background task was initiated. It may not be relevant to the current task.
