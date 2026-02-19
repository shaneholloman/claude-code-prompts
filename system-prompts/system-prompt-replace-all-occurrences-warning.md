# System Prompt: replace-all-occurrences-warning

- Source: inline

## Summary

Warns about multiple replacement matches when replace_all is false, requesting unique context.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Found local matches of the string to replace, but replace_all is false. To replace all occurrences, set replace_all to true. To replace only one occurrence, please provide more context to uniquely identify the instance.
String: ${EXPR_1}
