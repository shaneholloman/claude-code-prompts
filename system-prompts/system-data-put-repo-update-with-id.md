# System Data Block: put-repo-update-with-id

- Source: inline

## Summary

Constructs a PUT request to update repository content with message, content, and branch fields.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | unknown | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |

# Raw Prompt Text
${EXPR_1}

start

${EXPR_2: 'unknown'}

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

fcoeoabgfenejglbffodgkkbkcdhcgfn
