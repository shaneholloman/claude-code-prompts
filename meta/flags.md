# Claude Code 1.0.8 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `claude_code_unicode_sanitize` | gate | tools | Optionally sanitize Unicode in MCP tool and prompt lists before mapping results. | IL() behavior not shown; inferred as sanitization step. | high | 4 |
| `force_local_installation_migration` | gate | tools | Forces CLI migration from global npm install to local installation with restart prompt | Triggered only when additional runtime checks pass. | high | 1 |
| `tengu_sub_recommended` | config | ui | Loads a recommended string to display as a first-party CLI tip/shortcut. | Exact downstream use of the loaded value isn’t shown. | medium | 1 |
| `tengu_version_config` | config | ui | Checks minimum required CLI version and instructs user to update if outdated. | Used for runtime version gating and update messaging. | high | 1 |
