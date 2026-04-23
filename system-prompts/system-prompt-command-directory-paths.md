# System Prompt: command-directory-paths

- Source: inline

## Summary

Guidelines for handling commands and directories.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
If your command will create new directories or files, first use this tool to run `ls` to verify the parent directory exists and is the correct location.

Always quote file paths that contain spaces with double quotes in your command (e.g., cd "path with spaces${PATH}")

Try to maintain your current working directory throughout the session by using absolute paths and avoiding usage of `cd`. You may use `cd` if the User explicitly requests it.

You may specify an optional timeout in milliseconds (up to ${EXPR_1}ms / ${EXPR_2} minutes). By default, your command will timeout after 120000ms (${EXPR_3} minutes).

--deep-link-origin

For git commands:

${EXPR_4}

Avoid unnecessary `sleep` commands:

stable
