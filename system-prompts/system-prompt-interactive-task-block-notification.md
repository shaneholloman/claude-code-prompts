# System Prompt: interactive-task-block-notification

- Source: inline

## Summary

Notification for blocked interactive tasks.

# Raw Prompt Text
<task-notification>
<task-id>${EXPR_1}<${PATH}> (PID ${EXPR_2})
<output-file>stable<${PATH}>
<summary>${EXPR_3}<${PATH}>
<${PATH}>
Last output:
${EXPR_4}

The command is likely blocked on an interactive prompt. Kill this task and re-run with piped input (e.g., `echo y | command`) or a non-interactive flag if one exists.
