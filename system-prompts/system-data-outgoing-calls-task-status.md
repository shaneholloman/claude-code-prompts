# System Data Block: outgoing-calls-task-status

- Source: inline

## Summary

Displays outgoing calls with task status and a follow-on repo update request.

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

pattern: "${EXPR_1}"

${EXPR_2}

${EXPR_3}

${EXPR_4}

${EXPR_5}

${EXPR_6}

${EXPR_7}

${EXPR_8}

${EXPR_9}

${EXPR_10}

Found ${EXPR_11} outgoing calls:

Task #${EXPR_12}: ${EXPR_13}

Status: ${EXPR_14}

Description: ${EXPR_15}

api

--method

PUT

repos/${EXPR_16}${PATH}${EXPR_17}

-f

message="Update ${EXPR_18}"

-f

content=${EXPR_19}

-f

branch=${EXPR_20}

${EXPR_21}

${EXPR_22}:

start

mcp__${EXPR_23}__

${EXPR_24}

${EXPR_25}

${EXPR_26}

${EXPR_27}
