# Claude Code 1.0.52 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `claude_code_docs_config` | config | prompts | Configures CLI assistant documentation instructions and URL safety guidance in prompt | Appears to load docs-related prompt/config content. | high | 1 |
| `claude_code_unicode_sanitize` | gate | tools | Optionally sanitize Unicode in MCP tool and prompt lists before mapping results. | IL() behavior not shown; inferred as sanitization step. | high | 2 |
| `force_local_installation_migration` | gate | tools | Forces CLI migration from global npm install to local installation with restart prompt | Triggered only when additional runtime checks pass. | high | 1 |
| `tengu_metrics_exporter_enabled` | gate | telemetry | Enables internal metrics exporting via HTTP with JSON payload and user agent |  | high | 1 |
| `tengu_native_installation` | gate | filesystem | Controls whether CLI creates/uses native launcher script when claude.sh missing | Inference based on file checks and symlink creation logic. | medium | 1 |
| `tengu_version_config` | config | ui | Checks minimum required CLI version and instructs user to update if outdated. | Used for runtime version gating and update messaging. | high | 1 |
