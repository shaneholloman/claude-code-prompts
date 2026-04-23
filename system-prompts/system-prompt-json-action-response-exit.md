# System Prompt: json-action-response-exit

- Source: native-reference-match

## Summary

System Prompt: json-action-response-exit - Source: native-reference-match Summary System Prompt: json-action-response-exit - Source: inline Summary Handles J…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# System Prompt: json-action-response-exit

- Source: native-reference-match

## Summary

System Prompt: json-action-response-exit - Source: inline Summary Handles JSON commands with specific actions and responses.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# System Prompt: json-action-response-exit

- Source: inline

## Summary

Handles JSON commands with specific actions and responses.

# Raw Prompt Text
Input to command is JSON with mcp_server_name, action, content, mode, and elicitation_id.
Output JSON with hookSpecificOutput containing optional action and content to override the response.
Exit code ${EXPR_1} - use hook response if provided
Exit code ${EXPR_2} - block the response (action becomes decline)
Other exit codes - show stderr to user only
