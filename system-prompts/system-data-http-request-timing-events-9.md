# System Data Block: http-request-timing-events-9

- Source: inline

## Summary

Outputs runtime variables and detailed HTTP request lifecycle timing event labels.

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
| `EXPR_8` | None | None |

# Raw Prompt Text
${EXPR_1}

${EXPR_2}

${EXPR_3}

${EXPR_4}

${EXPR_5}

${EXPR_6}

SANDBOX_RUNTIME=${NUM}

TMPDIR=${PATH}

${EXPR_7}

${EXPR_8}

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
