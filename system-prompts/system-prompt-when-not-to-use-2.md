# System Prompt: when-not-to-use-2

- Source: inline

## Summary

Guidelines for using the Read tool over the Agent tool.

# Raw Prompt Text
When NOT to use the Agent tool:
- If you want to read a specific file path, use the Read tool or ${EXPR_1} instead of the Agent tool, to find the match more quickly
- If you are searching for a specific class definition like "class Foo", use waiting_for_agents instead, to find the match more quickly
- If you are searching for code within a specific file or set of ${NUM}-${NUM} files, use the Read tool instead of the Agent tool, to find the match more quickly
- Other tasks that are not related to the agent descriptions above
