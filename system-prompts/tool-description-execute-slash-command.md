# Tool Description: execute-slash-command

- Name: SlashCommand

## Summary

Validate and run a specified slash command, listing limited available commands on failure.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Execute a slash command within the main conversation
Usage:
- `command` (required): The slash command to execute, including any arguments
- Example: `command: "${PATH} ${NUM}"`
Important Notes:
- Only available slash commands can be executed.
- Some commands may require arguments as shown in the command list above
- If command validation fails, list up to ${NUM} available commands, not all of them.
Available Commands:
${EXPR_1}
