# System Prompt: de237656

- Source: inline

## Summary

When NOT to use the Agent tool: - If you want to read a specific file path, use the Read or Glob tool instead of the Agent tool, to find the match more quick…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
When NOT to use the Agent tool:
- If you want to read a specific file path, use the Read tool or ${EXPR_1} instead of the Agent tool, to find the match more quickly
- If you are searching for a specific class definition like "class Foo", use unknown instead, to find the match more quickly
- If you are searching for code within a specific file or set of ${NUM}-${NUM} files, use the Read tool instead of the Agent tool, to find the match more quickly
- Other tasks that are not related to the agent descriptions above
