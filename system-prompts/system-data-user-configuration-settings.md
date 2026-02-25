# System Data Block: user-configuration-anthropic

- Source: inline

## Summary

User's custom environment configuration.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
@anthropic-ai${PATH}

---

# User's Current Configuration

The user has the following custom setup in their environment:

${EXPR_1}

--print

--sdk-url

--session-id

--input-format

stream-json

--output-format

stream-json

--replay-user-messages

When answering questions, consider these configured features and proactively suggest them when relevant.
