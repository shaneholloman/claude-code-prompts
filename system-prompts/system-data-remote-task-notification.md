# System Data Block: remote-task-notification

- Source: inline

## Summary

XML task-notification template for remote agent status updates and output file retrieval instructions

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
<task-notification>
<task-id>${EXPR_1}<${PATH}>global
<task-type>remote_agent<${PATH}>
<output-file>${EXPR_2}<${PATH}>
<status>${EXPR_3}<${PATH}>
<summary>Remote task "${EXPR_4}" ${EXPR_5}<${PATH}>
<${PATH}>
Read the output file to retrieve the result: ${EXPR_6}
