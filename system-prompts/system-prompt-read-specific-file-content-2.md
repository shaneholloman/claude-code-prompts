# System Prompt: read-specific-file-content-2

- Source: inline

## Summary

Read file content in chunks and summarize portions.

# Raw Prompt Text
${EXPR_1}Use offset and limit parameters to read specific portions of the file, search within it for specific content, and jq to make structured queries.
REQUIREMENTS FOR SUMMARIZATION${PATH}:
- You MUST read the content from the file at ${EXPR_2} in sequential chunks until ${NUM}% of the content has been read.
${EXPR_3}- Before producing ANY summary or analysis, you MUST explicitly describe what portion of the content you have read. ***If you did not read the entire content, you MUST explicitly state this.***
