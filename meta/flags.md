# Claude Code 1.0.3 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `claude_code_unicode_sanitize` | gate | tools | Optionally sanitize Unicode in MCP tool and prompt lists before mapping results. | IL() behavior not shown; inferred as sanitization step. | high | 4 |
| `contents_identical` | gate | other | Detects identical message contents to avoid further comparison or resolution. | Exact effect of W() and return value semantics unclear. | medium | 1 |
| `force_local_installation_migration` | gate | tools | Forces CLI migration from global npm install to local installation with restart prompt | Triggered only when additional runtime checks pass. | high | 1 |
| `missing_file_edits` | gate | tools | Detects missing file-edit tool calls during tool-use validation between two message contents. | Exact tool name f3 is obfuscated; inferred as file edits tool. | high | 1 |
| `tool_use_invalid` | gate | tools | Detects invalid tool call content during message comparison and aborts | Based on tool_use validation logic in CLI diff/compare flow. | high | 1 |
