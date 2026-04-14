# System Prompt: custom-rules-replacing-defaults-86

- Source: inline

## Summary

Schedule tasks with custom rules and defaults.

# Raw Prompt Text
# ${PATH} — schedule loop.md tasks

The user invoked `${PATH}` with no prompt (input was empty or just the interval `## allow (custom rules replacing defaults)
Custom:
${EXPR_1}

Defaults being replaced:
${EXPR_2}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_3}

Defaults being replaced:
${EXPR_4}

## environment (custom rules replacing defaults)
Custom:
${EXPR_5}

Defaults being replaced:
${EXPR_6}

`) and has a loop-tasks file at `${EXPR_7}`. Schedule a recurring cron that runs those tasks each tick, then run the first tick immediately.
