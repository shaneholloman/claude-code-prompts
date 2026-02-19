# Claude Code 1.0.21 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `claude_code_unicode_sanitize` | gate | tools | Optionally sanitize Unicode in MCP tool and prompt lists before mapping results. | IL() behavior not shown; inferred as sanitization step. | high | 4 |
| `force_local_installation_migration` | gate | tools | Forces CLI migration from global npm install to local installation with restart prompt | Triggered only when additional runtime checks pass. | high | 1 |
| `tengu_remote_mcp` | gate | auth | Enable authenticated SSE connections to MCP servers with request timeout | Only affects B.type==="sse" connection path. | high | 2 |
