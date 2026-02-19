# System Data Block: remote-task-notification-format

- Source: inline

## Summary

Remote agent task notification including task ID, output path, status, and action summary

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | resolved list (4 items) | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | resolved list (4 items) | None |

# Raw Prompt Text
<task-notification>
<task-id>${EXPR_1}<${PATH}>
<task-type>remote_agent<${PATH}>
<output-file>${EXPR_2}<${PATH}>
<status>${EXPR_3}<${PATH}>
<summary>Remote task "${EXPR_4}" ${EXPR_5}<${PATH}>
<${PATH}>
Read the output file to retrieve the result: ${EXPR_6}
