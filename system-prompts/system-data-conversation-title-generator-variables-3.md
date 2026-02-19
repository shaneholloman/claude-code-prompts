# System Data Block: conversation-title-generator-variables-3

- Source: inline

## Summary

Compose a word title from the last messages using multiple inserted sections.

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

# Raw Prompt Text
${EXPR_1}

${EXPR_2}

${EXPR_3}

${EXPR_4}

${EXPR_5}

${EXPR_6}

${EXPR_7}

Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_8} of ${EXPR_9} messages]

${EXPR_10}


Respond with the title for the conversation and nothing else.
