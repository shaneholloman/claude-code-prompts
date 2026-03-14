# Claude Code 2.1.76 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `tengu_1p_event_batch_config` | config | telemetry | Configures OpenTelemetry first-party event logging batch sizes, queue limits, and export interval. | Only seen in initializer; downstream usage not fully shown. | high | 2 |
| `tengu_auto_mode_config` | config | tools | Controls CLI auto mode enablement and circuit-breaker disabling via async config check |  | high | 1 |
| `tengu_bad_survey_transcript_ask_config` | config | prompts | Config for prompting transcript sharing after a negative feedback survey response |  | high | 1 |
| `tengu_bridge_initial_history_cap` | config | networking | Limits number of prior chat messages initially flushed over REPL bridge transport | Applies during initial connect flush in onWorkReceived. | high | 1 |
| `tengu_bridge_min_version` | config | tools | Minimum required version for Remote Control bridge; blocks feature when CLI version too old. | Appears to gate Remote Control/bridge based on a configured minVersion. | high | 1 |
| `tengu_bridge_poll_interval_config` | config | networking | Configures polling interval timing for a bridge component when not at capacity | Exact bridge behavior not shown; inferred from poll interval schema. | medium | 1 |
| `tengu_ccr_bridge` | gate | tools | Enables a CLI bridge component with async/blocking checks and minimum version validation. | Exact bridge behavior isn’t shown beyond enable checks and min-version logic. | medium | 1 |
| `tengu_ccr_bridge_multi_session` | gate | tools | Controls whether the CLI bridge supports multiple concurrent spawned sessions. | Only a gate return is shown; exact behavior beyond session spawning is unclear. | medium | 1 |
| `tengu_chair_sermon` | gate | ui | Enables an alternate transformation/normalization path for attachments when building the chat message list. | Exact visual/formatting outcome is unclear due to obfuscated helper functions (i3z, n3z, o3z). | medium | 3 |
| `tengu_desktop_upsell` | config | ui | Controls desktop startup upsell dialog on supported OS/architecture | Exact upsell content/behavior beyond startup dialog not shown. | high | 1 |
| `tengu_disable_bypass_permissions_mode` | gate | safety | Disables bypass-permissions mode availability in CLI permission handling based on remote gate/settings | Used to prevent selecting bypassPermissions mode via CLI/config. | high | 3 |
| `tengu_feedback_survey_config` | config | ui | Configuration controlling when a feedback survey UI appears and closes | Also appears to emit survey events for tracking. | high | 1 |
| `tengu_good_survey_transcript_ask_config` | config | prompts | Configuration for asking to share transcript after a positive feedback survey. |  | high | 1 |
| `tengu_iron_gate_closed` | config | safety | Fail-closed when auto-mode classifier is unavailable, denying actions with retry guidance. | Controls deny vs fail-open behavior on classifier unavailability. | high | 1 |
| `tengu_kairos_brief` | config | ui | Enables a user-visible “brief” message (markdown-supported), configurable via flag or CLAUDE_CODE_BRIEF. | Context suggests a displayed message, but the exact UI surface/location isn’t shown in the snippet. | medium | 1 |
| `tengu_kairos_cron` | config | tools | Enables session-scoped cron scheduling tools to run prompts later. | Only one return-site occurrence; exact behavior behind gate not shown. | medium | 1 |
| `tengu_kairos_cron_config` | config | other | Cron jitter configuration for recurring task scheduling parameters. | Only shows parsing/validation; actual use of config not included. | medium | 1 |
| `tengu_max_version_config` | config | tools | Defines a minimum allowed app version; updates below it are skipped and may show an external message. |  | medium | 1 |
| `tengu_scratch` | gate | filesystem | enable temporary scratchpad directory for session memory summaries | Behavior inferred from nearby path construction and conditional check. | medium | 1 |
| `tengu_sm_compact_config` | config | prompts | Configure compaction thresholds using token and message count limits | Only token/message limit fields are visible. | medium | 1 |
| `tengu_sm_config` | config | caching | Configure thresholds for initializing and updating session memory based on tokens and tool calls | Only shows config read and threshold fields, not how updates are applied. | medium | 1 |
| `tengu_streaming_tool_execution2` | gate | tools | Gates creation of a tool-execution handler in the streaming CLI request loop | Only observed gating EV0 construction; exact behavior of EV0 is unclear. | high | 1 |
| `tengu_thinkback` | gate | tools | Enables Thinkback year-in-review command and hidden animation playback tool | Controls availability of local CLI/plugin commands. | high | 2 |
| `tengu_tool_pear` | gate | tools | Enables stricter tool schema/strict mode when using specific models in CLI tool definitions | Exact behavior of OV0/Ey2 unknown from snippet. | medium | 2 |
| `tengu_toolref_defer_j8m` | gate | tools | Toggles whether an extra tool-reference text block is injected into message content. | Exact text/prefix (JWq) is obfuscated; behavior inferred from conditional content insertion and list transform. | medium | 2 |
| `tengu_version_config` | config | ui | Checks minimum required CLI version and instructs user to update if outdated. | Used for runtime version gating and update messaging. | high | 1 |
| `tengu_vscode_onboarding` | gate | ui | Controls whether VSCode connected experience shows onboarding flow | Only seen declared and sent as a gate; no UI behavior shown. | medium | 1 |
| `tengu_vscode_review_upsell` | gate | ui | Enable VS Code review upsell experiment gate sent to connected client. | Only shows gate transmission and event logging, not the upsell UI itself. | medium | 1 |
