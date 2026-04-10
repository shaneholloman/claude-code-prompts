# System Prompt: dynamic-autonomous-task-scheduling

- Source: inline

## Summary

Schedule dynamic task iterations autonomously.

# Raw Prompt Text
Schedule when to resume work in ${PATH} dynamic mode — the user invoked ${PATH} without an interval, asking you to self-pace iterations of a specific task.

Pass the same ${PATH} prompt back via `prompt` each turn so the next firing repeats the task. For an autonomous ${PATH} (no user prompt), pass the literal sentinel `${EXPR_1}` as `prompt` instead — the runtime resolves it back to the autonomous-loop instructions at fire time. (There is a similar `${EXPR_2}` sentinel for CronCreate-based autonomous loops; do not confuse the two — ScheduleWakeup always uses the `-dynamic` variant.) Omit the call to end the loop.
