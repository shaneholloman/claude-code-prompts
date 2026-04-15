# System Reminder: activate-terminal-script

- Source: inline

## Summary

Activates Terminal and runs a script.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
tell application "Terminal"
  do script ${EXPR_1}
  activate
end tell
