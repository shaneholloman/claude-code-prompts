# Claude Code 2.0.32 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `auto_migrate_to_native` | gate | tools | Enables automatic CLI migration to a native updater, with analytics events emitted. | Exact migration behavior not shown; only gating and event names are visible. | medium | 1 |
| `cache_warming` | experiment | caching | Controls cache warmup behavior after idle, with interval and request limits. | Only config retrieval and early-return usage shown. | medium | 1 |
| `cc_microcompact_ext` | experiment | prompts | Disable micro-compact behavior for items without assistant messages. | Only indicates gating a set; exact feature purpose unclear. | medium | 1 |
| `cc_onboarding_github` | experiment | ui | Controls whether to show GitHub integration onboarding step and related tip. | Seen only as a gate value used in onboarding checklist construction. | high | 1 |
| `cc_onboarding_hide_workspace` | experiment | ui | Controls whether a workspace onboarding tip/step is hidden in CLI onboarding flow. | Exact UI location not shown; inferred from onboarding tip strings. | high | 1 |
| `cc_onboarding_init_modal` | experiment | ui | Controls showing an initial onboarding modal on first session startup | Gated by first startup and onboarding-not-shown state. | high | 1 |
| `force_local_installation_migration` | gate | tools | Forces CLI migration from global npm install to local installation with restart prompt | Triggered only when additional runtime checks pass. | high | 1 |
| `preserve_thinking` | experiment | networking | Adds a beta option for preserving model thinking in first-party requests | Ny2 meaning not shown; inferred as request beta/header token. | medium | 1 |
| `prompt_cache_1h_experiment` | experiment | caching | Enable ephemeral prompt caching with a one-hour TTL | Only affects returned cache config object. | high | 1 |
| `sonnet_1m_default` | experiment | tools | Enables default selection/display of a specific model in the CLI when accessible | Appears to gate a fallback model name when none is chosen. | high | 1 |
| `sonnet_45_1m_header` | experiment | networking | Enables adding a special 1-minute header for a specific Sonnet model variant. | Exact meaning of pushed header value is unclear from snippet. | medium | 1 |
| `tengu_auto_checkpointing` | gate | ui | Enables showing autocheckpointing availability in the config panel when not disabled by env | Only seen wired into config UI state. | medium | 1 |
| `tengu_bash_command_backgrounded` | gate | telemetry | logs/records when a shell command is backgrounded, including timeout and auto-background cases | Appears to be event logging rather than behavior gating. | medium | 1 |
| `tengu_bash_command_timeout_backgrounded` | gate | telemetry | Logs timeout events when a bash command is backgrounded | Appears to emit an event/metric, not alter behavior. | high | 1 |
| `tengu_cap_grep_results` | experiment | tools | Limit grep tool output size via configurable cap when head_limit not provided | Appears to control default head_limit for grep results. | high | 1 |
| `tengu_disable_bypass_permissions_mode` | gate | safety | Disables bypass-permissions mode availability in CLI permission handling based on remote gate/settings | Used to prevent selecting bypassPermissions mode via CLI/config. | high | 2 |
| `tengu_feedback_survey_config` | config | ui | Configuration controlling when a feedback survey UI appears and closes | Also appears to emit survey events for tracking. | high | 1 |
| `tengu_gha_plugin_code_review` | gate | tools | Controls which GitHub Actions code review workflow template is written | Gate selects between two workflow contents (OY2 vs MY2). | high | 1 |
| `tengu_haiku_default_pro_plan` | experiment | tools | Switches default model selection to Haiku for plan users. | Exact effect depends on XY and surrounding model-selection logic. | medium | 1 |
| `tengu_migrate_ignore_patterns` | gate | filesystem | Run a migration step related to ignore patterns during startup | Exact effect of ji2() is unclear from snippet. | medium | 1 |
| `tengu_native_installation` | gate | filesystem | Controls whether CLI creates/uses native launcher script when claude.sh missing | Inference based on file checks and symlink creation logic. | medium | 1 |
| `tengu_spinner_words` | config | ui | Provides word list for a rotating spinner display in the CLI UI | Only declarator usage shown; exact UI component unknown. | high | 1 |
| `tengu_streaming_tool_execution` | gate | tools | Enables streaming-time tool execution handler during CLI request loop | Only observed gating creation of a tool execution object. | high | 1 |
| `tengu_tool_pear` | gate | tools | Enables stricter tool schema/strict mode when using specific models in CLI tool definitions | Exact behavior of OV0/Ey2 unknown from snippet. | medium | 2 |
| `trust_folder_dialog_copy` | experiment | safety | Selects copy variant for a trust-folder security prompt with continue/exit choices. | Actual variant text mapping not included. | high | 1 |
