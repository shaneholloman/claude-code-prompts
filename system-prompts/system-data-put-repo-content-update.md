# System Data Block: put-repo-content-update

- Source: inline

## Summary

API PUT request template to update repository content with message, content, and branch.

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
| `EXPR_17` | false | None |
| `EXPR_18` | None | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |

# Raw Prompt Text
${EXPR_1}

${EXPR_2}

${EXPR_3}

${EXPR_4}

${EXPR_5}

${EXPR_6}

${EXPR_7}

api

--method

PUT

repos/${EXPR_8}${PATH}${EXPR_9}

-f

message="Update ${EXPR_10}"

-f

content=${EXPR_11}

-f

branch=${EXPR_12}

user

project

local

${EXPR_13}

${EXPR_14}

${EXPR_15}

${EXPR_16}

stream-json

${EXPR_17: false}

${EXPR_18}

${EXPR_19}

${EXPR_20}
