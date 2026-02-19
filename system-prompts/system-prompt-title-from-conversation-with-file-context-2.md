# System Prompt: title-from-conversation-with-file-context-2

- Source: inline

## Summary

Generate a 3–4 word conversation title from recent messages, with file-glob context

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
| `EXPR_8` | None | None |

# Raw Prompt Text
--files --glob ${EXPR_1} --sort=modified --no-ignore --hidden ${EXPR_2} ${EXPR_3} ${EXPR_4} ${EXPR_5} Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_6} of ${EXPR_7} messages]

${EXPR_8}
 Respond with the title for the conversation and nothing else.
