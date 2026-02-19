# System Prompt: api-output-token-limit

- Source: inline

## Summary

Error reports Claude output exceeded token limit, referencing configured submit hook expression

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
API Error: Claude's response exceeded the <user-prompt-submit-hook>${EXPR_1}

[output truncated - exceeded ${NUM} characters]<${PATH}> output token maximum. To configure this behavior, set the CLAUDE_CODE_MAX_OUTPUT_TOKENS environment variable.
