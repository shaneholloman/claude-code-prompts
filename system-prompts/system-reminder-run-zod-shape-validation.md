# System Reminder: run-zod-shape-validation

- Source: inline

## Summary

Run a Zod shape validator on an input value and collect issues.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
shape[${EXPR_1}@${EXPR_2}]._zod.run({ value: input[${EXPR_3}@${EXPR_4}], issues: [] }, ctx)
