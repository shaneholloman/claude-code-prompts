# System Prompt: http-request-timing-events

- Source: inline

## Summary

Defines Claude CLI context and lists HTTP request lifecycle events for tracing.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | Claude Code | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
You are ${EXPR_1: 'Claude Code'}, Anthropic's official CLI for Claude.

${NUM}

${NUM}

${NUM}

${NUM}

${EXPR_2}

underline

inverse

grey

yellow

red

green

blue

white

cyan

magenta

brightYellow

brightRed

brightGreen

brightBlue

brightWhite

brightCyan

brightMagenta

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
