# System Prompt: read-large-output-in-chunks

- Source: inline

## Summary

Guides reading oversized saved output in chunks, searching with grep/jq, meeting coverage threshold

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
Error: result (${EXPR_1} characters) exceeds maximum allowed tokens. Output has been saved to ${EXPR_2}.
Format: ${EXPR_3}
Use offset and limit parameters to read specific portions of the file, the Grep tool to search for specific content, and jq to make structured queries.
REQUIREMENTS FOR SUMMARIZATION${PATH}:
- You MUST read the content from the file at ${EXPR_4} in sequential chunks until ${NUM}% of the content has been read.
