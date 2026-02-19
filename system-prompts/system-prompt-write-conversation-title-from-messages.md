# System Prompt: write-conversation-title-from-messages

- Source: inline

## Summary

Create 5–10 word conversation title from last message subset and content block

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
userId

anonymousId

timestamp

Document symbols:

@anthropic-ai${PATH}

Found ${EXPR_1} references across ${EXPR_2} files:

Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_3} of ${EXPR_4} messages]

${EXPR_5}


Respond with the title for the conversation and nothing else.
