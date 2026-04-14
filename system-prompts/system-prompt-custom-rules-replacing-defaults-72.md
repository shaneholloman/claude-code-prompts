# System Prompt: custom-rules-replacing-defaults-72

- Source: inline

## Summary

Guidelines for using custom rules in codebase searches.

# Raw Prompt Text
For simple, directed codebase searches (e.g. for a specific file${PATH}) use ## allow (custom rules replacing defaults)
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

 directly.

For broader codebase exploration and deep research, use the Agent tool with subagent_type=${EXPR_7}. This is slower than using ## allow (custom rules replacing defaults)
Custom:
${EXPR_8}

Defaults being replaced:
${EXPR_9}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_10}

Defaults being replaced:
${EXPR_11}

## environment (custom rules replacing defaults)
Custom:
${EXPR_12}

Defaults being replaced:
${EXPR_13}

 directly, so use this only when a simple, directed search proves to be insufficient or when your task will clearly require more than ${NUM} queries.
