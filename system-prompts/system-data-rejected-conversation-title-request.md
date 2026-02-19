# System Data Block: rejected-conversation-title-request

- Source: inline

## Summary

Generate a 3–7 word conversation title, incorporating rejected prior context and recent messages

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
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |

# Raw Prompt Text
REJECTED

${EXPR_1}

${EXPR_2}

${EXPR_3}

${EXPR_4}

${EXPR_5}

${EXPR_6}

${EXPR_7}

${EXPR_8}

${EXPR_9}

${EXPR_10}

Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_11} of ${EXPR_12} messages]

${EXPR_13}


Respond with the title for the conversation and nothing else.
