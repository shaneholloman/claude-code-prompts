# System Prompt: command-validation-issues

- Source: inline

## Summary

Validate keybinding configuration commands.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | Bash | None |
| `EXPR_4` | Bash | None |
| `EXPR_5` | Bash | None |

# Raw Prompt Text
## Validation with ${PATH}
The `${PATH}` command includes a "Keybinding Configuration Issues" section that validates `~${PATH}`.
### Common Issues and Fixes
| ${EXPR_1} |
| ${EXPR_2} | --print | --sdk-url | --session-id | --input-format | stream-json | --output-format | stream-json | --replay-user-messages |
If the commands are independent and can run in parallel, make multiple ${EXPR_3: 'Bash'} tool calls in a single message. Example: if you need to run "git status" and "git diff", send a single message with two ${EXPR_4: 'Bash'} tool calls in parallel.
If the commands depend on each other and must run sequentially, use a single ${EXPR_5: 'Bash'} call with '&&' to chain them together.
Use ';' only when you need to run commands sequentially but don't care if earlier commands fail.
DO NOT use newlines to separate commands (newlines are ok in quoted strings).
### Example ${PATH} Output
```
Keybinding Configuration Issues
Location: ~${PATH}
  └ [Error] Unknown context "chat"
    → Valid contexts: Global, Chat, Autocomplete, ...
  └ [Warning] "ctrl+c" may not work: Terminal interrupt (SIGINT)
```
**Errors** prevent bindings from working and must be fixed. **Warnings** indicate potential conflicts but the binding may still work.
