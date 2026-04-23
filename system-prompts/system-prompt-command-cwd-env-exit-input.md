# System Prompt: command-cwd-env-exit-input

- Source: native-reference-match

## Summary

System Prompt: command-cwd-env-exit-input - Source: inline Summary Handles command execution with environment settings.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
# System Prompt: command-cwd-env-exit-input

- Source: inline

## Summary

Handles command execution with environment settings.

# Raw Prompt Text
Input to command is JSON with old_cwd and new_cwd.
CLAUDE_ENV_FILE is set — write bash exports there to apply env to subsequent BashTool commands.
Hook output can include hookSpecificOutput.watchPaths (array of absolute paths) to register with the FileChanged watcher.
Exit code ${EXPR_1} - command completes successfully
Other exit codes - show stderr to user only
