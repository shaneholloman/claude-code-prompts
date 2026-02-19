# System Reminder: file-offset-shorter-warning

- Source: inline

## Summary

Warn that a file is shorter than the requested offset and report line count.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
<system-reminder>Warning: the file exists but is shorter than the provided offset (${EXPR_1}). The file has ${EXPR_2} lines.<${PATH}>
