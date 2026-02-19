# System Prompt: collect-validation-errors

- Source: inline

## Summary

Concat validation error arrays when submit-hook condition fails, updating vErrors and errors count.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
if (!<user-prompt-submit-hook>${EXPR_1}

[output truncated - exceeded ${NUM} characters]<${PATH}>) { if (vErrors === null) vErrors = ${EXPR_2}.errors; else vErrors = vErrors.concat(${EXPR_3}.errors); errors = vErrors.length; }
