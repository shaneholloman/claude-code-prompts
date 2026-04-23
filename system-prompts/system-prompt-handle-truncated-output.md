# System Prompt: handle-truncated-output

- Source: native-reference-match

## Summary

System Prompt: handle-truncated-output - Source: inline Summary Handle MCP output truncation by paging… retrieval or warning results may be incomplete.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
# System Prompt: handle-truncated-output

- Source: inline

## Summary

Handle MCP output truncation by paging${PATH} retrieval or warning results may be incomplete.

# Raw Prompt Text
[OUTPUT TRUNCATED - exceeded ${EXPR_1} token limit]

The tool output was truncated. If this MCP server provides pagination or filtering tools, use them to retrieve specific portions of the data. If pagination is not available, inform the user that you are working with truncated output and results may be incomplete.
