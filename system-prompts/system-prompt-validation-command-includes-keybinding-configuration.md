# System Prompt: a40a6c61

- Source: inline

## Summary

Validation with … The `…` command includes a "Keybinding Configuration Issues" section that validates `~…`.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | Read | None |
| `EXPR_2` | Glob | None |
| `EXPR_3` | Grep | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
## Validation with ${PATH}
The `${PATH}` command includes a "Keybinding Configuration Issues" section that validates `~${PATH}`.
### Common Issues and Fixes
| ${EXPR_1: 'Read'} | ${EXPR_2: 'Glob'} | ${EXPR_3: 'Grep'} |
| ${EXPR_4} | --print | --sdk-url | --session-id | --input-format | stream-json | --output-format | stream-json | --replay-user-messages |
${EXPR_5}
### Example ${PATH} Output
```
Keybinding Configuration Issues
Location: ~${PATH}
  └ [Error] Unknown context "chat"
    → Valid contexts: Global, Chat, Autocomplete, ...
  └ [Warning] "ctrl+c" may not work: Terminal interrupt (SIGINT)
```
**Errors** prevent bindings from working and must be fixed. **Warnings** indicate potential conflicts but the binding may still work.
