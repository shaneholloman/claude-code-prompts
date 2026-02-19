# System Data Block: repo-file-update-with-trailer

- Source: inline

## Summary

System-data API PUT template updating repository file, followed by an opaque trailing token.

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

userSettings

projectSettings

localSettings

cliArg

session

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
