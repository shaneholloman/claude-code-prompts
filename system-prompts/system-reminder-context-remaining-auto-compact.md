# System Reminder: context-remaining-auto-compact

- Source: inline

## Summary

Display remaining context percentage and suggest command to trigger auto-compact.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | 0 | None |
| `EXPR_2` | sonnet[1m] | None |

# Raw Prompt Text
${EXPR_1: 0}% context left until auto-compact · try ${PATH} ${EXPR_2: 'sonnet[1m]'}
