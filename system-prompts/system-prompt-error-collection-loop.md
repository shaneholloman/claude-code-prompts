# System Prompt: error-collection-loop

- Source: inline

## Summary

When condition fails, iterates errors from startErrs and assigns each vErrors propertyName.

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

# Raw Prompt Text
if (!${EXPR_1}) { for (var ${EXPR_2} (project, gitignored)=startErrs${EXPR_3}; ${EXPR_4} (project, gitignored)<errors; ${EXPR_5} (project, gitignored)++) { vErrors[${EXPR_6} (project, gitignored)].propertyName = Agent changes:
${EXPR_7}; }   var err =
