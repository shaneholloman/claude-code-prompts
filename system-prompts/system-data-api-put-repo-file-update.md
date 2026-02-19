# System Data Block: api-put-repo-file-update

- Source: inline

## Summary

Builds a PUT repo file update API call with message, content, branch, and metadata.

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
| `EXPR_10` | true | None |
| `EXPR_11` | true | None |
| `EXPR_12` | false | None |

# Raw Prompt Text
${EXPR_1}

${EXPR_2}

${EXPR_3}

--files

--follow

--hidden

api

--method

PUT

repos/${EXPR_4}${PATH}${EXPR_5}

-f

message="Update ${EXPR_6}"

-f

content=${EXPR_7}

-f

branch=${EXPR_8}

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

userId

anonymousId

timestamp

userSettings

projectSettings

localSettings

${EXPR_9}

stream-json

${EXPR_10: true}

${EXPR_11: true}

${EXPR_12: false}
