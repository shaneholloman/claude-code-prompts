# Claude Code 1.0.93 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `claude_code_unicode_sanitize` | gate | tools | Optionally sanitize Unicode in MCP tool and prompt lists before mapping results. | IL() behavior not shown; inferred as sanitization step. | high | 2 |
| `force_local_installation_migration` | gate | tools | Forces CLI migration from global npm install to local installation with restart prompt | Triggered only when additional runtime checks pass. | high | 1 |
| `tengu_auto_checkpointing` | gate | ui | Enables showing autocheckpointing availability in the config panel when not disabled by env | Only seen wired into config UI state. | medium | 1 |
| `tengu_feedback_survey_config` | config | ui | Configuration controlling when a feedback survey UI appears and closes | Also appears to emit survey events for tracking. | high | 1 |
| `tengu_metrics_exporter_enabled` | gate | telemetry | Enables internal metrics exporting via HTTP with JSON payload and user agent |  | high | 1 |
| `tengu_native_installation` | gate | filesystem | Controls whether CLI creates/uses native launcher script when claude.sh missing | Inference based on file checks and symlink creation logic. | medium | 1 |
| `tengu_show_all_subscription_types` | gate | ui | Enable displaying all subscription types in a setup or login flow UI | Exact UI/flow unclear from limited snippet. | medium | 1 |
| `tengu_spinner_words` | config | ui | Provides word list for a rotating spinner display in the CLI UI | Only declarator usage shown; exact UI component unknown. | high | 1 |
