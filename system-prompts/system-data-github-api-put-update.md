# System Data Block: github-api-put-update

- Source: inline

## Summary

Scripted GitHub API PUT call to update repository content with message, content, and branch fields.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | Write | None |
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
| `EXPR_14` | true | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |
| `EXPR_18` | false | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | None | None |
| `EXPR_22` | None | None |
| `EXPR_23` | None | None |
| `EXPR_24` | None | None |

# Raw Prompt Text
${EXPR_1}

${EXPR_2: 'Write'}

${EXPR_3}

${EXPR_4}

${EXPR_5}

${EXPR_6}

${EXPR_7} tool uses

${EXPR_8}h ${EXPR_9}m ${EXPR_10}s

${EXPR_11}

${EXPR_12}

${EXPR_13}

${EXPR_14: true}

${EXPR_15}

${EXPR_16}

${EXPR_17}

${EXPR_18: false}

${EXPR_19}

${EXPR_20}

${EXPR_21}

${EXPR_22}

api

--method

PUT

repos/${EXPR_23}${PATH}${EXPR_24}

-f

message=Update ${EXPR_25}

-f

content=${EXPR_26}

-f

branch=${EXPR_27}

${EXPR_28}

${EXPR_29}

${EXPR_30}

${EXPR_31}

${EXPR_32}

${EXPR_33}

${EXPR_34}

up

mid

down

${EXPR_35}

${EXPR_36}

${EXPR_37}
