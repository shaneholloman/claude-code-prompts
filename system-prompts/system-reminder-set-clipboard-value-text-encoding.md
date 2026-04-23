# System Reminder: set-clipboard-value-text-encoding

- Source: inline

## Summary

Sets clipboard value using UTF8 encoding.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Set-Clipboard -Value ([Text.Encoding]::UTF8.GetString([Convert]::FromBase64String('${EXPR_1}')))
