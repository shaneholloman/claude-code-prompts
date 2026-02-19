# Claude Code 2.0.63 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `auto_migrate_to_native` | gate | tools | Enables automatic CLI migration to a native updater, with analytics events emitted. | Exact migration behavior not shown; only gating and event names are visible. | medium | 1 |
| `cache_warming` | experiment | caching | Controls cache warmup behavior after idle, with interval and request limits. | Only config retrieval and early-return usage shown. | medium | 1 |
| `cc_microcompact_ext` | experiment | prompts | Disable micro-compact behavior for items without assistant messages. | Only indicates gating a set; exact feature purpose unclear. | medium | 1 |
| `claude_code_overages_upgrade_cta` | experiment | ui | Controls CLI overage upgrade call-to-action variant and interactive options menu behavior | Only seen in CLI React component logic. | high | 1 |
| `code_slack_app_install_banner` | gate | tools | Enables Slack app installation tip and local command to open marketplace link |  | high | 2 |
| `preserve_thinking` | experiment | networking | Adds a beta option for preserving model thinking in first-party requests | Ny2 meaning not shown; inferred as request beta/header token. | medium | 2 |
| `prompt_cache_1h_experiment` | experiment | caching | Enable ephemeral prompt caching with a one-hour TTL | Only affects returned cache config object. | high | 1 |
| `sonnet_1m_default` | experiment | tools | Enables default selection/display of a specific model in the CLI when accessible | Appears to gate a fallback model name when none is chosen. | high | 1 |
| `sonnet_45_1m_header` | experiment | networking | Enables adding a special 1-minute header for a specific Sonnet model variant. | Exact meaning of pushed header value is unclear from snippet. | medium | 1 |
| `tengu_bash_command_backgrounded` | gate | telemetry | logs/records when a shell command is backgrounded, including timeout and auto-background cases | Appears to be event logging rather than behavior gating. | medium | 1 |
| `tengu_bash_command_timeout_backgrounded` | gate | telemetry | Logs timeout events when a bash command is backgrounded | Appears to emit an event/metric, not alter behavior. | high | 1 |
| `tengu_cap_grep_results` | experiment | tools | Limit grep tool output size via configurable cap when head_limit not provided | Appears to control default head_limit for grep results. | high | 1 |
| `tengu_compact_mc_files` | gate | filesystem | Save tool results to a file and replace content with a viewing hint. | Applies when processing user message tool_result items. | high | 1 |
| `tengu_deep_ocean_current` | experiment | prompts | Enable always-thinking mode for specific Claude models in CLI | Only affects Opus path; Sonnet forced on. | high | 1 |
| `tengu_disable_bypass_permissions_mode` | gate | safety | Disables bypass-permissions mode availability in CLI permission handling based on remote gate/settings | Used to prevent selecting bypassPermissions mode via CLI/config. | high | 3 |
| `tengu_effort_exp` | experiment | prompts | Chooses a reasoning effort level and injects a reasoning_effort prompt block. | Only seen constructing a prompt string in cli.js. | high | 1 |
| `tengu_feedback_survey_config` | config | ui | Configuration controlling when a feedback survey UI appears and closes | Also appears to emit survey events for tracking. | high | 1 |
| `tengu_file_edit_optimization` | experiment | tools | Simplifies file edit tool output to a success message instead of detailed snippet | Only affects tool_result formatting in this mapping function. | high | 1 |
| `tengu_gha_plugin_code_review` | gate | tools | Controls which GitHub Actions code review workflow template is written | Gate selects between two workflow contents (OY2 vs MY2). | high | 1 |
| `tengu_log_1p_events` | gate | telemetry | Enables emitting first-party telemetry events with IDs and session/user attributes. | Also gated by EV(), K0(), and GB0 availability. | medium | 1 |
| `tengu_native_installation` | gate | filesystem | Controls whether CLI creates/uses native launcher script when claude.sh missing | Inference based on file checks and symlink creation logic. | medium | 1 |
| `tengu_opus_default_pro_plan` | experiment | tools | Controls whether Opus is the default model for plan subscribers | Exact effect inferred from nearby model/plan selection logic. | medium | 1 |
| `tengu_session_memory` | gate | caching | Enable persistent session memory and compact summaries in CLI repl. | Inferred from file read/write and repl_main_thread gating. | medium | 2 |
| `tengu_sm_compact` | gate | prompts | Enables compact summary messages for session memory handling in CLI transcript. | Only seen as combined gate check; exact behavior elsewhere unknown. | medium | 1 |
| `tengu_spinner_words` | config | ui | Provides word list for a rotating spinner display in the CLI UI | Only declarator usage shown; exact UI component unknown. | high | 1 |
| `tengu_streaming_tool_execution2` | gate | tools | Gates creation of a tool-execution handler in the streaming CLI request loop | Only observed gating EV0 construction; exact behavior of EV0 is unclear. | high | 1 |
| `tengu_sumi` | gate | tools | controls CLI stream I/O configuration or console patching behavior | Only appears as a simple gate in a CLI helper. | low | 1 |
| `tengu_tool_pear` | gate | tools | Enables stricter tool schema/strict mode when using specific models in CLI tool definitions | Exact behavior of OV0/Ey2 unknown from snippet. | medium | 2 |
| `tengu_tool_result_persistence` | gate | caching | Persist large tool result text by storing and replacing oversized content. | Exact persistence mechanism not shown; only size-based transformation is visible. | medium | 2 |
| `tengu_vscode_review_upsell` | gate | ui | Enable VS Code review upsell experiment gate sent to connected client. | Only shows gate transmission and event logging, not the upsell UI itself. | medium | 1 |
| `tengu_web_tasks` | gate | ui | Enables background command mode using an '&' prefix in CLI input parsing. | Only observed gating of '&' background mode parsing. | high | 7 |
| `tool_use_examples` | experiment | tools | Include tool input example data and enable related first-party tool option. | Applies only when enabled; one path gated to firstParty. | high | 1 |
| `trust_folder_dialog_copy` | experiment | safety | Selects copy variant for a trust-folder security prompt with continue/exit choices. | Actual variant text mapping not included. | high | 1 |
