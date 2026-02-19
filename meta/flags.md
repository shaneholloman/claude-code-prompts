# Claude Code 2.1.25 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `enhanced_telemetry_beta` | experiment | telemetry | Enables enhanced telemetry via env override, else uses remote experiment default. | Only shows gating logic; telemetry behavior not shown. | medium | 1 |
| `tengu_attribution_header` | experiment | networking | Controls whether an attribution header string is included, overridable via environment variable. | Env var can force enable/disable. | high | 1 |
| `tengu_bash_haiku_prefetch` | experiment | caching | Prefetches and reads referenced file paths after a bash command finishes. | Prefetch source of file paths depends on P42 output. | high | 1 |
| `tengu_brass_pebble` | experiment | prompts | toggles whether certain model choices/descriptions appear in the CLI selection flow | Only a boolean gate near model strings is shown. | medium | 1 |
| `tengu_c4w_usage_limit_notifications_enabled` | gate | ui | Controls enabling usage limit notifications, with special handling for team plans. | Only boolean gating logic is visible; notification behavior not shown. | medium | 1 |
| `tengu_cache_plum_violet` | experiment | caching | Skips microcompact context management that caches tool results as attachments | Exact enable/disable direction unclear. | medium | 1 |
| `tengu_chrome_auto_enable` | experiment | tools | Auto-enable Claude-in-Chrome native host integration via MCP stdio config. | Based on nearby native-host/MCP strings; exact behavior inferred. | medium | 1 |
| `tengu_code_diff_cli` | experiment | ui | Enables CLI code diff footer setting and updates git diff stats/hunks. | Also gates background git diff data refresh logic. | high | 9 |
| `tengu_compact_cache_prefix` | experiment | caching | Enable cache-sharing path for conversation compaction summaries using prefixed cache keys | Exact cache prefix behavior not shown; inferred from logs and naming. | high | 2 |
| `tengu_compact_streaming_retry` | experiment | networking | Controls retry attempts when streaming a conversation-compaction summary request fails | Exact retry count K97 not shown. | high | 1 |
| `tengu_coral_fern` | experiment | tools | Enables guidance for searching and using past session logs and memory summaries. | Gates returning a help/prompt string for session search usage. | high | 1 |
| `tengu_cork_m4q` | experiment | safety | Gates BashTool command prefix extraction safety policy prompt for injection detection. | Only declared here; downstream behavior not shown. | medium | 1 |
| `tengu_disable_bypass_permissions_mode` | gate | safety | Disables bypass-permissions mode availability in CLI permission handling based on remote gate/settings | Used to prevent selecting bypassPermissions mode via CLI/config. | high | 3 |
| `tengu_file_write_optimization` | experiment | filesystem | Simplifies file update tool output by skipping returning a cat snippet | Only affects update tool_result formatting path. | high | 1 |
| `tengu_keybinding_customization_release` | experiment | ui | Controls rollout of keybinding customization functionality | Only a simple boolean gate; behavior beyond name is unclear. | medium | 1 |
| `tengu_kv7_prompt_sort` | experiment | tools | Sorts deferred tool/skill names in generated tool prompt and logging output. | Affects ordering only; no functional tool changes shown. | high | 1 |
| `tengu_marble_anvil` | experiment | prompts | Enables adding a clear-thinking context edit and related processing in the CLI pipeline. | Exact effect of wnA/W_9 unclear beyond prompt/context handling. | high | 2 |
| `tengu_marble_kite` | experiment | tools | Controls display of file-tool guidance requiring reading before editing existing files | Appears to gate help/prompt text only. | high | 6 |
| `tengu_mcp_tool_search` | experiment | tools | Selects a test mode for tool search behavior in the MCP CLI. | Exact behavior of "tst" mode not shown. | medium | 1 |
| `tengu_permission_explainer` | experiment | tools | Enable permission explanation text for tool invocations in CLI. | Only one occurrence; behavior inferred from toolName/toolDescription string building. | medium | 1 |
| `tengu_pid_based_version_locking` | experiment | filesystem | Enable PID-based version locking to avoid concurrent or conflicting runs | Only PID/process check context is visible. | low | 1 |
| `tengu_plan_mode_interview_phase` | experiment | prompts | Enables an interview phase in plan mode behavior in the CLI. | Only a flag getter is shown; no downstream usage context. | medium | 1 |
| `tengu_plum_vx3` | experiment | tools | Force web search tool call with zero thinking tokens and alternate model selection | Exact behavior outside web_search call path unknown. | high | 1 |
| `tengu_pr_status_cli` | experiment | ui | Enables a configurable PR status footer display in the CLI UI | Also emits an event when the setting changes. | high | 2 |
| `tengu_quartz_lantern` | experiment | telemetry | Enables computing file diffs for remote edit/write operations and logs timing telemetry | Only runs for remote entrypoint; computes diff via uO1 then logs metrics. | high | 2 |
| `tengu_remote_backend` | experiment | networking | Permits starting a remote session without an initial description for the CLI remote command. | Only seen gating the missing-description error path. | high | 1 |
| `tengu_scarf_coffee` | experiment | other | Conditionally adds a capability/beta entry to a features list in CLI | Exact meaning of FiA/K entries is unclear from snippet. | medium | 1 |
| `tengu_scratch` | gate | filesystem | enable temporary scratchpad directory for session memory summaries | Behavior inferred from nearby path construction and conditional check. | medium | 1 |
| `tengu_session_memory` | experiment | caching | Enable persistent session memory and compact summaries in CLI repl. | Inferred from file read/write and repl_main_thread gating. | medium | 2 |
| `tengu_sm_compact` | experiment | prompts | Enables compact summary messages for session memory handling in CLI transcript. | Only seen as combined gate check; exact behavior elsewhere unknown. | medium | 1 |
| `tengu_sm_compact_config` | config | prompts | Configure compaction thresholds using token and message count limits | Only token/message limit fields are visible. | medium | 1 |
| `tengu_streaming_tool_execution2` | gate | tools | Gates creation of a tool-execution handler in the streaming CLI request loop | Only observed gating EV0 construction; exact behavior of EV0 is unclear. | high | 1 |
| `tengu_system_prompt_global_cache` | experiment | caching | Enables global system prompt caching marker and tool-based cache marker behavior | Gated to firstParty and can be forced via env var. | high | 3 |
| `tengu_thinkback` | gate | tools | Enables Thinkback year-in-review command and hidden animation playback tool | Controls availability of local CLI/plugin commands. | high | 2 |
| `tengu_tool_pear` | gate | tools | Enables stricter tool schema/strict mode when using specific models in CLI tool definitions | Exact behavior of OV0/Ey2 unknown from snippet. | medium | 2 |
| `tengu_tool_search_unsupported_models` | experiment | tools | Provides list of model substrings that disable tool search support checks | Used to filter model names by substring match. | high | 1 |
| `tengu_tst_kx7` | experiment | tools | Gates whether tool search is enabled when auto search is below threshold | Only seen in CLI auto tool-search flow. | high | 1 |
| `tengu_version_config` | config | ui | Checks minimum required CLI version and instructs user to update if outdated. | Used for runtime version gating and update messaging. | high | 1 |
| `tengu_vscode_onboarding` | gate | ui | Controls whether VSCode connected experience shows onboarding flow | Only seen declared and sent as a gate; no UI behavior shown. | medium | 1 |
| `tengu_vscode_review_upsell` | gate | ui | Enable VS Code review upsell experiment gate sent to connected client. | Only shows gate transmission and event logging, not the upsell UI itself. | medium | 1 |
| `tengu_workout` | experiment | prompts | Enable higher-effort mode unless disabled by environment variable. | Exact behavior beyond gating effort is unclear. | medium | 1 |
