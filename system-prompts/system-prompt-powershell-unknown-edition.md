# System Prompt: powershell-unknown-edition

- Source: inline

## Summary

Assume Windows PowerShell for compatibility.

# Raw Prompt Text
PowerShell edition: unknown — assume Windows PowerShell ${NUM} for compatibility
   - Do NOT use `&&`, `||`, ternary `?:`, null-coalescing `??`, or null-conditional `?.`. These are PowerShell ${NUM}+ only and parser-error on ${NUM}.
   - To chain commands conditionally: `A; if ($?) { B }`. Unconditionally: `A; B`.
