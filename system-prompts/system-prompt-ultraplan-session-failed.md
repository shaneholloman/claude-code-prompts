# System Prompt: ultraplan-session-failed

- Source: inline

## Summary

Notification of a failed Ultraplan session.

# Raw Prompt Text
<task-notification>
<task-id>${EXPR_1}<${PATH}>
<task-type>remote_agent<${PATH}>
<status>failed<${PATH}>
<summary>Ultraplan failed: ${EXPR_2}<${PATH}>
<${PATH}>
The remote Ultraplan session did not produce a plan (${EXPR_3}). Inspect the session at ${EXPR_4} and tell the user to retry locally with plan mode.
