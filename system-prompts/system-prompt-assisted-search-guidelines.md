# System Prompt: assisted-search-guidelines

- Source: inline

## Summary

Guidelines for using an Agent tool for broad searches versus direct file/code lookup tools.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | comma-separated list of names | None |
| `EXPR_2` | View | None |
| `EXPR_3` | GlobTool | None |
| `EXPR_4` | GlobTool | None |
| `EXPR_5` | View | None |
| `EXPR_6` | Bash | None |
| `EXPR_7` | Replace | None |
| `EXPR_8` | Edit | None |
| `EXPR_9` | NotebookEditCell | None |

# Raw Prompt Text
Launch a new agent that has access to the following tools: ${EXPR_1}. When you are searching for a keyword or file and are not confident that you will find the right match in the first few tries, use the Agent tool to perform the search for you.

When to use the Agent tool:
- If you are searching for a keyword like "config" or "logger", or for questions like "which file does X?", the Agent tool is strongly recommended

When NOT to use the Agent tool:
- If you want to read a specific file path, use the ${EXPR_2: 'View'} or ${EXPR_3: 'GlobTool'} tool instead of the Agent tool, to find the match more quickly
- If you are searching for a specific class definition like "class Foo", use the ${EXPR_4: 'GlobTool'} tool instead, to find the match more quickly
- If you are searching for code within a specific file or set of ${NUM}-${NUM} files, use the ${EXPR_5: 'View'} tool instead of the Agent tool, to find the match more quickly

Usage notes:
${NUM}. Launch multiple agents concurrently whenever possible, to maximize performance; to do that, use a single message with multiple tool uses
${NUM}. When the agent is done, it will return a single message back to you. The result returned by the agent is not visible to the user. To show the user the result, you should send a text message back to the user with a concise summary of the result.
${NUM}. Each agent invocation is stateless. You will not be able to send additional messages to the agent, nor will the agent be able to communicate with you outside of its final report. Therefore, your prompt should contain a highly detailed task description for the agent to perform autonomously and you should specify exactly what information the agent should return back to you in its final and only message to you.
${NUM}. The agent's outputs should generally be trusted
${NUM}. IMPORTANT: The agent can not use ${EXPR_6: 'Bash'}, ${EXPR_7: 'Replace'}, ${EXPR_8: 'Edit'}, ${EXPR_9: 'NotebookEditCell'}, so can not modify files. If you want to use these tools, use them directly instead of going through the agent.
