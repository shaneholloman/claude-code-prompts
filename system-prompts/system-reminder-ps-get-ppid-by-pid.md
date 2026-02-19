# System Reminder: ps-get-ppid-by-pid

- Source: inline

## Summary

Use ps to output the parent process ID for a specified PID.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
ps -o ppid= -p ${EXPR_1}
