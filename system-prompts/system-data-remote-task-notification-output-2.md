# System Data Block: remote-task-notification-output-2

- Source: inline

## Summary

Remote agent task notification includes status, summary, and output file path to read results

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |

# Raw Prompt Text
<task-notification>
<task-id>${PATH}<${PATH}>
<task-type>remote_agent<${PATH}>
<output-file>mcp__${EXPR_1}__${EXPR_2}<${PATH}>
<status>${EXPR_3}<${PATH}>
<summary>Remote task "${EXPR_4}" [${EXPR_5}] [Claude Chrome Native Host] ${EXPR_6}${EXPR_7}
<${PATH}>
<${PATH}>
Read the output file to retrieve the result: mcp__${EXPR_8}__${EXPR_9}
