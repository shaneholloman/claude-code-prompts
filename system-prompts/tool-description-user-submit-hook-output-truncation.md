# Tool Description: user-submit-hook-output-truncation


## Summary

Wraps submitted user prompt in hook tags and appends truncation marker.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
<user-prompt-submit-hook>${EXPR_1}

[output truncated - exceeded ${NUM} characters]<${PATH}>
