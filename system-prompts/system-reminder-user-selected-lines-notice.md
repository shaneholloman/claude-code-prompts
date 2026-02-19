# System Reminder: user-selected-lines-notice

- Source: inline

## Summary

Warn that user-selected lines from a source file may be unrelated to current task

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
<system-reminder>
The user selected the following lines from ${EXPR_1}:
${EXPR_2}. This may or may not be related to the current task.
<${PATH}>
