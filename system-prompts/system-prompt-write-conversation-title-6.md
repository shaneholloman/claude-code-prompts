# System Prompt: write-conversation-title-6

- Source: inline

## Summary

Create a word-limited title summarizing the provided conversation snippet from a file update.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
The file ${EXPR_1} has been updated. Here's the result of running `cat -n` on a snippet of the edited file:
Please write a ${NUM}-${NUM} word title the following conversation:

${EXPR_2}

Respond with the title for the conversation and nothing else.
