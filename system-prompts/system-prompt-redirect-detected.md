# System Prompt: redirect-detected

- Source: inline

## Summary

Instruction to refetch a redirected URL using updated WebFetch parameters.

# Raw Prompt Text
REDIRECT DETECTED: The URL redirects to a different host.

Original URL: ${EXPR_1}
Redirect URL: ${EXPR_2}
Status: ${EXPR_3} ${EXPR_4}

To complete your request, I need to fetch content from the redirected URL. Please use WebFetch again with these parameters:
- url: "${EXPR_5}"
- prompt: "${EXPR_6}"
