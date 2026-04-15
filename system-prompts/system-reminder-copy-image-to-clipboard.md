# System Reminder: copy-image-to-clipboard

- Source: inline

## Summary

Loads an image file and sets it to the Windows clipboard.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Add-Type -AssemblyName System.Windows.Forms; [System.Windows.Forms.Clipboard]::SetImage([System.Drawing.Image]::FromFile('${EXPR_1}'))
