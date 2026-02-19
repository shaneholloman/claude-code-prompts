# System Prompt: cwd-reset-type-validation-error

- Source: inline

## Summary

Report that the cwd reset value has an invalid type with expected types.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | false | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
${EXPR_1: false}
Shell cwd was reset to ${EXPR_2} is not an accepted type. Expected one of ${EXPR_3}.
