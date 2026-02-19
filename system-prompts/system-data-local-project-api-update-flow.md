# System Data Block: local-project-api-update-flow

- Source: inline

## Summary

Local project context with API PUT request to update repository content and metadata

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
| `EXPR_13` | stream-json | None |
| `EXPR_14` | stream-json | None |

# Raw Prompt Text
fcoeoabgfenejglbffodgkkbkcdhcgfn

user

project

local

${EXPR_1}

fcoeoabgfenejglbffodgkkbkcdhcgfn

${EXPR_2}

api

--method

PUT

repos/${EXPR_3}${PATH}${EXPR_4}

-f

message="Update ${EXPR_5}"

-f

content=${EXPR_6}

-f

branch=${EXPR_7}

${EXPR_8}:

${EXPR_9}

mcp__${EXPR_10}__

${EXPR_11}

${EXPR_12}

${EXPR_13: 'stream-json'}

${EXPR_14: 'stream-json'}
