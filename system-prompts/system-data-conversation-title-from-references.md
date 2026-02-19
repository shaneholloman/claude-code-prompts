# System Data Block: conversation-title-from-references

- Source: inline

## Summary

Generates a short conversation title alongside extracted file reference and API update context.

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

--files

--follow

--hidden

Found ${EXPR_6} references across ${EXPR_7} files:

Found ${EXPR_8} symbols in workspace:

${EXPR_9}

${EXPR_10}

${EXPR_11}

${EXPR_12}

${EXPR_13}

${EXPR_14}

<!DOCTYPE html>

<html>

<${PATH}>

${EXPR_15}

${EXPR_16}

${EXPR_17}

${EXPR_18}

${EXPR_19}

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
