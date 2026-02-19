# System Data Block: repeated-api-put-commands

- Source: inline

## Summary

Two sequential GitHub API PUT calls updating repo files with messages, content, and branch.

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
| `EXPR_8` | unknown | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |

# Raw Prompt Text
${EXPR_1}

start

api

--method

PUT

repos/${EXPR_2}${PATH}${EXPR_3}

-f

message="Update ${EXPR_4}"

-f

content=${EXPR_5}

-f

branch=${EXPR_6}

${EXPR_7}

start

${EXPR_8: 'unknown'}

api

--method

PUT

repos/${EXPR_9}${PATH}${EXPR_10}

-f

message="Update ${EXPR_11}"

-f

content=${EXPR_12}

-f

branch=${EXPR_13}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}
