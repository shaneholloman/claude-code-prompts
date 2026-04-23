# System Reminder: search-disabled-unsupported

- Source: inline

## Summary

States tool search is disabled because the model lacks tool_reference support.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Tool search disabled for model '${EXPR_1}': model does not support tool_reference blocks. This feature is only available on Claude Sonnet ${NUM}+, Opus ${NUM}+, and newer models.
