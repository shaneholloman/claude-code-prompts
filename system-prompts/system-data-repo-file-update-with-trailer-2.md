# System Data Block: repo-file-update-with-trailer-2

- Source: inline

## Summary

System-data API PUT template updating repository file, followed by an opaque trailing token.

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

userSettings

projectSettings

localSettings

cliArg

session

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

userSettings

projectSettings

localSettings

cliArg

session

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
