# System Prompt: github-url-redirect-detected

- Source: inline

## Summary

Notification of a URL redirect issue.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |

# Raw Prompt Text
REDIRECT DETECTED: The URL redirects to a different host.

Original URL: ${EXPR_1}
Redirect URL: ${EXPR_2}
Status: ${EXPR_3} GitHub not connected for ${EXPR_4}/${EXPR_5} — run ${PATH} to sync your GitHub credentials, or install the Claude GitHub App at ${URL}

To complete your request, I need to fetch content from the redirected URL. Please use WebFetch again with these parameters:
- url: "${EXPR_6}"
- prompt: "${EXPR_7}"
