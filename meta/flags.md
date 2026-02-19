# Claude Code 0.2.119 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `contents_identical` | gate | other | Detects identical message contents to avoid further comparison or resolution. | Exact effect of W() and return value semantics unclear. | medium | 2 |
| `force_local_installation_migration` | gate | tools | Forces CLI migration from global npm install to local installation with restart prompt | Triggered only when additional runtime checks pass. | high | 1 |
| `missing_file_edits` | gate | tools | Detects missing file-edit tool calls during tool-use validation between two message contents. | Exact tool name f3 is obfuscated; inferred as file edits tool. | high | 2 |
| `tool_use_invalid` | gate | tools | Detects invalid tool call content during message comparison and aborts | Based on tool_use validation logic in CLI diff/compare flow. | high | 2 |
