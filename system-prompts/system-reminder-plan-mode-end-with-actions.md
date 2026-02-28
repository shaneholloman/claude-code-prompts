# System Reminder: plan-mode-end-with-actions

- Source: inline

## Summary

Requires ending each turn with a question or plan-approval action in plan mode.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | ExitPlanMode | None |

# Raw Prompt Text
Plan mode still active (see full instructions earlier in conversation). Read-only except plan file (${EXPR_1}). ${EXPR_2} End turns with AskUserQuestion (for clarifications) or ${EXPR_3: 'ExitPlanMode'} (for plan approval). Never ask about plan approval via text or AskUserQuestion.
