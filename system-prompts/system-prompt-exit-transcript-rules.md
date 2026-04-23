# System Prompt: exit-transcript-rules

- Source: native-reference-match

## Summary

System Prompt: exit-transcript-rules - Source: inline Summary Specifies how stdout and stderr are displayed for tool call inputs and responses by exit code.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# System Prompt: exit-transcript-rules

- Source: inline

## Summary

Specifies how stdout and stderr are displayed for tool call inputs and responses by exit code.

# Raw Prompt Text
Input to command is JSON with fields "inputs" (tool call arguments) and "response" (tool call response).
Exit code ${EXPR_1} - stdout shown in transcript mode (ctrl+o)
Exit code ${EXPR_2} - show stderr to model immediately
Other exit codes - show stderr to user only
