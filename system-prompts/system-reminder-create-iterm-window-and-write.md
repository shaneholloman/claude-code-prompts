# System Prompt: create-iterm-window-and-write

- Source: inline

## Summary

Creates a new iTerm window and writes text.

# Raw Prompt Text
tell application "iTerm"
  create window with default profile
  tell current session of current window
    write text "${EXPR_1}"
  end tell
end tell
