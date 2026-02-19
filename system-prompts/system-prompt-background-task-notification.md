# System Prompt: background-task-notification

- Source: inline

## Summary

Reports background command status, summary message, and output file path for results.

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
<task-id>${PATH}<${PATH}>
<output-file>${EXPR_1}<${PATH}>
<status>${EXPR_2}<${PATH}>
<summary>Background command "${EXPR_3}" ${EXPR_4}<${PATH}>
<${PATH}>
Read the output file to retrieve the result: ${EXPR_5}
