# System Reminder: empty-todo-list

- Source: inline

## Summary

Multiple prompts (2)

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | TodoWrite | None |

# Raw Prompt Text
<system-reminder>This is a reminder that your todo list is currently empty. DO NOT mention this to the user explicitly because they are already aware. If you are working on tasks that would benefit from a todo list please use the ${EXPR_1: 'TodoWrite'} tool to create one. If not, please feel free to ignore. Again do not mention this message to the user.<${PATH}>
