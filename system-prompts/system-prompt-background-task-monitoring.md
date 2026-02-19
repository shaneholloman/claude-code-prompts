# System Prompt: background-task-monitoring

- Source: inline

## Summary

Announces task moved to background; provides monitoring link and teleport resume command.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
<background-task-output>This task is now running in the background.
Monitor it with ${PATH} or at ${EXPR_1}.

Or, resume it later with: claude --teleport ${EXPR_2}<${PATH}>
