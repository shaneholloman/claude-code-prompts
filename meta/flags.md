# Claude Code 2.1.71 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `tengu_1p_event_batch_config` | config | telemetry | Configures OpenTelemetry first-party event logging batch sizes, queue limits, and export interval. | Only seen in initializer; downstream usage not fully shown. | high | 1 |
| `tengu_amber_quartz` | gate | tools | Controls amber quartz behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_auto_mode_config` | config | config | Controls auto mode config behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bad_survey_transcript_ask_config` | config | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_bridge_initial_history_cap` | config | config | Controls bridge initial history cap behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_min_version` | config | tools | Enforces a minimum Claude Code version for Remote Control bridge usage. | If current version is below minVersion, Remote Control bridge usage is blocked and update guidance is shown. | high | 1 |
| `tengu_bridge_poll_interval_config` | config | config | Controls bridge poll interval config behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_ccr_bridge` | gate | tools | Enforces a minimum Claude Code version for Remote Control bridge usage. | If current version is below minVersion, Remote Control bridge usage is blocked and update guidance is shown. | medium | 1 |
| `tengu_ccr_bridge_multi_session` | gate | tools | Controls ccr bridge multi session behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_desktop_upsell` | config | config | Controls desktop upsell behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_disable_bypass_permissions_mode` | gate | safety | Disables bypass-permissions mode availability in CLI permission handling based on remote gate/settings | Used to prevent selecting bypassPermissions mode via CLI/config. | high | 3 |
| `tengu_feedback_survey_config` | config | ui | Configuration controlling when a feedback survey UI appears and closes | Also appears to emit survey events for tracking. | high | 1 |
| `tengu_good_survey_transcript_ask_config` | config | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_iron_gate_closed` | config | config | Controls iron gate closed behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_kairos_cron` | config | config | Controls kairos cron behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_kairos_cron_config` | config | config | Controls kairos cron config behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_max_version_config` | config | tools | Controls CLI minimum version enforcement and update messaging behavior | Only one occurrence; exact effect of external value unclear. | medium | 1 |
| `tengu_scratch` | gate | filesystem | enable temporary scratchpad directory for session memory summaries | Behavior inferred from nearby path construction and conditional check. | medium | 1 |
| `tengu_sm_compact_config` | config | prompts | Configure compaction thresholds using token and message count limits | Only token/message limit fields are visible. | medium | 1 |
| `tengu_sm_config` | config | caching | Configure thresholds for initializing and updating session memory based on tokens and tool calls | Only shows config read and threshold fields, not how updates are applied. | medium | 1 |
| `tengu_streaming_tool_execution2` | gate | tools | Gates creation of a tool-execution handler in the streaming CLI request loop | Only observed gating EV0 construction; exact behavior of EV0 is unclear. | high | 1 |
| `tengu_thinkback` | gate | tools | Enables Thinkback year-in-review command and hidden animation playback tool | Controls availability of local CLI/plugin commands. | high | 2 |
| `tengu_tool_pear` | gate | tools | Enables stricter tool schema/strict mode when using specific models in CLI tool definitions | Exact behavior of OV0/Ey2 unknown from snippet. | medium | 2 |
| `tengu_version_config` | config | ui | Checks minimum required CLI version and instructs user to update if outdated. | Used for runtime version gating and update messaging. | high | 1 |
| `tengu_vscode_onboarding` | gate | ui | Controls whether VSCode connected experience shows onboarding flow | Only seen declared and sent as a gate; no UI behavior shown. | medium | 1 |
| `tengu_vscode_review_upsell` | gate | ui | Enable VS Code review upsell experiment gate sent to connected client. | Only shows gate transmission and event logging, not the upsell UI itself. | medium | 1 |
