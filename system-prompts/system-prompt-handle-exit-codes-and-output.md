# System Prompt: handle-exit-codes-and-output

- Source: inline

## Summary

Routes stdout and stderr visibility based on exit code and continues execution when needed.

# Raw Prompt Text
Exit code ${NUM} - Stdout${PATH} not shown
Exit code ${NUM} - show stderr to subagent and continue having it run
Other exit codes - show stderr to user only
