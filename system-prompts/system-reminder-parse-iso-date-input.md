# System Reminder: parse-iso-date-input

- Source: inline

## Summary

Parse user date/time input into ISO format using provided current context.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
Current context:
- Current date and time: ${EXPR_1} (UTC)
- Local timezone: ${EXPR_2}
- Day of week:  (PID ${EXPR_3})

User input: "${EXPR_4}"

Output format: ${EXPR_5}

Parse the user's input into ISO ${NUM} format. Return ONLY the formatted string, or "INVALID" if the input is incomplete or unparseable.
