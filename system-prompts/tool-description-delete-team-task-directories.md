# Tool Description: delete-team-task-directories

- Source: native-reference-match

## Summary

Removes team and task directories and clears session context after teammates shut down.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# Tool Description: delete-team-task-directories

- Name: TeamDelete

## Summary

Removes team and task directories and clears session context after teammates shut down.

# Raw Prompt Text
# TeamDelete

Remove team and task directories when the swarm work is complete.

This operation:
- Removes the team directory (`~${EXPR_1}{team-name}/`)
- Removes the task directory (`~${EXPR_2}{team-name}/`)
- Clears team context from the current session

**IMPORTANT**: TeamDelete will fail if the team still has active members. Gracefully terminate teammates first, then call TeamDelete after all teammates have shut down.

Use this when all teammates have finished their work and you want to clean up the team resources. The team name is automatically determined from the current session's team context.
