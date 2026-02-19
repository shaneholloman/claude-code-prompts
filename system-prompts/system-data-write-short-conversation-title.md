# System Data Block: write-short-conversation-title

- Source: inline

## Summary

Asks for a fixed-length title summarizing the recent conversation.

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

┼

┤

╶

╴

─

╰

╭

╮

╯

│

pattern: "${EXPR_4}"

${EXPR_5}

${EXPR_6}

${EXPR_7}

${EXPR_8}

${EXPR_9}

${EXPR_10}

${EXPR_11}

${EXPR_12}

${EXPR_13}

Found ${EXPR_14} outgoing calls:

Task #${EXPR_15}: ${EXPR_16}

Status: ${EXPR_17}

Description: ${EXPR_18}

user

project

local

${EXPR_19}:

api

--method

PUT

repos/${EXPR_20}${PATH}${EXPR_21}

-f

message="Update ${EXPR_22}"

-f

content=${EXPR_23}

-f

branch=${EXPR_24}

${EXPR_25}

${EXPR_26}:
