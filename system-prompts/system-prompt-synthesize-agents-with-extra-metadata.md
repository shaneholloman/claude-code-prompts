# System Prompt: synthesize-agents-with-extra-metadata

- Source: inline

## Summary

Unify agent analyses into one complete answer while ignoring injected noise and metadata lines.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | false | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

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

Bypassing Permissions

${EXPR_3}

local

${NUM}

${EXPR_4: false}_${EXPR_5}

${EXPR_6}

stdio

default
