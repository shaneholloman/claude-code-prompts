# System Reminder: auto-mode-gate-exit-plan-2

- Source: inline

## Summary

Fallback to default on plan exit when gate is off.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
[auto-mode gate @ ExitPlanModeV2Tool] prePlanMode=${EXPR_1} but gate is off (reason=@anthropic-ai${PATH}) — falling back to default on plan exit
