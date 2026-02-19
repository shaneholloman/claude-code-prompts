# System Data Block: http-request-timing-events

- Source: inline

## Summary

Provide HTTP request timing event markers from redirect start through response end.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
${EXPR_1}

${EXPR_2}

${EXPR_3}

http.request.redirect_start

http.request.fetch_start

http.request.domain_lookup_start

http.request.domain_lookup_end

http.request.connect_start

http.request.secure_connection_start

http.request.connection_end

http.request.request_start

http.request.response_start

http.request.response_end
