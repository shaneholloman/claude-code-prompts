# System Prompt: conversation-title-with-pattern

- Source: inline

## Summary

Compose a NUM-NUM word conversation title from recent messages, matching EXPR_4 pattern.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | true | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |

# Raw Prompt Text
Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_1} of ${EXPR_2} messages]

${EXPR_3}
 Respond with the title for the conversation and nothing else. pattern: "${EXPR_4}" ${EXPR_5} ${EXPR_6} ${EXPR_7: true} ${EXPR_8} ${EXPR_9} ${EXPR_10} ${EXPR_11} ${EXPR_12} ${EXPR_13} ${EXPR_14}
