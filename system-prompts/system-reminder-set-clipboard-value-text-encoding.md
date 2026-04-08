# System Prompt: set-clipboard-value-text-encoding

- Source: inline

## Summary

Sets clipboard value using UTF8 encoding.

# Raw Prompt Text
Set-Clipboard -Value ([Text.Encoding]::UTF8.GetString([Convert]::FromBase64String('${EXPR_1}')))
