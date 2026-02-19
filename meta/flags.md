# Claude Code 2.1.10 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `enhanced_telemetry_beta` | experiment | telemetry | Enables enhanced telemetry via env override, else uses remote experiment default. | Only shows gating logic; telemetry behavior not shown. | medium | 1 |
| `hide_overages_option_at_rate_limit_hit` | experiment | ui | Controls whether to show extra usage/overage option in rate-limit options menu | Affects rate-limit options list and auto-opening behavior. | high | 2 |
| `preserve_thinking` | experiment | networking | Adds a beta option for preserving model thinking in first-party requests | Ny2 meaning not shown; inferred as request beta/header token. | medium | 2 |
| `prompt_cache_1h_experiment` | experiment | caching | Enable ephemeral prompt caching with a one-hour TTL | Only affects returned cache config object. | high | 1 |
| `sonnet_1m_default` | experiment | tools | Enables default selection/display of a specific model in the CLI when accessible | Appears to gate a fallback model name when none is chosen. | high | 1 |
| `sonnet_45_1m_header` | experiment | networking | Enables adding a special 1-minute header for a specific Sonnet model variant. | Exact meaning of pushed header value is unclear from snippet. | medium | 1 |
| `tengu_ant_attribution_header_new` | gate | prompts | controls new attribution header text in a Claude Code system prompt | Flag is read but shown return path is empty/obfuscated. | medium | 1 |
| `tengu_bash_haiku_prefetch` | experiment | caching | Prefetches and reads referenced file paths after a bash command finishes. | Prefetch source of file paths depends on P42 output. | high | 1 |
| `tengu_c4w_usage_limit_notifications_enabled` | gate | ui | Controls enabling usage limit notifications, with special handling for team plans. | Only boolean gating logic is visible; notification behavior not shown. | medium | 1 |
| `tengu_chrome_auto_enable` | experiment | tools | Auto-enable Claude-in-Chrome native host integration via MCP stdio config. | Based on nearby native-host/MCP strings; exact behavior inferred. | medium | 1 |
| `tengu_code_diff_cli` | experiment | ui | Enables CLI code diff footer setting and updates git diff stats/hunks. | Also gates background git diff data refresh logic. | high | 6 |
| `tengu_compact_streaming_retry` | experiment | networking | Controls retry attempts when streaming a conversation-compaction summary request fails | Exact retry count K97 not shown. | high | 1 |
| `tengu_disable_bypass_permissions_mode` | gate | safety | Disables bypass-permissions mode availability in CLI permission handling based on remote gate/settings | Used to prevent selecting bypassPermissions mode via CLI/config. | high | 3 |
| `tengu_file_edit_optimization` | experiment | tools | Simplifies file edit tool output to a success message instead of detailed snippet | Only affects tool_result formatting in this mapping function. | high | 1 |
| `tengu_mcp_tool_search` | experiment | tools | Selects a test mode for tool search behavior in the MCP CLI. | Exact behavior of "tst" mode not shown. | medium | 1 |
| `tengu_permission_explainer` | experiment | tools | Enable permission explanation text for tool invocations in CLI. | Only one occurrence; behavior inferred from toolName/toolDescription string building. | medium | 1 |
| `tengu_pid_based_version_locking` | experiment | filesystem | Enable PID-based version locking to avoid concurrent or conflicting runs | Only PID/process check context is visible. | low | 1 |
| `tengu_plan_mode_interview_phase` | experiment | prompts | Enables an interview phase in plan mode behavior in the CLI. | Only a flag getter is shown; no downstream usage context. | medium | 1 |
| `tengu_prompt_suggestion` | gate | prompts | Enable prompt suggestions setting in user preferences UI. | Gates only the settings toggle visibility. | high | 1 |
| `tengu_scratch` | gate | filesystem | enable temporary scratchpad directory for session memory summaries | Behavior inferred from nearby path construction and conditional check. | medium | 1 |
| `tengu_session_memory` | experiment | caching | Enable persistent session memory and compact summaries in CLI repl. | Inferred from file read/write and repl_main_thread gating. | medium | 2 |
| `tengu_sm_compact` | experiment | prompts | Enables compact summary messages for session memory handling in CLI transcript. | Only seen as combined gate check; exact behavior elsewhere unknown. | medium | 1 |
| `tengu_sm_compact_config` | config | prompts | Configure compaction thresholds using token and message count limits | Only token/message limit fields are visible. | medium | 1 |
| `tengu_streaming_tool_execution2` | gate | tools | Gates creation of a tool-execution handler in the streaming CLI request loop | Only observed gating EV0 construction; exact behavior of EV0 is unclear. | high | 1 |
| `tengu_sumi` | gate | tools | controls CLI stream I/O configuration or console patching behavior | Only appears as a simple gate in a CLI helper. | low | 1 |
| `tengu_teams_usage_limit_notifications` | experiment | ui | Enable usage limit notifications when running in team context. | Only applies if another gate is enabled and context is "team". | medium | 1 |
| `tengu_thinkback` | gate | tools | Enables Thinkback year-in-review command and hidden animation playback tool | Controls availability of local CLI/plugin commands. | high | 2 |
| `tengu_tool_pear` | gate | tools | Enables stricter tool schema/strict mode when using specific models in CLI tool definitions | Exact behavior of OV0/Ey2 unknown from snippet. | medium | 2 |
| `tengu_tool_search_unsupported_models` | experiment | tools | Provides list of model substrings that disable tool search support checks | Used to filter model names by substring match. | high | 1 |
| `tengu_version_config` | config | ui | Checks minimum required CLI version and instructs user to update if outdated. | Used for runtime version gating and update messaging. | high | 1 |
| `tengu_vscode_onboarding` | gate | ui | Controls whether VSCode connected experience shows onboarding flow | Only seen declared and sent as a gate; no UI behavior shown. | medium | 1 |
| `tengu_vscode_review_upsell` | gate | ui | Enable VS Code review upsell experiment gate sent to connected client. | Only shows gate transmission and event logging, not the upsell UI itself. | medium | 1 |
| `tool_use_examples` | experiment | tools | Include tool input example data and enable related first-party tool option. | Applies only when enabled; one path gated to firstParty. | high | 1 |
| `trust_folder_dialog_copy` | experiment | safety | Selects copy variant for a trust-folder security prompt with continue/exit choices. | Actual variant text mapping not included. | high | 1 |
