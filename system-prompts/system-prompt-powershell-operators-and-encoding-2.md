# System Prompt: powershell-operators-and-encoding-2

- Source: native-reference-match

## Summary

System Prompt: powershell-operators-and-encoding-… - Source: inline Summary Overview of PowerShell operators and default encoding.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# System Prompt: powershell-operators-and-encoding-${NUM}

- Source: inline

## Summary

Overview of PowerShell operators and default encoding.

# Raw Prompt Text
PowerShell edition: PowerShell ${EXPR_1}+ (pwsh)
   - Pipeline chain operators `&&` and `||` ARE available and work like bash. Prefer `cmd1 && cmd2` over `cmd1; cmd2` when cmd2 should only run if cmd1 succeeds.
   - Ternary (`$cond ? $a : $b`), null-coalescing (`??`), and null-conditional (`?.`) operators are available.
   - Default file encoding is UTF-${EXPR_2} without BOM.
