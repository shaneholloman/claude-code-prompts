# System Reminder: lsp-contentmodified-retry-request

- Source: inline

## Summary

Logs ContentModified LSP request failure and schedules retry with backoff and attempt counters.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
LSP request '${EXPR_1}:${EXPR_2}' to '${EXPR_3}' got ContentModified error, retrying in  color="${EXPR_4}"ms (attempt ${EXPR_5}@${EXPR_6}${NUM}/${NUM})…
