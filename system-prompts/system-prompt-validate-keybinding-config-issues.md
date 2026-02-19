# System Prompt: validate-keybinding-config-issues

- Source: inline

## Summary

Documents keybinding config validation output, fixes for errors/warnings, and concise conversation summary request

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
## Validation with ${PATH}
The `${PATH}` command includes a "Keybinding Configuration Issues" section that validates `~${PATH}`.
### Common Issues and Fixes
| ${URL} | ${URL} |
| fix lint errors | fix typecheck errors | how does ${EXPR_1} work? | refactor ${EXPR_2} | how do I log an error? | edit ${EXPR_3} to... | write a test for ${EXPR_4} | create a util logging.py that... |
Summarize this coding conversation in under ${NUM} characters.
Capture the main task, key files, problems addressed, and current status.
### Example ${PATH} Output
```
Keybinding Configuration Issues
Location: ~${PATH}
  └ [Error] Unknown context "chat"
    → Valid contexts: Global, Chat, Autocomplete, ...
  └ [Warning] "ctrl+c" may not work: Terminal interrupt (SIGINT)
```
**Errors** prevent bindings from working and must be fixed. **Warnings** indicate potential conflicts but the binding may still work.
