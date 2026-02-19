# System Data Block: hidden-github-put-request

- Source: inline

## Summary

Template for a hidden-parameter PUT request to update repository content.

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
| `EXPR_12` | sonnet | None |
| `EXPR_13` | false | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |

# Raw Prompt Text
${EXPR_1}

${EXPR_2}

${EXPR_3}

${EXPR_4}

${EXPR_5}

api

--method

PUT

repos/${EXPR_6}${PATH}${EXPR_7}

-f

message="Update ${EXPR_8}"

-f

content=${EXPR_9}

-f

branch=${EXPR_10}

user

project

local

--hidden

${EXPR_11}

${EXPR_12: 'sonnet'}

${EXPR_13: false}

${EXPR_14}

${EXPR_15}
