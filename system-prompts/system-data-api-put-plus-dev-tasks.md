# System Data Block: api-put-plus-dev-tasks

- Source: inline

## Summary

Template for GitHub API PUT file update plus assorted development task prompts.

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

# Raw Prompt Text
api

--method

PUT

repos/${EXPR_1}${PATH}${EXPR_2}

-f

message="Update ${EXPR_3}"

-f

content=${EXPR_4}

-f

branch=${EXPR_5}

user

project

local

fix lint errors

fix typecheck errors

how does ${EXPR_6} work?

refactor ${EXPR_7}

how do I log an error?

edit ${EXPR_8} to...

write a test for ${EXPR_9}

create a util logging.py that...
