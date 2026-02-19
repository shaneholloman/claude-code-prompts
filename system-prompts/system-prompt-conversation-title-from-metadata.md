# System Prompt: conversation-title-from-metadata

- Source: inline

## Summary

Create a 3–6 word conversation title from recent messages and workspace settings metadata

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
${EXPR_1} ${EXPR_2} userId anonymousId timestamp Found ${EXPR_3} symbols in workspace: userId anonymousId timestamp userSettings projectSettings localSettings Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_4} of ${EXPR_5} messages]

${EXPR_6}
 Respond with the title for the conversation and nothing else.
