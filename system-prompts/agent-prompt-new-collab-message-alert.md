# Agent Prompt: new-collab-message-alert

- Agent Type: null
- When to use: stdio
- Model: unknown
- Source: plugin
- Color: firstParty

## Summary

System reminder announcing new collaboration messages from a specified source.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | unknown | None |

# Raw Prompt Text
<system-reminder>New collab messages from ${EXPR_1: 'unknown'}.<${PATH}>
