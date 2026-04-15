# System Data Block: tell-application-current-window

- Source: inline

## Summary

Creates a new window in iTerm if it's running.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
tell application "iTerm"
  if running then
    create window with default profile
  else
    activate
  end if
  tell current session of current window
    write text "${EXPR_1}"
  end tell
end tell
