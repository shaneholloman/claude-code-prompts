# System Prompt: task-exit-handling

- Source: inline

## Summary

Defines JSON command input and exit-code rules for showing stdout or stderr and completing tasks.

# Raw Prompt Text
Input to command is JSON with task_id, task_subject, task_description, teammate_name, and team_name.
Exit code ${NUM} - stdout${PATH} not shown
Exit code ${NUM} - show stderr to model and prevent task completion
Other exit codes - show stderr to user only
