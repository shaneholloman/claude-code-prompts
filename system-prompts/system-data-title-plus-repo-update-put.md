# System Data Block: title-plus-repo-update-put

- Source: inline

## Summary

Conversation title request plus workspace stats and a PUT request to update repository content.

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
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |
| `EXPR_18` | None | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | None | None |
| `EXPR_22` | None | None |
| `EXPR_23` | None | None |
| `EXPR_24` | None | None |

# Raw Prompt Text
Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_1} of ${EXPR_2} messages]

${EXPR_3}


Respond with the title for the conversation and nothing else.

Found ${EXPR_4} references across ${EXPR_5} files:

Found ${EXPR_6} symbols in workspace:

Found ${EXPR_7} references across ${EXPR_8} files:

Found ${EXPR_9} symbols in workspace:

${EXPR_10}

${EXPR_11}

${EXPR_12}

${EXPR_13}

${EXPR_14}

${EXPR_15}

${EXPR_16}

${EXPR_17}

${EXPR_18}

${EXPR_19}

${EXPR_20}

${EXPR_21}

api

--method

PUT

repos/${EXPR_22}${PATH}${EXPR_23}

-f

message="Update ${EXPR_24}"

-f

content=${EXPR_25}

-f

branch=${EXPR_26}
