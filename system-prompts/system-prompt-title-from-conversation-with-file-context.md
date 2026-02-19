# System Prompt: title-from-conversation-with-file-context

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

# Raw Prompt Text
--files --glob ${EXPR_1} --sort=modified --no-ignore --hidden Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_2} of ${EXPR_3} messages]

${EXPR_4}
 Respond with the title for the conversation and nothing else.
