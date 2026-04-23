# System Reminder: powershell-get-process-commandline

- Source: inline

## Summary

Run PowerShell CIM query to print a process command line by PID.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
powershell.exe -NoProfile -Command "(Get-CimInstance Win32_Process -Filter \"ProcessId=${EXPR_1}\").CommandLine"
