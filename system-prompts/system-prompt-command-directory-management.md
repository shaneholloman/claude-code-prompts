# System Prompt: commands-directory-paths

- Source: inline

## Summary

Guidelines for managing commands and directories.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
If your command will create new directories or files, first use this tool to run `ls` to verify the parent directory exists and is the correct location.

Always quote file paths that contain spaces with double quotes in your command (e.g., cd "path with spaces${PATH}")

Try to maintain your current working directory throughout the session by using absolute paths and avoiding usage of `cd`. You may use `cd` if the User explicitly requests it.

You may specify an optional timeout in milliseconds (up to ${EXPR_1}ms / ${EXPR_2} minutes). By default, your command will timeout after 120000ms (${EXPR_3} minutes).

Write a clear, concise description of what your command does. For simple commands, keep it brief (${NUM}-${NUM} words). For complex commands (piped commands, obscure flags, or anything hard to understand at a glance), include enough context so that the user can understand what your command will do.

When issuing multiple commands:

${EXPR_4}

For git commands:

${EXPR_5}

Avoid unnecessary `sleep` commands:

${EXPR_6}
