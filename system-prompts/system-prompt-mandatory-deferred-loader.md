# System Prompt: mandatory-deferred-loader

- Source: inline

## Summary

Enforces searching or selecting deferred tools to load them before any direct calls

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | resolved string (2462 chars) | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
Search for or select deferred tools to make them available for use.

**MANDATORY PREREQUISITE - THIS IS A HARD REQUIREMENT**

You MUST use this tool to load deferred tools BEFORE calling them directly.

This is a BLOCKING REQUIREMENT - deferred tools listed below are NOT available until you load them using this tool. Both query modes (keyword search and direct selection) load the returned tools — once a tool appears in the results, it is immediately available to call.${EXPR_1}

Available deferred tools (must be loaded before use):
${EXPR_2}
