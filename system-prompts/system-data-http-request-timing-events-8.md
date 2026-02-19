# System Data Block: http-request-timing-events-8

- Source: inline

## Summary

Register HTTP timing hooks for redirect, DNS, connect, TLS, request, and response.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
${EXPR_1}

permissions

sandbox

hooks

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
