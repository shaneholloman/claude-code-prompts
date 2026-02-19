# System Prompt: tmux-terminal-shortcut-setup

- Source: inline

## Summary

Sets Shift+Enter multiline shortcut by running terminal command outside tmux, persisting settings.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
Terminal setup cannot be run from ${EXPR_1}.

This command configures a convenient Shift+Enter shortcut for multi-line prompts.
${EXPR_2}

To set up the shortcut (optional):
${NUM}. Exit tmux${PATH} temporarily
${NUM}. Run ${PATH} directly in one of these terminals:
${EXPR_3}   • IDE: VSCode, Cursor, Windsurf
   • Other: Ghostty, WezTerm
${NUM}. Return to tmux${PATH} - settings will persist
