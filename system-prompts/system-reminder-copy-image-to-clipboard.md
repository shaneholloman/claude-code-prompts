# System Reminder: a6e8da12

- Source: inline

## Summary

Load an image from a file path and copy it to Windows clipboard.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | value after fromfile | None |

# Raw Prompt Text
Add-Type -AssemblyName System.Windows.Forms; [System.Windows.Forms.Clipboard]::SetImage([System.Drawing.Image]::FromFile('${EXPR_1}
