# System Reminder: plan-mode-read-only-workflow

- Source: inline

## Summary

Enforces plan mode: read-only outside plan file, follow phased workflow, end with questions or token.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | ExitPlanMode | None |

# Raw Prompt Text
Plan mode still active (see full instructions earlier in conversation). Read-only except plan file (${EXPR_1}). Follow ${NUM}-phase workflow. End turns with questions or ${EXPR_2: 'ExitPlanMode'}.
