# System Prompt: multi-synthesis

- Source: inline

## Summary

Synthesize multiple agents’ analyses into one unified, contradiction-resolved response for the original task

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
Original task: ${EXPR_1}

I've assigned multiple agents to tackle this task. Each agent has analyzed the problem and provided their findings.

${EXPR_2}

Based on all the information provided by these agents, synthesize a comprehensive and cohesive response that:
${NUM}. Combines the key insights from all agents
${NUM}. Resolves any contradictions between agent findings
${NUM}. Presents a unified solution that addresses the original task
${NUM}. Includes all important details and code examples from the individual responses
${NUM}. Is well-structured and complete

Your synthesis should be thorough but focused on the original task.
