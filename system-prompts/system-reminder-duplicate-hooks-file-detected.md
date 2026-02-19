# System Reminder: duplicate-hooks-file-detected

- Source: inline

## Summary

Flags duplicate hook load: manifest.hooks points to an already auto-loaded standard hooks file.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | unknown | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
Duplicate hooks file detected: <system-reminder>New collab messages from ${EXPR_1: 'unknown'}.<${PATH}> resolves to already-loaded file ${EXPR_2}. The standard hooks${PATH} is loaded automatically, so manifest.hooks should only reference additional hook files.
