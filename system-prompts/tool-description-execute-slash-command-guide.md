# Tool Description: execute-slash-command-guide

- Name: SlashCommand

## Summary

Execute validated slash command with arguments; on failure list up to … alternatives.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
Execute a slash command within the main conversation
Usage:
- `command` (required): The slash command to execute, including any arguments
- Example: `command: "${PATH} ${NUM}"`
Important Notes:
- Only available slash commands can be executed.
- Some commands may require arguments as shown in the command list above
- If command validation fails, list up to ${NUM} available commands, not all of them.
- Do not use this tool if you are already processing a slash command with the same name as indicated by <command-message>{name_of_command} is running…<${PATH}>
Available Commands:
${EXPR_1}${EXPR_2}
