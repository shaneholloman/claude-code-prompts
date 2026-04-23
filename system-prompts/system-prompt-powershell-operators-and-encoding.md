# System Prompt: powershell-operators-and-encoding

- Source: inline

## Summary

Guidelines for using PowerShell operators and encoding.

# Raw Prompt Text
PowerShell edition: Windows PowerShell ${NUM} (powershell.exe)
   - Pipeline chain operators `&&` and `||` are NOT available — they cause a parser error. To run B only if A succeeds: `A; if ($?) { B }`. To chain unconditionally: `A; B`.
   - Ternary (`?:`), null-coalescing (`??`), and null-conditional (`?.`) operators are NOT available. Use `if${PATH}` and explicit `$null -eq` checks instead.
   - Avoid `${NUM}>&${NUM}` on native executables. In ${NUM}, redirecting a native command's stderr inside PowerShell wraps each line in an ErrorRecord (NativeCommandError) and sets `$?` to `$false` even when the exe returned exit code ${NUM}. stderr is already captured for you — don't redirect it.
   - Default file encoding is UTF-${NUM} LE (with BOM). When writing files other tools will read, pass `-Encoding utf8` to `Out-File`/`Set-Content`.
   - `ConvertFrom-Json` returns a PSCustomObject, not a hashtable. `-AsHashtable` is not available.
