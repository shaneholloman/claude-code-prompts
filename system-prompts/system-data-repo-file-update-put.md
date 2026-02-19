# System Data Block: repo-file-update-put

- Source: inline

## Summary

PUT GitHub repo contents update request with commit message, base64 content, and branch.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
nullapi
--method
PUT
repos/${EXPR_1}${PATH}${EXPR_2}
-f
message="Update ${EXPR_3}"
-f
content=${EXPR_4}
-f
branch=${EXPR_5}
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
