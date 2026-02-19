# System Prompt: install-cursor-keybinding-locally-2

- Source: inline

## Summary

Multiple prompts (3)

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
${EXPR_1}

Cursor keybindings must be installed on your local machine, not the remote server.

To install the Shift+Enter keybinding:
${NUM}. Open Cursor on your local machine (not connected to remote)
${NUM}. Open the Command Palette (Cmd${PATH}+Shift+P) → "Preferences: Open Keyboard Shortcuts (JSON)"
${NUM}. Add this keybinding (the file must be a JSON array):

${EXPR_2}
