# System Reminder: copy-image-to-clipboard

- Source: inline

## Summary

Load an image from a file path and copy it to Windows clipboard.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | image file path | None |

# Raw Prompt Text
Add-Type -AssemblyName System.Windows.Forms; [System.Windows.Forms.Clipboard]::SetImage([System.Drawing.Image]::FromFile('${EXPR_1}
