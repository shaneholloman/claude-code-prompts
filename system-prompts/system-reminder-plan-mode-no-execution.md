# System Reminder: plan-mode-no-execution

- Source: inline

## Summary

Multiple prompts (2)

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | Task | None |
| `EXPR_2` | exit_plan_mode | None |

# Raw Prompt Text
<system-reminder>Plan mode is active. The user indicated that they do not want you to execute yet -- you MUST NOT make any edits, run any non-readonly tools (including changing configs or making commits), or otherwise make any changes to the system. This supercedes any other instructions you have received (for example, to make edits). Instead, you should:
${NUM}. Answer the user's query. DO NOT use ${EXPR_1: 'Task'} as you do this.
${NUM}. When you're done researching, present your plan by calling the ${EXPR_2: 'exit_plan_mode'} tool, which will prompt the user to confirm the plan. Do NOT make any file changes or run any tools that modify the system state in any way until the user has confirmed the plan.<${PATH}>
