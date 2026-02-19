# System Prompt: start-coding-after-approval

- Source: inline

## Summary

After plan approval, update todo list and implement code referencing saved plan path.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
User has approved your plan. You can now start coding. Start with updating your todo list if applicable

Your plan has been saved to: ${EXPR_1}
You can refer back to it if needed during implementation.

If this plan can be broken down into multiple independent tasks, consider using a team of teammates (via the Task tool with team_name) to parallelize the work.

## Approved Plan:
${EXPR_2}
