# System Reminder: bridge-session-exited-status

- Source: inline

## Summary

Session exited with status.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | tasklist | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
[bridge:session] sessionId=${EXPR_1} workId=${EXPR_2} exited status=${EXPR_3: 'tasklist'} duration=${EXPR_4}s
