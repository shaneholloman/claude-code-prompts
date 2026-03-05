# System Prompt: e8158375

- Source: inline

## Summary

<task-notification> <task-id>…<…> <task-type>remote_agent<…> <status>failed<…> <summary>Ultraplan failed: …<…> <…> The remote Ultraplan session did not produ…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
<task-notification>
<task-id>${EXPR_1}<${PATH}>
<task-type>remote_agent<${PATH}>
<status>failed<${PATH}>
<summary>Ultraplan failed: ${EXPR_2}<${PATH}>
<${PATH}>
The remote Ultraplan session did not produce a plan (${EXPR_3}). Inspect the session at ${EXPR_4} and tell the user to retry locally with plan mode.
