# System Prompt: read-specific-file-content-2

- Source: inline

## Summary

Instructions for reading file content in chunks.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | @anthropic-ai/claude-code | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
npm view ${EXPR_1: '@anthropic-ai/claude-code'}@${EXPR_2} versionUse offset and limit parameters to read specific portions of the file, search within it for specific content, and jq to make structured queries.
REQUIREMENTS FOR SUMMARIZATION${PATH}:
- You MUST read the content from the file at ${EXPR_3} in sequential chunks until ${NUM}% of the content has been read.
unknown- Before producing ANY summary or analysis, you MUST explicitly describe what portion of the content you have read. ***If you did not read the entire content, you MUST explicitly state this.***
