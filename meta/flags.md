# Claude Code 2.0.72 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `auto_migrate_to_native` | gate | tools | Enables automatic CLI migration to a native updater, with analytics events emitted. | Exact migration behavior not shown; only gating and event names are visible. | medium | 1 |
| `cache_warming` | experiment | caching | Controls cache warmup behavior after idle, with interval and request limits. | Only config retrieval and early-return usage shown. | medium | 1 |
| `hide_overages_option_at_rate_limit_hit` | experiment | ui | Controls whether to show extra usage/overage option in rate-limit options menu | Affects rate-limit options list and auto-opening behavior. | high | 2 |
| `preserve_thinking` | experiment | networking | Adds a beta option for preserving model thinking in first-party requests | Ny2 meaning not shown; inferred as request beta/header token. | medium | 2 |
| `prompt_cache_1h_experiment` | experiment | caching | Enable ephemeral prompt caching with a one-hour TTL | Only affects returned cache config object. | high | 1 |
| `sonnet_1m_default` | experiment | tools | Enables default selection/display of a specific model in the CLI when accessible | Appears to gate a fallback model name when none is chosen. | high | 1 |
| `sonnet_45_1m_header` | experiment | networking | Enables adding a special 1-minute header for a specific Sonnet model variant. | Exact meaning of pushed header value is unclear from snippet. | medium | 1 |
| `tengu_ant_attribution_header_new` | gate | prompts | controls new attribution header text in a Claude Code system prompt | Flag is read but shown return path is empty/obfuscated. | medium | 1 |
| `tengu_bash_command_backgrounded` | gate | telemetry | logs/records when a shell command is backgrounded, including timeout and auto-background cases | Appears to be event logging rather than behavior gating. | medium | 1 |
| `tengu_bash_command_timeout_backgrounded` | gate | telemetry | Logs timeout events when a bash command is backgrounded | Appears to emit an event/metric, not alter behavior. | high | 1 |
| `tengu_c4w_usage_limit_notifications_enabled` | gate | ui | Controls enabling usage limit notifications, with special handling for team plans. | Only boolean gating logic is visible; notification behavior not shown. | medium | 1 |
| `tengu_compact_mc_files` | gate | filesystem | Save tool results to a file and replace content with a viewing hint. | Applies when processing user message tool_result items. | high | 1 |
| `tengu_disable_bypass_permissions_mode` | gate | safety | Disables bypass-permissions mode availability in CLI permission handling based on remote gate/settings | Used to prevent selecting bypassPermissions mode via CLI/config. | high | 3 |
| `tengu_effort_exp` | experiment | prompts | Chooses a reasoning effort level and injects a reasoning_effort prompt block. | Only seen constructing a prompt string in cli.js. | high | 1 |
| `tengu_feedback_survey_config` | config | ui | Configuration controlling when a feedback survey UI appears and closes | Also appears to emit survey events for tracking. | high | 1 |
| `tengu_file_edit_optimization` | experiment | tools | Simplifies file edit tool output to a success message instead of detailed snippet | Only affects tool_result formatting in this mapping function. | high | 1 |
| `tengu_gha_plugin_code_review` | gate | tools | Controls which GitHub Actions code review workflow template is written | Gate selects between two workflow contents (OY2 vs MY2). | high | 1 |
| `tengu_native_installation` | gate | filesystem | Controls whether CLI creates/uses native launcher script when claude.sh missing | Inference based on file checks and symlink creation logic. | medium | 1 |
| `tengu_opus_default_pro_plan` | experiment | tools | Controls whether Opus is the default model for plan subscribers | Exact effect inferred from nearby model/plan selection logic. | medium | 1 |
| `tengu_prompt_suggestion` | gate | prompts | Enable prompt suggestions setting in user preferences UI. | Gates only the settings toggle visibility. | high | 1 |
| `tengu_session_memory` | gate | caching | Enable persistent session memory and compact summaries in CLI repl. | Inferred from file read/write and repl_main_thread gating. | medium | 2 |
| `tengu_sm_compact` | gate | prompts | Enables compact summary messages for session memory handling in CLI transcript. | Only seen as combined gate check; exact behavior elsewhere unknown. | medium | 1 |
| `tengu_sm_config` | config | caching | Configure thresholds for initializing and updating session memory based on tokens and tool calls | Only shows config read and threshold fields, not how updates are applied. | medium | 1 |
| `tengu_spinner_words` | config | ui | Provides word list for a rotating spinner display in the CLI UI | Only declarator usage shown; exact UI component unknown. | high | 1 |
| `tengu_streaming_tool_execution2` | gate | tools | Gates creation of a tool-execution handler in the streaming CLI request loop | Only observed gating EV0 construction; exact behavior of EV0 is unclear. | high | 1 |
| `tengu_sumi` | gate | tools | controls CLI stream I/O configuration or console patching behavior | Only appears as a simple gate in a CLI helper. | low | 1 |
| `tengu_teams_usage_limit_notifications` | experiment | ui | Enable usage limit notifications when running in team context. | Only applies if another gate is enabled and context is "team". | medium | 1 |
| `tengu_thinkback` | gate | tools | Enables Thinkback year-in-review command and hidden animation playback tool | Controls availability of local CLI/plugin commands. | high | 2 |
| `tengu_tool_pear` | gate | tools | Enables stricter tool schema/strict mode when using specific models in CLI tool definitions | Exact behavior of OV0/Ey2 unknown from snippet. | medium | 2 |
| `tengu_tool_result_persistence` | gate | caching | Persist large tool result text by storing and replacing oversized content. | Exact persistence mechanism not shown; only size-based transformation is visible. | medium | 2 |
| `tengu_version_config` | config | ui | Checks minimum required CLI version and instructs user to update if outdated. | Used for runtime version gating and update messaging. | high | 1 |
| `tengu_vscode_review_upsell` | gate | ui | Enable VS Code review upsell experiment gate sent to connected client. | Only shows gate transmission and event logging, not the upsell UI itself. | medium | 1 |
| `tool_use_examples` | experiment | tools | Include tool input example data and enable related first-party tool option. | Applies only when enabled; one path gated to firstParty. | high | 1 |
| `trust_folder_dialog_copy` | experiment | safety | Selects copy variant for a trust-folder security prompt with continue/exit choices. | Actual variant text mapping not included. | high | 1 |
