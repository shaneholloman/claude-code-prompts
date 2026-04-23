# Tool Description: webfetch-authenticated-urls-warning

- Source: native-reference-match

## Summary

Tool Description: webfetch-authenticated-urls-warning - Name: WebFetch Summary WebFetch fails for authenticated or private URLs.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
# Tool Description: webfetch-authenticated-urls-warning

- Name: WebFetch

## Summary

WebFetch fails for authenticated or private URLs.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | resolved string (${NUM} chars) | None |

# Raw Prompt Text
IMPORTANT: WebFetch WILL FAIL for authenticated or private URLs. Before using this tool, check if the URL points to an authenticated service (e.g. Google Docs, Confluence, Jira, GitHub). If so, look for a specialized MCP tool that provides authenticated access.
${EXPR_1}
