# System Prompt: keybinding-config-validation-guide

- Source: inline

## Summary

Validate keybinding config file, list common errors and warnings with fixes.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
## Validation with ${PATH}
The `${PATH}` command includes a "Keybinding Configuration Issues" section that validates `~${PATH}`.
### Common Issues and Fixes
| ${URL} | ${URL} |
| ${EXPR_1} | ${EXPR_2} | ${EXPR_3} | ${EXPR_4} | ${EXPR_5} |
${EXPR_6}
### Example ${PATH} Output
```
Keybinding Configuration Issues
Location: ~${PATH}
  └ [Error] Unknown context "chat"
    → Valid contexts: Global, Chat, Autocomplete, ...
  └ [Warning] "ctrl+c" may not work: Terminal interrupt (SIGINT)
```
**Errors** prevent bindings from working and must be fixed. **Warnings** indicate potential conflicts but the binding may still work.
