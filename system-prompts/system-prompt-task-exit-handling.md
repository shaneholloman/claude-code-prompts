# System Prompt: task-exit-handling

- Source: native-reference-match

## Summary

System Prompt: task-exit-handling - Source: inline Summary Multiple prompts (…) Raw Prompt Text Input to command is JSON with task_id, task_subject, task_des…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
# System Prompt: task-exit-handling

- Source: inline

## Summary

Multiple prompts (${NUM})

# Raw Prompt Text
Input to command is JSON with task_id, task_subject, task_description, teammate_name, and team_name.
Exit code ${EXPR_1} - stdout${EXPR_2} not shown
Exit code ${EXPR_3} - show stderr to model and prevent task completion
Other exit codes - show stderr to user only
