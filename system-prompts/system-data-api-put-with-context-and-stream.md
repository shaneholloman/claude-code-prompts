# System Data Block: api-put-with-context-and-stream

- Source: inline

## Summary

API PUT update sequence with user/project/local context and stream-json fields.

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

# Raw Prompt Text
Background Bash ${EXPR_1}

(command: ${EXPR_2})

(status: ${EXPR_3})

${EXPR_4}

${EXPR_5}

${EXPR_6}

api

--method

PUT

repos/${EXPR_7}${PATH}${EXPR_8}

-f

message="Update ${EXPR_9}"

-f

content=${EXPR_10}

-f

branch=${EXPR_11}

user

project

local

${EXPR_12}

${EXPR_13}

${EXPR_14}

${EXPR_15}

stream-json

${EXPR_16}

${EXPR_17}

${EXPR_18}

${EXPR_19}
