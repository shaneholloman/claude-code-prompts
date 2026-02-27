# System Prompt: 86a262a7

- Source: inline

## Summary

Defines Task tool subagent types and requires selecting subagent_type for autonomous tasks

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Launch a new agent to handle complex, multi-step tasks autonomously.

The Task tool launches specialized agents (subprocesses) that autonomously handle complex tasks. Each agent type has specific capabilities and tools available to it.

Available agent types and the tools they have access to:
${EXPR_1}

When using the Task tool, you must specify a subagent_type parameter to select which agent type to use.
