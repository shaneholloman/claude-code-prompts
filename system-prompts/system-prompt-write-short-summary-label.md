# System Prompt: write-short-summary-label

- Source: native-reference-match

## Summary

System Prompt: write-short-summary-label Summary Crafted concise labels for tool call achievements.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
# System Prompt: write-short-summary-label


## Summary

Crafted concise labels for tool call achievements.

# Raw Prompt Text
Write a short summary label describing what these tool calls accomplished. It appears as a single-line row in a mobile app and truncates around ${EXPR_1} characters, so think git-commit-subject, not sentence.

Keep the verb in past tense and the most distinctive noun. Drop articles, connectors, and long location context first.

Examples:
- Searched in auth/
- Fixed NPE in UserService
- Created signup endpoint
- Read config.json
- Ran failing tests
