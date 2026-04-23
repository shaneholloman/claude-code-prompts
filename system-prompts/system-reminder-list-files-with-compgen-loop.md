# System Reminder: list-files-with-compgen-loop

- Source: inline

## Summary

Shell command listing matching filesystem paths and appending slash for directories.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
compgen -f ${EXPR_1} ${NUM}>${PATH} | head -${NUM} | while IFS= read -r f; do [ -d "$f" ] && echo "$f/" || echo "$f "; done
