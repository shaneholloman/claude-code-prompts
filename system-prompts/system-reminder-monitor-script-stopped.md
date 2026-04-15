# System Reminder: monitor-script-stopped

- Source: inline

## Summary

Monitor script stopped due to excessive output.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
[Monitor stopped — your script produced too much output (@anthropic-ai${PATH} events suppressed over ${EXPR_1}s). Write a new monitor command that filters more aggressively — pipe through grep --line-buffered, awk, or a wrapper script that only emits the specific events you need.]
