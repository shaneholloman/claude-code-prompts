# Claude Code 1.0.119 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `auto_migrate_to_native` | gate | tools | Enables automatic CLI migration to a native updater, with analytics events emitted. | Exact migration behavior not shown; only gating and event names are visible. | medium | 1 |
| `cache_warming` | gate | caching | Controls cache warmup behavior after idle, with interval and request limits. | Only config retrieval and early-return usage shown. | medium | 1 |
| `cc_onboarding_github` | gate | ui | Controls whether to show GitHub integration onboarding step and related tip. | Seen only as a gate value used in onboarding checklist construction. | high | 1 |
| `cc_onboarding_hide_claudemd` | gate | ui | Controls whether the onboarding tip about creating CLAUDE.md is hidden | Appears to gate display of an onboarding tip. | high | 1 |
| `cc_onboarding_hide_questions_changes` | gate | ui | Controls hiding an onboarding tip about questions/changes guidance | Seen only as a variable set via mz() in onboarding UI flow. | high | 1 |
| `cc_onboarding_hide_terminal` | gate | ui | Controls whether the terminal integration onboarding tip/step is hidden in CLI onboarding | Seen only as a gate value used during onboarding list construction. | high | 1 |
| `cc_onboarding_hide_workspace` | gate | ui | Controls whether a workspace onboarding tip/step is hidden in CLI onboarding flow. | Exact UI location not shown; inferred from onboarding tip strings. | high | 1 |
| `cc_plan_mode_first_session` | gate | prompts | Automatically start first-time users in plan mode when default mode is set | Applies only on first startup and default mode. | high | 1 |
| `claude_code_unicode_sanitize` | gate | tools | Optionally sanitize Unicode in MCP tool and prompt lists before mapping results. | IL() behavior not shown; inferred as sanitization step. | high | 2 |
| `force_local_installation_migration` | gate | tools | Forces CLI migration from global npm install to local installation with restart prompt | Triggered only when additional runtime checks pass. | high | 1 |
| `max_user_opusplan` | gate | auth | Controls whether Opus-plan users get an active default model override. | Exact behavior beyond enabling override is unclear. | medium | 1 |
| `new_max_user_default_model` | gate | tools | Controls default model override selection, optionally forcing opus plan based on gating and token date. | Behavior inferred from obfuscated CLI snippet and surrounding Statsig keys. | medium | 1 |
| `tengu_auto_checkpointing` | gate | ui | Enables showing autocheckpointing availability in the config panel when not disabled by env | Only seen wired into config UI state. | medium | 1 |
| `tengu_disable_bypass_permissions_mode` | gate | safety | Disables bypass-permissions mode availability in CLI permission handling based on remote gate/settings | Used to prevent selecting bypassPermissions mode via CLI/config. | high | 2 |
| `tengu_feedback_survey_config` | config | ui | Configuration controlling when a feedback survey UI appears and closes | Also appears to emit survey events for tracking. | high | 1 |
| `tengu_native_installation` | gate | filesystem | Controls whether CLI creates/uses native launcher script when claude.sh missing | Inference based on file checks and symlink creation logic. | medium | 1 |
| `tengu_show_all_subscription_types` | gate | ui | Enable displaying all subscription types in a setup or login flow UI | Exact UI/flow unclear from limited snippet. | medium | 1 |
| `tengu_spinner_words` | config | ui | Provides word list for a rotating spinner display in the CLI UI | Only declarator usage shown; exact UI component unknown. | high | 1 |
| `tengu_use_file_checkpoints` | gate | filesystem | Enables restoring conversation or code using file-based checkpoints in message selector | Only declared here; actual conditional behavior not shown. | medium | 1 |
