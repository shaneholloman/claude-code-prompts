# System Prompt: conversation-title-from-context-2

- Source: inline

## Summary

Compose a 3-5 word conversation title after reporting workspace reference and symbol counts

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
Found ${EXPR_1} references across ${EXPR_2} files:

--files

--follow

--hidden

Found ${EXPR_3} references across ${EXPR_4} files:

Found ${EXPR_5} symbols in workspace:

"

'

Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_6} of ${EXPR_7} messages]

${EXPR_8}


Respond with the title for the conversation and nothing else.
