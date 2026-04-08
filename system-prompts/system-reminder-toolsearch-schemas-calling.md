# System Prompt: toolsearch-schemas-calling

- Source: inline

## Summary

Use ToolSearch to load tool schemas before calling.

# Raw Prompt Text
The following deferred tools are now available via ToolSearch. Their schemas are NOT loaded — calling them directly will fail with InputValidationError. Use ToolSearch with query "select:<name>[,<name>...]" to load tool schemas before calling them:
${EXPR_1}
