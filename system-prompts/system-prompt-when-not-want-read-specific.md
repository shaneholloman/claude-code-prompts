# System Prompt: 2b491db7

- Source: inline

## Summary

When NOT to use the Agent tool: - If you want to read a specific file path, use the Read tool or … instead of the Agent tool, to find the match more quickly…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
When NOT to use the Agent tool:
- If you want to read a specific file path, use the Read tool or ${EXPR_1} instead of the Agent tool, to find the match more quickly
- If you are searching for a specific class definition like "class Foo", use ${EXPR_2} loaded with errors instead, to find the match more quickly
- If you are searching for code within a specific file or set of ${NUM}-${NUM} files, use the Read tool instead of the Agent tool, to find the match more quickly
- Other tasks that are not related to the agent descriptions above
