# System Reminder: github-autonomous-global-scheduling

- Source: inline

## Summary

Instructions for scheduled autonomous tasks and GitHub sync.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | CronDelete | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
global@anthropic-ai${PATH}'s scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_1} days, and that they can cancel sooner with ${EXPR_2: 'CronDelete'} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.GitHub not connected for ${EXPR_3}/${EXPR_4} — run ${PATH} to sync your GitHub credentials, or install the Claude GitHub App at ${URL} (PID ${EXPR_5})${EXPR_6}
