# System Reminder: shell-exec-wrapper

- Source: inline

## Summary

Shebang-based wrapper execs a computed target path, forwarding all command-line arguments.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
#!${PATH}
exec "${EXPR_1}${PATH}" "$@"
