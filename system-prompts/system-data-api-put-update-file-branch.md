# System Data Block: api-put-update-file-branch

- Source: inline

## Summary

Runs background bash then issues an API PUT to update repo content on a branch.

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
${EXPR_1}

${EXPR_2}

${EXPR_3}

${EXPR_4}

${EXPR_5}

${EXPR_6}

${EXPR_7}

pattern: "${EXPR_8}"

${EXPR_9}

${EXPR_10}

${EXPR_11}

${EXPR_12}

Background Bash ${EXPR_13}

(command: ${EXPR_14})

(status: ${EXPR_15})

${EXPR_16}

${EXPR_17}

${EXPR_18}

${EXPR_19}

${EXPR_20}

${EXPR_21}

${EXPR_22}

${EXPR_23}

${EXPR_24}

${EXPR_25}

Background Bash ${EXPR_26}

(command: ${EXPR_27})

(status: ${EXPR_28})

${EXPR_29}

${EXPR_30}

${EXPR_31}

api

--method

PUT

repos/${EXPR_32}${PATH}${EXPR_33}

-f

message="Update ${EXPR_34}"

-f

content=${EXPR_35}

-f

branch=${EXPR_36}
