# System Prompt: copy-image-to-clipboard

- Source: inline

## Summary

Loads an image file and sets it to the Windows clipboard.

# Raw Prompt Text
Add-Type -AssemblyName System.Windows.Forms; [System.Windows.Forms.Clipboard]::SetImage([System.Drawing.Image]::FromFile('${EXPR_1}'))
