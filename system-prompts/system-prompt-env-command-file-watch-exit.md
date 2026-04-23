# System Data Block: env-command-file-watch-exit

- Source: native-reference-match

## Summary

System Prompt: env-command-file-watch-exit - Source: native-reference-match Summary System Prompt: env-command-file-watch-exit - Source: inline Summary Handl…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
# System Prompt: env-command-file-watch-exit

- Source: native-reference-match

## Summary

System Prompt: env-command-file-watch-exit - Source: inline Summary Handles file events and environment exports.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
# System Prompt: env-command-file-watch-exit

- Source: inline

## Summary

Handles file events and environment exports.

# Raw Prompt Text
Input to command is JSON with file_path and event (change, add, unlink).
CLAUDE_ENV_FILE is set — write bash exports there to apply env to subsequent BashTool commands.
The matcher field specifies filenames to watch in the current directory (e.g. ".envrc|.env").
Hook output can include hookSpecificOutput.watchPaths (array of absolute paths) to dynamically update the watch list.
Exit code ${EXPR_1} - command completes successfully
Other exit codes - show stderr to user only
