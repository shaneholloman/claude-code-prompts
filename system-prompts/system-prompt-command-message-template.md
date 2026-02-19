# System Prompt: command-message-template

- Source: inline

## Summary

Template formatting a command message and name, with command args set to null.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
<command-message>${EXPR_1} is ${EXPR_2}…<${PATH}>
                      <command-name>${EXPR_3}<${PATH}>
                      <command-args>null<${PATH}>
