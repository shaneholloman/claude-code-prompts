# System Data Block: remote-review-notification

- Source: inline

## Summary

Notification for completed remote review task.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
<task-notification>
<task-id>${EXPR_1}<${PATH}>
<task-type>remote_agent<${PATH}>
<status>completed<${PATH}>
<summary>Remote review completed<${PATH}>
<${PATH}>
The remote review produced the following findings:

${EXPR_2}
