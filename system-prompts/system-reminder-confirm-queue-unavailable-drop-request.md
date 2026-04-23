# System Reminder: confirm-queue-unavailable-drop-request

- Source: inline

## Summary

Drops a permission request when ToolUseConfirmQueue is unavailable for a source.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
[InboxPoller] ToolUseConfirmQueue unavailable, dropping permission request from ${EXPR_1}
