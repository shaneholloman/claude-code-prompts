# System Prompt: generate-conversation-title-2

- Source: inline

## Summary

Create a fixed-length title summarizing recent conversation messages, outputting only the title.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
start

user

project

local

${EXPR_1}

Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_2} of ${EXPR_3} messages]

${EXPR_4}


Respond with the title for the conversation and nothing else.
