# System Reminder: defer-hook-permission-decision-2

- Source: inline

## Summary

Handling deferred permission decisions in batch calls.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
Hook ${EXPR_1} returned permissionDecision=defer but ${EXPR_2} tool calls are in this batch; ignoring (defer is solo-only — siblings would be orphaned on resume)
