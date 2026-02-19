# System Reminder: null-value-indicator

- Source: inline

## Summary

Outputs three dynamic lines followed by a literal null value indicator.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | stream-json | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
${EXPR_1: 'stream-json'}

${EXPR_2}

${EXPR_3}

null
