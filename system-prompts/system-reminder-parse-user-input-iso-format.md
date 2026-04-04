# System Prompt: parse-user-input-iso-format

- Source: inline

## Summary

Parse user input into ISO format.

# Raw Prompt Text
Current context:
- Current date and time: ${EXPR_1} (UTC)
- Local timezone: global
- Day of week: ${EXPR_2}

User input: "${EXPR_3}"

Output format:  (PID ${EXPR_4})

Parse the user's input into ISO ${NUM} format. Return ONLY the formatted string, or "INVALID" if the input is incomplete or unparseable.
