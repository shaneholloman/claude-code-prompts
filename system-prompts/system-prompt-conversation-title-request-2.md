# System Prompt: conversation-title-request-2

- Source: inline

## Summary

Generate a 4–6 word conversation title using the last N messages context.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |

# Raw Prompt Text
${EXPR_1} ${EXPR_2} ${EXPR_3} ${EXPR_4} userSettings projectSettings localSettings Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_5} of ${EXPR_6} messages]

${EXPR_7}
 Respond with the title for the conversation and nothing else.
