# Tool Description: load-deferred-tools-2

- Name: ToolSearch

## Summary

Discover and load deferred tools via search or selection before invoking them

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | resolved string (2462 chars) | None |

# Raw Prompt Text
Search for or select deferred tools to make them available for use.

**MANDATORY PREREQUISITE - THIS IS A HARD REQUIREMENT**

You MUST use this tool to load deferred tools BEFORE calling them directly.

This is a BLOCKING REQUIREMENT - deferred tools are NOT available until you load them using this tool. Look for <available-deferred-tools> messages in the conversation for the list of tools you can discover. Both query modes (keyword search and direct selection) load the returned tools — once a tool appears in the results, it is immediately available to call.${EXPR_1}
