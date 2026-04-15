# System Data Block: task-notification-interactive

- Source: inline

## Summary

Notification for blocked interactive tasks.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
<task-notification>
<task-id>${EXPR_1}<${PATH}> (PID ${EXPR_2})
<output-file>stable<${PATH}>
<summary>${EXPR_3}<${PATH}>
<${PATH}>
Last output:
${EXPR_4}

The command is likely blocked on an interactive prompt. Kill this task and re-run with piped input (e.g., `echo y | command`) or a non-interactive flag if one exists.
