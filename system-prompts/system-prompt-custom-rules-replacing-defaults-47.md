# System Prompt: custom-rules-replacing-defaults-47

- Source: inline

## Summary

Defines custom rules to replace default settings.

# Raw Prompt Text
<task-notification>
<task-id>${EXPR_1}<${PATH}>npm view ${EXPR_2}@${EXPR_3} version
<task-type>remote_agent<${PATH}>
<output-file>## allow (custom rules replacing defaults)
Custom:
${EXPR_4}

Defaults being replaced:
${EXPR_5}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_6}

Defaults being replaced:
${EXPR_7}

## environment (custom rules replacing defaults)
Custom:
${EXPR_8}

Defaults being replaced:
${EXPR_9}

<${PATH}>
<status>${EXPR_10}<${PATH}>
<summary>Remote task "${EXPR_11}" stable<${PATH}>
<${PATH}>
