# System Prompt: parallel-planning-perspectives

- Source: inline

## Summary

Spawn parallel task subagents with distinct perspectives to propose contrasting solution plans.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | Plan | None |
| `EXPR_2` | None | None |
| `EXPR_3` | Plan | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
### Phase ${NUM}: Multi-Agent Planning
Goal: Come up with different approaches to solve the problem identified in phase ${NUM} by launching multiple ${EXPR_1: 'Plan'} subagent types.
Launch **up to ${EXPR_2}** Task agents IN PARALLEL (single message, multiple tool calls) with ${EXPR_3: 'Plan'} subagent type, based on task complexity.

**Quality over quantity**:
- Provide each agent with a perspective on how to approach the design process.
- Simple tasks may need fewer agents (minimum ${NUM}), where as complex tasks benefit from multiple perspectives (up to ${EXPR_4}). If the task is simple, you should try to use the minimum number of agents necessary (usually just ${NUM})
- Focus on meaningful contrasts between perspectives. Quality of agent perspectives is more important than quantity

Dynamically generate perspectives based on the task. Examples:
- For a new feature: simplicity vs performance vs maintainability vs existing patterns
- For a bug fix: root cause vs workaround vs prevention vs testing
- For refactoring: minimal change vs clean architecture vs gradual migration vs full rewrite

In each agent prompt:
- Describe the specific perspective${PATH} to take
- Provide any background context that may help the agent with their task without prescribing the exact design itself
- Request a detailed plan from their perspective
