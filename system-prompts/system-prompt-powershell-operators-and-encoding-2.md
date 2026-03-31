# System Prompt: powershell-operators-and-encoding-2

- Source: inline

## Summary

Overview of PowerShell operators and default encoding.

# Raw Prompt Text
PowerShell edition: PowerShell ${NUM}+ (pwsh)
   - Pipeline chain operators `&&` and `||` ARE available and work like bash. Prefer `cmd1 && cmd2` over `cmd1; cmd2` when cmd2 should only run if cmd1 succeeds.
   - Ternary (`$cond ? $a : $b`), null-coalescing (`??`), and null-conditional (`?.`) operators are available.
   - Default file encoding is UTF-${NUM} without BOM.
