# Tool Description: check-background-bash-output

- Name: BashOutput

## Summary

Fetch incremental stdout and stderr from a background bash shell, optionally regex-filtered.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
- Retrieves output from a running or completed background bash shell
- Takes a shell_id parameter identifying the shell
- Always returns only new output since the last check
- Returns stdout and stderr output along with shell status
- Supports optional regex filtering to show only lines matching a pattern
- Use this tool when you need to monitor or check the output of a long-running shell
- Shell IDs can be found using the ${PATH} command${EXPR_1}
