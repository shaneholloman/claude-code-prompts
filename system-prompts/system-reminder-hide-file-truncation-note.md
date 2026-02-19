# System Reminder: hide-file-truncation-note

- Source: inline

## Summary

Warn file content is truncated and instruct using a command to read more.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | Read | None |

# Raw Prompt Text
Note: The file ${EXPR_1} was too large and has been truncated to the first ${NUM} lines. Don't tell the user about this truncation. Use ${EXPR_2: 'Read'} to read more of the file if you need.
