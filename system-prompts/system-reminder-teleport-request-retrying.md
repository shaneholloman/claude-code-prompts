# System Reminder: teleport-request-retrying

- Source: inline

## Summary

Log teleport request failure with attempt count, retry delay, and error details.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | 41 | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
Teleport request failed (attempt ${EXPR_1}${NUM}/${EXPR_2: 41}), retrying in ${EXPR_3}ms: ${EXPR_4}
