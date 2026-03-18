# System Prompt: launch-handle-complex-tasks

- Source: inline

## Summary

Create an agent for autonomous multi-step task management.

# Raw Prompt Text
Launch a new agent to handle complex, multi-step tasks autonomously.

The Agent tool launches specialized agents (subprocesses) that autonomously handle complex tasks. Each agent type has specific capabilities and tools available to it.

Available agent types and the tools they have access to:
@anthropic-ai${PATH}

When using the Agent tool, specify a subagent_type to use a specialized agent, or omit it to fork yourself — a fork inherits your full conversation context.
