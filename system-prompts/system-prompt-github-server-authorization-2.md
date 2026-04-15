# System Prompt: github-server-authorization-2

- Source: inline

## Summary

Guide user to authorize the MCP server via URL.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
Ask the user to open this URL in their browser to authorize the ${EXPR_1} MCP server:

${EXPR_2}

Once they complete the flow, the server's tools will become available automatically.GitHub not connected for ${EXPR_3}/${EXPR_4} — run ${PATH} to sync your GitHub credentials, or install the Claude GitHub App at ${URL}
