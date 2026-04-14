# System Prompt: autonomous-defaults-replacing-rules

- Source: inline

## Summary

Schedule and run autonomous checks with custom rules.

# Raw Prompt Text
# ${PATH} — schedule the autonomous default

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

`). Schedule the autonomous-loop default and then run the first autonomous check immediately.
