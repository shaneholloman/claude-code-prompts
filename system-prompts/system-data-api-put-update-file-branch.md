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

pattern: "${EXPR_2}"

${EXPR_3}

${EXPR_4}

${EXPR_5}

${EXPR_6}

${EXPR_7}

${EXPR_8}

Background Bash ${EXPR_9}

(command: ${EXPR_10})

(status: ${EXPR_11})

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

Background Bash ${EXPR_22}

(command: ${EXPR_23})

(status: ${EXPR_24})

${EXPR_25}

${EXPR_26}

${EXPR_27}

${EXPR_28}

${EXPR_29}

api

--method

PUT

repos/${EXPR_30}${PATH}${EXPR_31}

-f

message="Update ${EXPR_32}"

-f

content=${EXPR_33}

-f

branch=${EXPR_34}
