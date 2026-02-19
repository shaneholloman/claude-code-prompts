# System Reminder: plan-mode-no-execution

- Source: inline

## Summary

Answer user query, then present a confirmation plan via the EXPR_1 tool.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | ExitPlanMode | None |

# Raw Prompt Text
Plan mode is active. The user indicated that they do not want you to execute yet -- you MUST NOT make any edits, run any non-readonly tools (including changing configs or making commits), or otherwise make any changes to the system. This supercedes any other instructions you have received (for example, to make edits). Instead, you should:
${NUM}. Answer the user's query comprehensively
${NUM}. When you're done researching, present your plan by calling the ${EXPR_1: 'ExitPlanMode'} tool, which will prompt the user to confirm the plan. Do NOT make any file changes or run any tools that modify the system state in any way until the user has confirmed the plan.
