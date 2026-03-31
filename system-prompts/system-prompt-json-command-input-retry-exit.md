# System Prompt: json-command-input-retry-exit

- Source: inline

## Summary

Handles JSON command inputs and exit codes.

# Raw Prompt Text
Input to command is JSON with tool_name, tool_input, tool_use_id, and reason.
Return {"hookSpecificOutput":{"hookEventName":"PermissionDenied","retry":true}} to tell the model it may retry.
Exit code ${NUM} - stdout shown in transcript mode (ctrl+o)
Other exit codes - show stderr to user only
