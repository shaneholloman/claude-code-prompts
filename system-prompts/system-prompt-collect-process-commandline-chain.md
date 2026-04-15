# System Reminder: powershell-process-command-trace

- Source: inline

## Summary

Iterate up parent processes to collect command lines and join into one string.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
$currentPid = ${EXPR_1}
      $commands = @()
      for ($i = ${NUM}; $i -lt ${EXPR_2}; $i++) {
        $proc = Get-CimInstance Win32_Process -Filter "ProcessId=$currentPid" -ErrorAction SilentlyContinue
        if (-not $proc) { break }
        if ($proc.CommandLine) { $commands += $proc.CommandLine }
        if (-not $proc.ParentProcessId -or $proc.ParentProcessId -eq ${NUM}) { break }
        $currentPid = $proc.ParentProcessId
      }
      $commands -join [char]${NUM}
