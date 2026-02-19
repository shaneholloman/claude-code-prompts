# Tool Description: execute-slash-commands

- Name: SlashCommand

## Summary

Execute a listed custom slash command to route user intent into workflows.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Execute a slash command within the main conversation

**IMPORTANT - Intent Matching:**
Before starting any task, CHECK if the user's request matches one of the slash commands listed below. This tool exists to route user intentions to specialized workflows.

How slash commands work:
When you use this tool or when a user types a slash command, you will see <command-message>{name} is running…<${PATH}> followed by the expanded prompt. For example, if .claude${PATH} contains "Print today's date", then ${PATH} expands to that prompt in the next message.

Usage:
- `command` (required): The slash command to execute, including any arguments
- Example: `command: "${PATH} ${NUM}"`

IMPORTANT: Only use this tool for custom slash commands that appear in the Available Commands list below. Do NOT use for:
- Built-in CLI commands (like ${PATH}, ${PATH}, etc.)
- Commands not shown in the list
- Commands you think might exist but aren't listed

${EXPR_1}localNotes:
- When a user requests multiple slash commands, execute each one sequentially and check for <command-message>{name} is running…<${PATH}> to verify each has been processed
- Do not invoke a command that is already running. For example, if you see <command-message>foo is running…<${PATH}>, do NOT use this tool with "${PATH}" - process the expanded prompt in the following message
- Only custom slash commands with descriptions are listed in Available Commands. If a user's command is not listed, ask them to check the slash command file and consult the docs.
