# System Reminder: sessionid-null-workid-exited

- Source: inline

## Summary

Session exited with workId and status.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | tasklist | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
[bridge:session] sessionId=null workId=${EXPR_1} exited status=${EXPR_2: 'tasklist'} duration=${EXPR_3}s
