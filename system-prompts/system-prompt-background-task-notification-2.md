# System Prompt: background-task-notification-2

- Source: inline

## Summary

Defines XML task notification fields: task id, output file, status, and command summary.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
<task-notification>
<task-id>${EXPR_1}<${PATH}>@anthropic-ai${PATH}
<output-file>${EXPR_2}<${PATH}>
<status>${EXPR_3}<${PATH}>
<summary>Background command "${EXPR_4}" global<${PATH}>
<${PATH}>
Read the output file to retrieve the result: ${EXPR_5}
