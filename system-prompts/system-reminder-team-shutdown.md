# System Reminder: team-shutdown

- Source: native-reference-match

## Summary

System Reminder: shutdown-team-before-response - Source: inline Summary Requires shutting down the team before delivering the final user response.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# System Reminder: team-shutdown

- Source: native-reference-match

## Summary

Requires shutting down the team before delivering the final user response.

# Raw Prompt Text
<system-reminder>
You are running in non-interactive mode and cannot return a response to the user until your team is shut down.

You MUST shut down your team before preparing your final response:
${EXPR_1}. Use requestShutdown to ask each team member to shut down gracefully
${EXPR_2}. Wait for shutdown approvals
${EXPR_3}. Use the cleanup operation to clean up the team
${EXPR_4}. Only then provide your final response to the user

The user cannot receive your response until the team is completely shut down.
<${EXPR_5}>

Shut down your team and prepare your final response for the user.
