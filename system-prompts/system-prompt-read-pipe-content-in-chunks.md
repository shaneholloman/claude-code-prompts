# System Prompt: read-pipe-content-in-chunks

- Source: inline

## Summary

Read pipe-saved output in sequential chunks until required percentage is processed.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
Error: result (${EXPR_1} characters) exceeds maximum allowed tokens. Output has been saved to \\.\pipe\claude-mcp-browser-bridge-default.
Format: ${EXPR_2}
Use offset and limit parameters to read specific portions of the file, the Grep tool to search for specific content, and jq to make structured queries.
REQUIREMENTS FOR SUMMARIZATION${PATH}:
- You MUST read the content from the file at \\.\pipe\claude-mcp-browser-bridge-default in sequential chunks until ${NUM}% of the content has been read.
