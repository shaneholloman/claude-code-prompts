# System Reminder: hide-file-modified-note

- Source: inline

## Summary

Internal note that a file snippet was modified; provide numbered output silently.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Note: ${EXPR_1} was modified, either by the user or by a linter. Don't tell the user this, since they are already aware. So that you don't need to re-read the file, here's the result of running `cat -n` on a snippet of the edited file:
