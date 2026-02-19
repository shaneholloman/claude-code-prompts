# System Prompt: synthesize-multiple-outputs

- Source: inline

## Summary

Synthesize multi-agent findings into one structured, contradiction-resolved solution with full details and code.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | Write | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |

# Raw Prompt Text
${EXPR_1: 'Write'}

${EXPR_2}

${EXPR_3}

-Uli

--multiline-dotall

${EXPR_4}

up

mid

down

args

Original task: ${EXPR_5}

I've assigned multiple agents to tackle this task. Each agent has analyzed the problem and provided their findings.

${EXPR_6}

Based on all the information provided by these agents, synthesize a comprehensive and cohesive response that:
${NUM}. Combines the key insights from all agents
${NUM}. Resolves any contradictions between agent findings
${NUM}. Presents a unified solution that addresses the original task
${NUM}. Includes all important details and code examples from the individual responses
${NUM}. Is well-structured and complete

Your synthesis should be thorough but focused on the original task.

${EXPR_7}

${EXPR_8}

${EXPR_9}

${EXPR_10}
