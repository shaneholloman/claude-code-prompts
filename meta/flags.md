# Claude Code 2.1.80 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `action_after_hooks` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `action_after_input_prompt` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `action_after_plugins_init` | gate | safety | Controls whether bypass-permissions mode can be used. | Can disable bypass mode via gate/config and show warnings when bypass is requested. | high | 2 |
| `action_after_setup` | gate | tools | Controls action after setup behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `action_before_setup` | gate | tools | Controls action before setup behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `action_commands_loaded` | gate | tools | Controls action commands loaded behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `action_handler_start` | gate | tools | Controls action handler start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `action_mcp_configs_loaded` | gate | tools | Controls action mcp configs loaded behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `action_tools_loaded` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `agent_mentions` | gate | tools | Controls agent mentions behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `agent_pending_messages` | gate | tools | Controls agent pending messages behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `all_proxy` | gate | tools | Controls all proxy behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `allow_product_feedback` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 3 |
| `allow_remote_control` | gate | tools | Controls allow remote control behavior. | Heuristic inference from non-LLM flag context. | high | 4 |
| `allow_remote_sessions` | gate | tools | Controls allow remote sessions behavior. | Heuristic inference from non-LLM flag context. | high | 5 |
| `ant_model_override` | gate | filesystem | Controls temporary scratch/session-memory filesystem behavior. | Inference based on scratch/session-memory naming and context. | high | 1 |
| `api_request` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `api_request_sent` | gate | tools | Controls api request sent behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `async_hook_responses` | gate | tools | Controls async hook responses behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `at_mentioned_files` | gate | tools | Controls at mentioned files behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `auto` | gate | safety | Controls whether bypass-permissions mode can be used. | Can disable bypass mode via gate/config and show warnings when bypass is requested. | high | 4 |
| `auto_migrate_to_native` | gate | tools | Enables automatic CLI migration to a native updater, with analytics events emitted. | Exact migration behavior not shown; only gating and event names are visible. | medium | 1 |
| `auto_mode` | gate | tools | Controls auto mode behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `auto_mode_exit` | gate | tools | Controls auto mode exit behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `autocomplete` | gate | tools | Controls autocomplete behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `aws_security_credentials_supplier` | gate | tools | Controls aws security credentials supplier behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `budget_usd` | gate | tools | Controls budget usd behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `built_in` | gate | tools | Controls built in behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `cache_cold` | gate | tools | Controls cache cold behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `call_after_close` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | low | 1 |
| `changed_files` | gate | tools | Controls changed files behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `checking_out` | gate | tools | Controls checking out behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `child_process` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 7 |
| `claude` | gate | tools | Controls claude behavior. | Heuristic inference from non-LLM flag context. | high | 6 |
| `cli_after_main_complete` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `cli_after_main_import` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `cli_before_main_import` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `cli_bridge_path` | gate | tools | Enforces a minimum Claude Code version for Remote Control bridge usage. | If current version is below minVersion, Remote Control bridge usage is blocked and update guidance is shown. | high | 1 |
| `cli_chrome_native_host_path` | gate | tools | Controls cli chrome native host path behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `cli_claude_in_chrome_mcp_path` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `cli_entry` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `cli_tmux_worktree_fast_path` | gate | tools | Controls cli tmux worktree fast path behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `client_id` | gate | tools | Controls client id behavior. | Heuristic inference from non-LLM flag context. | high | 5 |
| `client_secret` | gate | tools | Controls client secret behavior. | Heuristic inference from non-LLM flag context. | high | 4 |
| `close_tab` | gate | tools | Controls close tab behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `cloud_resource_manager_url` | gate | tools | Controls cloud resource manager url behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `code` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | high | 6 |
| `code_challenge` | gate | tools | Controls code challenge behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `code_challenge_method` | gate | tools | Controls code challenge method behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `codesign` | gate | tools | Controls codesign behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `coral_reef_sonnet` | gate | tools | Controls coral reef sonnet behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `credential_source` | gate | tools | Controls credential source behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `critical_system_reminder` | gate | tools | Controls critical system reminder behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `date_change` | gate | tools | Controls date change behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `deferred_tools_delta` | gate | tools | Controls deferred tools delta behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `delivery_failure` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | medium | 1 |
| `delivery_retry` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | medium | 1 |
| `dispatch_start` | gate | tools | Controls dispatch start behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `dynamic_skill` | gate | tools | Controls dynamic skill behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `early_conversation` | gate | tools | Controls early conversation behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `enhanced_telemetry_beta` | experiment | telemetry | Enables enhanced telemetry via env override, else uses remote experiment default. | Only shows gating logic; telemetry behavior not shown. | medium | 1 |
| `env_info_simple` | gate | filesystem | Controls temporary scratch/session-memory filesystem behavior. | Inference based on scratch/session-memory naming and context. | high | 1 |
| `environment_id` | gate | tools | Controls environment id behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `error_description` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `feedback_survey` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 5 |
| `feedback_survey_bad` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | medium | 2 |
| `field_mask` | gate | tools | Controls field mask behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `file_path` | gate | tools | Controls file path behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `first_chunk` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 2 |
| `from_sequence_num` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `headless_managed_settings_wait` | gate | tools | Controls headless managed settings wait behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `headless_marketplace_reconcile` | gate | tools | Controls headless marketplace reconcile behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `hook_execution_complete` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `hook_execution_start` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `http_request` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `ide_opened_file` | gate | tools | Controls ide opened file behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `ide_selection` | gate | tools | Controls ide selection behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `imdsv2_session_token_url` | gate | tools | Controls imdsv2 session token url behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `in_process_teammate` | gate | tools | Controls in process teammate behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `init_after_1p_event_logging` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `init_after_graceful_shutdown` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `init_after_jetbrains_detection` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `init_after_oauth_populate` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `init_after_remote_settings_check` | gate | filesystem | Controls temporary scratch/session-memory filesystem behavior. | Inference based on scratch/session-memory naming and context. | high | 1 |
| `init_configs_enabled` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `init_function_end` | gate | filesystem | Controls temporary scratch/session-memory filesystem behavior. | Inference based on scratch/session-memory naming and context. | high | 1 |
| `init_function_start` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `init_network_configured` | gate | filesystem | Controls temporary scratch/session-memory filesystem behavior. | Inference based on scratch/session-memory naming and context. | high | 1 |
| `init_safe_env_vars_applied` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `limit_increase` | gate | tools | Controls limit increase behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `llm_request` | gate | tools | Controls llm request behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `local_bash` | gate | tools | Controls local bash behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `lsp_diagnostics` | gate | tools | Controls lsp diagnostics behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `main_after_run` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 2 |
| `main_before_run` | gate | tools | Controls main before run behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `main_client_type_determined` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | high | 1 |
| `main_function_start` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | high | 1 |
| `main_tsx_entry` | gate | tools | Controls main tsx entry behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `main_tsx_imports_loaded` | gate | tools | Controls main tsx imports loaded behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `main_warning_handler_initialized` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | high | 1 |
| `max_age` | gate | tools | Controls max age behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `mcp_instructions` | gate | filesystem | Controls temporary scratch/session-memory filesystem behavior. | Inference based on scratch/session-memory naming and context. | high | 1 |
| `mcp_instructions_delta` | gate | tools | Controls mcp instructions delta behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `mcp_resources` | gate | tools | Controls mcp resources behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `mdm_load_end` | gate | tools | Controls mdm load end behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `mdm_load_start` | gate | tools | Controls mdm load start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `message_delivered` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | medium | 1 |
| `message_enriched` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | medium | 2 |
| `nested_memory` | gate | tools | Controls nested memory behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `no_proxy` | gate | tools | Controls no proxy behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `notebook_path` | gate | tools | Controls notebook path behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `npm_config_no_proxy` | gate | tools | Controls npm config no proxy behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `npm_config_proxy` | gate | tools | Controls npm config proxy behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `output_style` | gate | filesystem | Controls temporary scratch/session-memory filesystem behavior. | Inference based on scratch/session-memory naming and context. | high | 2 |
| `output_token_usage` | gate | tools | Controls output token usage behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `perf_hooks` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 4 |
| `plan_approval` | gate | tools | Controls plan approval behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `plan_mode` | gate | tools | Controls plan mode behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `plan_mode_exit` | gate | tools | Controls plan mode exit behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `plugin_time` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | medium | 1 |
| `profiler_initialized` | gate | tools | Controls profiler initialized behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `project_id` | gate | tools | Controls project id behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `prompts` | gate | tools | Controls prompts behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_api_loop_start` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_api_request_sent` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 2 |
| `query_api_streaming_end` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_api_streaming_start` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_attachment_loading_end` | gate | tools | Controls query attachment loading end behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_attachment_loading_start` | gate | tools | Controls query attachment loading start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_autocompact_end` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_autocompact_start` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_client_creation_end` | gate | tools | Controls query client creation end behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `query_client_creation_start` | gate | tools | Controls query client creation start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_context_loading_end` | gate | tools | Controls query context loading end behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `query_context_loading_start` | gate | tools | Controls query context loading start behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `query_end` | gate | tools | Controls query end behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_file_history_snapshot_end` | gate | tools | Controls query file history snapshot end behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `query_file_history_snapshot_start` | gate | tools | Controls query file history snapshot start behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `query_first_chunk_received` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_fn_entry` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_hooks_end` | gate | tools | Controls query hooks end behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_hooks_start` | gate | tools | Controls query hooks start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_image_processing_end` | gate | tools | Controls query image processing end behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_image_processing_start` | gate | tools | Controls query image processing start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_message_normalization_end` | gate | tools | Controls query message normalization end behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_message_normalization_start` | gate | tools | Controls query message normalization start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_microcompact_end` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_microcompact_start` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_pasted_image_processing_end` | gate | tools | Controls query pasted image processing end behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_pasted_image_processing_start` | gate | tools | Controls query pasted image processing start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_process_user_input_base_end` | gate | tools | Controls query process user input base end behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_process_user_input_base_start` | gate | tools | Controls query process user input base start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_process_user_input_end` | gate | tools | Controls query process user input end behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `query_process_user_input_start` | gate | tools | Controls query process user input start behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `query_profile_end` | gate | tools | Controls query profile end behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `query_query_start` | gate | tools | Controls query query start behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `query_recursive_call` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_response_headers_received` | gate | tools | Controls query response headers received behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `query_setup_end` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_setup_start` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_tool_execution_end` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_tool_execution_start` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `query_tool_schema_build_end` | gate | tools | Controls query tool schema build end behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_tool_schema_build_start` | gate | tools | Controls query tool schema build start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `query_user_input_received` | gate | tools | Controls query user input received behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `queued_commands` | gate | tools | Controls queued commands behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `quota_project_id` | gate | tools | Controls quota project id behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `redirect_uri` | gate | tools | Controls redirect uri behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `region_url` | gate | tools | Controls region url behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `regional_cred_verification_url` | gate | tools | Controls regional cred verification url behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `requires_action` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | medium | 1 |
| `resource_link` | gate | tools | Controls resource link behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `response_type` | gate | tools | Controls response type behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `run_after_parse` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `run_before_parse` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `run_commander_initialized` | gate | tools | Controls run commander initialized behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `run_function_start` | gate | tools | Controls run function start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `sdk_no_params` | gate | tools | Controls sdk no params behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `server_max_window_bits` | gate | tools | Controls server max window bits behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `server_no_context_takeover` | gate | tools | Controls server no context takeover behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `service_account_impersonation` | gate | tools | Controls service account impersonation behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `service_account_impersonation_url` | gate | tools | Controls service account impersonation url behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `session_start` | gate | tools | Controls session start behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `set_permission_mode` | gate | safety | Controls whether bypass-permissions mode can be used. | Can disable bypass mode via gate/config and show warnings when bypass is requested. | medium | 1 |
| `setup_after_prefetch` | gate | safety | Controls whether bypass-permissions mode can be used. | Can disable bypass mode via gate/config and show warnings when bypass is requested. | high | 1 |
| `setup_before_prefetch` | gate | safety | Controls whether bypass-permissions mode can be used. | Can disable bypass mode via gate/config and show warnings when bypass is requested. | high | 1 |
| `skill_listing` | gate | tools | Controls skill listing behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `skip_rendering` | gate | tools | Controls skip rendering behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `string_decoder` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `stt_provider` | gate | tools | Controls stt provider behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `subject_token_field_name` | gate | tools | Controls subject token field name behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `subject_token_supplier` | gate | tools | Controls subject token supplier behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `subject_token_type` | gate | tools | Controls subject token type behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `summarize_tool_results` | gate | filesystem | Controls temporary scratch/session-memory filesystem behavior. | Inference based on scratch/session-memory naming and context. | high | 1 |
| `system_message_yielded` | gate | tools | Controls system message yielded behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `system_prompt` | gate | tools | Controls system prompt behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `team_context` | gate | tools | Controls team context behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `teammate_mailbox` | gate | tools | Controls teammate mailbox behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `telemetry_init_start` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_1p_event_batch_config` | config | telemetry | Configures batching (delay, batch size, queue size) for exporting first‑party event logs. | Falls back to OTEL_LOGS_EXPORT_INTERVAL and defaults when fields are missing; triggers flush/reinit on config change. | high | 2 |
| `tengu_accept_feedback_mode_collapsed` | gate | tools | Controls accept feedback mode collapsed behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_accept_feedback_mode_entered` | gate | tools | Controls accept feedback mode entered behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_accept_submitted` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 3 |
| `tengu_agent_color_set` | gate | tools | Controls agent color set behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_agent_created` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_agent_definition_generated` | gate | tools | Controls agent definition generated behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_agent_flag` | gate | tools | Controls agent flag behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_agent_memory_loaded` | gate | tools | Controls agent memory loaded behavior. | Heuristic inference from non-LLM flag context. | high | 4 |
| `tengu_agent_name_set` | gate | tools | Controls agent name set behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_agent_stop_hook_max_turns` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_agent_tool_selected` | gate | tools | Controls agent tool selected behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_agent_tool_terminated` | gate | tools | Controls agent tool terminated behavior. | Heuristic inference from non-LLM flag context. | high | 4 |
| `tengu_agentic_search_cancelled` | gate | tools | Controls agentic search cancelled behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_amber_flint` | gate | tools | Controls amber flint behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_amber_prism` | gate | tools | Controls amber prism behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_amber_quartz_disabled` | gate | tools | Controls amber quartz disabled behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_amber_wren` | gate | tools | Controls amber wren behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_api_after_normalize` | gate | tools | Controls api after normalize behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_api_before_normalize` | gate | tools | Controls api before normalize behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_api_cache_breakpoints` | gate | tools | Controls api cache breakpoints behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_api_key_saved_to_config` | gate | tools | Controls api key saved to config behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_api_key_saved_to_keychain` | gate | tools | Controls api key saved to keychain behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_api_opus_fallback_triggered` | gate | tools | Controls api opus fallback triggered behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_api_persistent_retry_wait` | gate | tools | Controls api persistent retry wait behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_api_query` | gate | tools | Controls api query behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_api_retry` | gate | tools | Controls api retry behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_ask_user_question_finish_plan_interview` | gate | tools | Controls ask user question finish plan interview behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_ask_user_question_rejected` | gate | tools | Controls ask user question rejected behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_ask_user_question_respond_to_claude` | gate | tools | Controls ask user question respond to claude behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_at_mention_agent_not_found` | gate | tools | Controls at mention agent not found behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_attachment_compute_duration` | gate | tools | Controls attachment compute duration behavior. | Heuristic inference from non-LLM flag context. | medium | 2 |
| `tengu_attachment_file_too_large` | gate | tools | Controls attachment file too large behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_attachments` | gate | tools | Controls attachments behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_attribution_header` | experiment | networking | Controls whether an attribution header string is included, overridable via environment variable. | Env var can force enable/disable. | high | 1 |
| `tengu_auto_background_agents` | gate | tools | Controls auto background agents behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_auto_compact_succeeded` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_auto_dream_fired` | gate | tools | Controls auto dream fired behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_auto_migrate_to_native_attempt` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_auto_migrate_to_native_failure` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_auto_migrate_to_native_partial` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_auto_mode_config` | config | ui | Gates “auto mode” availability, with circuit-breaker disable plus model and org allowlist checks. | Also respects user settings (disableAutoMode) and can disable fast mode. | high | 6 |
| `tengu_auto_mode_decision` | gate | tools | Controls auto mode decision behavior. | Heuristic inference from non-LLM flag context. | high | 4 |
| `tengu_auto_mode_denial_limit_exceeded` | gate | tools | Controls auto mode denial limit exceeded behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_auto_mode_malformed_tool_input` | gate | tools | Controls auto mode malformed tool input behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_auto_mode_opt_in_dialog_accept` | gate | tools | Controls auto mode opt in dialog accept behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_auto_mode_opt_in_dialog_accept_default` | gate | tools | Controls auto mode opt in dialog accept default behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_auto_mode_opt_in_dialog_decline` | gate | tools | Controls auto mode opt in dialog decline behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_auto_mode_outcome` | gate | tools | Controls auto mode outcome behavior. | Heuristic inference from non-LLM flag context. | high | 12 |
| `tengu_auto_updater_fail` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_auto_updater_lock_contention` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_auto_updater_windows_npm_in_wsl` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_autoupdate_enabled` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | medium | 1 |
| `tengu_bad_survey_transcript_ask_config` | config | prompts | Config for whether a “bad” feedback survey asks to include the conversation transcript. | Bundle is obfuscated; exact UI text/conditions aren’t visible, only survey+transcript request wiring. | medium | 1 |
| `tengu_basalt_3kr` | gate | tools | Controls basalt 3kr behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_bash_ast_too_complex` | gate | tools | Controls bash ast too complex behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bash_command_explicitly_backgrounded` | gate | tools | Controls bash command explicitly backgrounded behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_bash_command_timeout_backgrounded` | gate | telemetry | Logs timeout events when a bash command is backgrounded | Appears to emit an event/metric, not alter behavior. | high | 1 |
| `tengu_bash_security_check_triggered` | gate | tools | Controls bash security check triggered behavior. | Heuristic inference from non-LLM flag context. | high | 42 |
| `tengu_bash_tool_reset_to_original_dir` | gate | tools | Controls bash tool reset to original dir behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_bash_tool_simple_echo` | gate | tools | Controls bash tool simple echo behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_began_setup` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | low | 1 |
| `tengu_binary_content_persisted` | gate | tools | Controls binary content persisted behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_binary_download_attempt` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_binary_download_failure` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_binary_manifest_fetch_failure` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_binary_platform_not_found` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_bramble_lintel` | gate | tools | Controls bramble lintel behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_command` | gate | tools | Controls bridge command behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_bridge_heartbeat_mode_entered` | gate | tools | Controls bridge heartbeat mode entered behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_bridge_heartbeat_mode_exited` | gate | tools | Controls bridge heartbeat mode exited behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_bridge_initial_history_cap` | config | tools | Caps how much prior message history is considered when starting a bridge REPL session. | Only the config read (default 200, max 300000) is visible; exact unit/behavior of the cap isn’t shown. | medium | 1 |
| `tengu_bridge_message_received` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 2 |
| `tengu_bridge_min_version` | config | tools | Blocks Remote Control when Claude Code is below a configured minimum version. |  | high | 1 |
| `tengu_bridge_multi_session_denied` | gate | tools | Controls bridge multi session denied behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_poll_give_up` | gate | tools | Controls bridge poll give up behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_bridge_poll_interval_config` | config | networking | Sets Tengu bridge poll interval (0 disables) plus session reclaim and keepalive timings. | Config is schema-validated; invalid values fall back to defaults. | medium | 1 |
| `tengu_bridge_reconnected` | gate | tools | Controls bridge reconnected behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_repl_connect_timeout` | gate | tools | Controls bridge repl connect timeout behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_bridge_repl_env_expired_fresh_session` | gate | tools | Controls bridge repl env expired fresh session behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_repl_env_lost` | gate | tools | Controls bridge repl env lost behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_repl_env_registered` | gate | tools | Controls bridge repl env registered behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_repl_history_capped` | gate | tools | Controls bridge repl history capped behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_repl_poll_give_up` | gate | tools | Controls bridge repl poll give up behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_repl_reconnected_in_place` | gate | tools | Controls bridge repl reconnected in place behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_repl_skipped` | gate | tools | Controls bridge repl skipped behavior. | Heuristic inference from non-LLM flag context. | high | 11 |
| `tengu_bridge_repl_suspension_detected` | gate | tools | Controls bridge repl suspension detected behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_repl_teardown` | gate | tools | Controls bridge repl teardown behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_bridge_repl_v2` | gate | tools | Enforces a minimum Claude Code version for Remote Control bridge usage. | If current version is below minVersion, Remote Control bridge usage is blocked and update guidance is shown. | medium | 1 |
| `tengu_bridge_repl_v2_config` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | medium | 1 |
| `tengu_bridge_repl_work_received` | gate | tools | Controls bridge repl work received behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_repl_ws_closed` | gate | tools | Controls bridge repl ws closed behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_bridge_repl_ws_connected` | gate | tools | Controls bridge repl ws connected behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_bridge_session_done` | gate | tools | Controls bridge session done behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_session_timeout` | gate | tools | Controls bridge session timeout behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_bridge_shutdown` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_bridge_spawn_mode_chosen` | gate | tools | Controls bridge spawn mode chosen behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bridge_system_init` | gate | tools | Controls bridge system init behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_bridge_token_refreshed` | gate | tools | Controls bridge token refreshed behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_brief_send` | gate | tools | Controls brief send behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_bug_report_description` | gate | tools | Controls bug report description behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_bug_report_submitted` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_bypass_permissions_mode_dialog_accept` | gate | tools | Controls bypass permissions mode dialog accept behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_cache_eviction_hint` | gate | tools | Controls cache eviction hint behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_cancel` | gate | tools | Controls cancel behavior. | Heuristic inference from non-LLM flag context. | high | 4 |
| `tengu_ccr_bridge` | gate | tools | Enables the Tengu CCR bridge for Claude Code, with an optional minimum bridge version check. | Only gate checks and a min-version config are visible; what the bridge does beyond enabling is not shown. | medium | 2 |
| `tengu_ccr_bridge_multi_session` | gate | tools | Toggles multi-session spawning behavior for a Tengu CCR bridge process. | Only spawn/session-related code is visible; the exact behavioral differences when enabled are not shown. | medium | 1 |
| `tengu_ccr_bundle_max_bytes` | gate | tools | Controls whether CCR bundle seeding is enabled. | Inference based on the flag name and CCR bundle naming pattern. | high | 1 |
| `tengu_ccr_bundle_seed_enabled` | gate | tools | Enables CCR git-bundle seeding fallback for remote/teleport sessions. | When enabled (or CCR_ENABLE_BUNDLE is set), a source bundle can be uploaded and passed as seed_bundle_file_id. | high | 1 |
| `tengu_ccr_bundle_upload` | gate | tools | Controls ccr bundle upload behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_ccr_unsupported_default_mode_ignored` | gate | safety | Controls whether bypass-permissions mode can be used. | Can disable bypass mode via gate/config and show warnings when bypass is requested. | high | 1 |
| `tengu_chain_parallel_tr_recovered` | gate | tools | Controls chain parallel tr recovered behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_chain_parent_cycle` | gate | tools | Controls chain parent cycle behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_chair_sermon` | gate | tools | Applies extra processing to attachment messages before they’re merged/added to the chat history. | Obfuscated helpers (K$_, nVq, O$_) hide exact transformation details. | medium | 4 |
| `tengu_chomp_inflection` | gate | tools | Controls chomp inflection behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_chrome_auto_enable` | experiment | tools | Auto-enable Claude-in-Chrome native host integration via MCP stdio config. | Based on nearby native-host/MCP strings; exact behavior inferred. | medium | 1 |
| `tengu_cicada_nap_ms` | gate | tools | Controls cicada nap ms behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_claude_in_chrome_setup` | gate | tools | Controls claude in chrome setup behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_claude_install_command` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_claudeai_mcp_eligibility` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 4 |
| `tengu_claudeai_mcp_reconnect` | gate | tools | Controls claudeai mcp reconnect behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_claudeai_mcp_toggle` | gate | tools | Controls claudeai mcp toggle behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_claudemd__initial_load` | gate | tools | Controls claudemd  initial load behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_cobalt_frost` | gate | tools | Controls cobalt frost behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_cobalt_lantern` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 4 |
| `tengu_code_indexing_tool_used` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 2 |
| `tengu_code_prompt_ignored` | gate | tools | Controls code prompt ignored behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_collage_kaleidoscope` | gate | tools | Controls collage kaleidoscope behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_compact` | gate | tools | Controls compact behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_compact_cache_prefix` | experiment | caching | Enable cache-sharing path for conversation compaction summaries using prefixed cache keys | Exact cache prefix behavior not shown; inferred from logs and naming. | high | 2 |
| `tengu_compact_cache_sharing_fallback` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 2 |
| `tengu_compact_streaming_retry` | experiment | networking | Controls retry attempts when streaming a conversation-compaction summary request fails | Exact retry count K97 not shown. | high | 2 |
| `tengu_concurrent_onquery_detected` | gate | tools | Controls concurrent onquery detected behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_concurrent_onquery_enqueued` | gate | tools | Controls concurrent onquery enqueued behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_concurrent_sessions` | gate | tools | Controls concurrent sessions behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_config_auth_loss_prevented` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 3 |
| `tengu_config_cache_stats` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | medium | 1 |
| `tengu_config_lock_contention` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_config_stale_write` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_context_size` | gate | tools | Controls context size behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_context_window_exceeded` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_continue` | gate | tools | Controls continue behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_continue_print` | gate | tools | Controls continue print behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_conversation_forked` | gate | tools | Controls conversation forked behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_conversation_rewind` | gate | tools | Controls conversation rewind behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_copper_bridge` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | medium | 1 |
| `tengu_copy` | gate | tools | Controls copy behavior. | Heuristic inference from non-LLM flag context. | high | 4 |
| `tengu_coral_fern` | experiment | tools | Enables guidance for searching and using past session logs and memory summaries. | Gates returning a help/prompt string for session search usage. | high | 1 |
| `tengu_cork_m4q` | experiment | safety | Gates BashTool command prefix extraction safety policy prompt for injection detection. | Only declared here; downstream behavior not shown. | medium | 1 |
| `tengu_cost_threshold_acknowledged` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | medium | 1 |
| `tengu_cost_threshold_reached` | gate | tools | Controls cost threshold reached behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_custom_keybindings_loaded` | gate | tools | Controls custom keybindings loaded behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_defer_all_bn4` | gate | tools | Controls defer all bn4 behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_deferred_tool_schema_not_sent` | gate | tools | Controls deferred tool schema not sent behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_deferred_tools_pool_change` | gate | tools | Controls deferred tools pool change behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_desktop_upsell` | config | prompts | Enables a startup dialog upsell for a desktop app on macOS or Windows x64. | Gate appears limited to darwin/win32 x64 and checks an enable_startup_dialog setting. | medium | 1 |
| `tengu_destructive_command_warning` | gate | tools | Controls destructive command warning behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_dir_search` | gate | tools | Controls dir search behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_disable_bypass_permissions_mode` | gate | safety | Blocks use of "bypassPermissions" mode (even if requested) due to gate/org policy. | Also checks a session/org setting (permissions.disableBypassPermissionsMode) alongside the gate. | high | 4 |
| `tengu_disable_streaming_to_non_streaming_fallback` | gate | tools | Controls disable streaming to non streaming fallback behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_doctor_command` | gate | tools | Controls doctor command behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_effort_command` | gate | tools | Controls effort command behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_exit` | gate | safety | Controls whether bypass-permissions mode can be used. | Can disable bypass mode via gate/config and show warnings when bypass is requested. | high | 1 |
| `tengu_exit_plan_mode_called_outside_plan` | gate | tools | Controls exit plan mode called outside plan behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_ext_at_mentioned` | gate | tools | Controls ext at mentioned behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_ext_diff_rejected` | gate | tools | Controls ext diff rejected behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_ext_ide_command` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | high | 1 |
| `tengu_ext_installed` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | medium | 1 |
| `tengu_ext_will_show_diff` | gate | tools | Controls ext will show diff behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_external_editor_used` | gate | tools | Controls external editor used behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_extract_memories_coalesced` | gate | tools | Controls extract memories coalesced behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_extract_memories_extraction` | gate | tools | Controls extract memories extraction behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_extract_memories_skipped_direct_write` | gate | tools | Controls extract memories skipped direct write behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_fast_mode_fallback_triggered` | gate | tools | Controls fast mode fallback triggered behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_fast_mode_overage_rejected` | gate | tools | Controls fast mode overage rejected behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_feedback_survey_config` | config | prompts | Settings for displaying a feedback survey and recording appeared/responded outcomes (good/bad). | Context shows error handling and fallback IDs like "unknown" when config/session data is missing. | medium | 1 |
| `tengu_feedback_survey_event` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 6 |
| `tengu_fgts` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_file_history_backup_deleted_file` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_file_history_backup_file_created` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | medium | 1 |
| `tengu_file_operation` | gate | tools | Controls file operation behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_file_read_limits_override` | gate | tools | Controls file read limits override behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_file_suggestions_git_ls_files` | gate | tools | Controls file suggestions git ls files behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_file_suggestions_query` | gate | tools | Controls file suggestions query behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_file_suggestions_ripgrep` | gate | tools | Controls file suggestions ripgrep behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_filtered_orphaned_thinking_message` | gate | tools | Controls filtered orphaned thinking message behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_filtered_trailing_thinking_block` | gate | tools | Controls filtered trailing thinking block behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_filtered_whitespace_only_assistant` | gate | tools | Controls filtered whitespace only assistant behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_fixed_empty_assistant_content` | gate | tools | Controls fixed empty assistant content behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_flicker` | gate | tools | Controls flicker behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_fork_agent_query` | gate | tools | Controls fork agent query behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_git_operation` | gate | tools | Controls git operation behavior. | Heuristic inference from non-LLM flag context. | high | 6 |
| `tengu_glacier_2xr` | gate | tools | Controls glacier 2xr behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_good_survey_transcript_ask_config` | config | ui | Config for asking to include/share transcript when a “good” feedback survey is shown. | Only seen alongside feedback survey configs/events; exact prompt text/logic isn’t visible here. | medium | 1 |
| `tengu_granite_whisper` | gate | tools | Controls granite whisper behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_grey_step2` | gate | tools | Controls grey step2 behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_grey_wool` | gate | tools | Controls grey wool behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_grove_oauth_401_received` | gate | tools | Controls grove oauth 401 received behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_grove_policy_dismissed` | gate | tools | Controls grove policy dismissed behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_grove_policy_escaped` | gate | tools | Controls grove policy escaped behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_grove_policy_exited` | gate | safety | Controls whether bypass-permissions mode can be used. | Can disable bypass mode via gate/config and show warnings when bypass is requested. | medium | 1 |
| `tengu_grove_policy_submitted` | gate | tools | Controls grove policy submitted behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_grove_policy_viewed` | gate | tools | Controls grove policy viewed behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_grove_print_viewed` | gate | tools | Controls grove print viewed behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_grove_privacy_settings_viewed` | gate | tools | Controls grove privacy settings viewed behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_guest_passes_link_copied` | gate | tools | Controls guest passes link copied behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_guest_passes_visited` | gate | tools | Controls guest passes visited behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_harbor` | gate | tools | Controls harbor behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_harbor_ledger` | gate | tools | Controls harbor ledger behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_hawthorn_steeple` | gate | tools | Controls hawthorn steeple behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_hawthorn_window` | gate | tools | Controls hawthorn window behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_headless_latency` | gate | tools | Controls headless latency behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_headless_plugin_install` | gate | tools | Controls headless plugin install behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_heap_dump` | gate | tools | Controls heap dump behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_herring_clock` | gate | tools | Controls herring clock behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_hooks_command` | gate | tools | Controls hooks command behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_image_resize_fallback` | gate | tools | Controls image resize fallback behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_immediate_model_command` | gate | tools | Controls immediate model command behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_init` | gate | tools | Controls init behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_input_bash` | gate | tools | Controls input bash behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_input_command` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 2 |
| `tengu_input_prompt` | gate | tools | Controls input prompt behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_input_slash_invalid` | gate | tools | Controls input slash invalid behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_input_slash_missing` | gate | tools | Controls input slash missing behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_iron_gate_closed` | config | safety | Chooses fail-closed denial when auto-mode classifier is unavailable instead of falling back to normal permission handling. | Flag toggles deny-with-retry guidance (fail closed) vs fail-open fallback when classifier is unavailable. | high | 1 |
| `tengu_kairos_brief` | config | prompts | Enables a “brief” user message/tool (markdown) when entitled or CLAUDE_CODE_BRIEF is set. | Gated by an entitlement check plus another condition (By()\|\|kZ()). | medium | 3 |
| `tengu_kairos_brief_config` | gate | tools | Controls kairos brief config behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_kairos_cron` | config | tools | Enables session-only cron tools to schedule prompts to run later or on a recurring schedule. | Disabled when CLAUDE_CODE_DISABLE_CRON is set. | high | 1 |
| `tengu_kairos_cron_config` | config | tools | Configures cron scheduling jitter/recurrence limits for a background job runner. | Only schema and accessor names are visible; the specific jobs affected aren’t shown. | medium | 1 |
| `tengu_keybinding_customization_release` | experiment | ui | Controls rollout of keybinding customization functionality | Only a simple boolean gate; behavior beyond name is unclear. | medium | 1 |
| `tengu_keybinding_fallback_used` | gate | tools | Controls keybinding fallback used behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_lean_cast` | gate | tools | Controls lean cast behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_legacy_opus_migration` | gate | tools | Controls legacy opus migration behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_login_from_refresh_token` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | high | 1 |
| `tengu_managed_settings_loaded` | gate | tools | Controls managed settings loaded behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_managed_settings_security_dialog_rejected` | gate | tools | Controls managed settings security dialog rejected behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_marble_anvil` | experiment | prompts | Enables adding a clear-thinking context edit and related processing in the CLI pipeline. | Exact effect of wnA/W_9 unclear beyond prompt/context handling. | high | 2 |
| `tengu_marble_sandcastle` | gate | tools | Controls marble sandcastle behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_marketplace_added` | gate | tools | Controls marketplace added behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_marketplace_background_install` | gate | tools | Controls marketplace background install behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_marketplace_removed` | gate | tools | Controls marketplace removed behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_marketplace_updated` | gate | tools | Controls marketplace updated behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_marketplace_updated_all` | gate | tools | Controls marketplace updated all behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_max_tokens_context_overflow_adjustment` | gate | tools | Controls max tokens context overflow adjustment behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_max_tokens_reached` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_max_version_config` | config | tools | Minimum-version config used to block applying an update when the target version is too old. | Config also exposes optional `external` and `external_message` fields, likely for update messaging. | medium | 1 |
| `tengu_mcp_add` | gate | tools | Controls mcp add behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_mcp_auth_config_authenticate` | gate | tools | Controls mcp auth config authenticate behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_mcp_auth_config_clear` | gate | tools | Controls mcp auth config clear behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_mcp_claudeai_proxy_401` | gate | tools | Controls mcp claudeai proxy 401 behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_mcp_delete` | gate | tools | Controls mcp delete behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_mcp_dialog_choice` | gate | tools | Controls mcp dialog choice behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_mcp_elicitation` | gate | tools | Controls mcp elicitation behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_mcp_elicitation_response` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 4 |
| `tengu_mcp_get` | gate | tools | Controls mcp get behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_mcp_ide_server_connection_succeeded` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_mcp_instructions_pool_change` | gate | tools | Controls mcp instructions pool change behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_mcp_list` | gate | tools | Controls mcp list behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_mcp_multidialog_choice` | gate | tools | Controls mcp multidialog choice behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_mcp_oauth_flow_start` | gate | tools | Controls mcp oauth flow start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_mcp_reset_mcpjson_choices` | gate | tools | Controls mcp reset mcpjson choices behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_mcp_server_connection_succeeded` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_mcp_server_needs_auth` | gate | tools | Controls mcp server needs auth behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_mcp_servers` | gate | tools | Controls mcp servers behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_mcp_session_expired` | gate | tools | Controls mcp session expired behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_mcp_start` | gate | tools | Controls mcp start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_mcp_tools_commands_loaded` | gate | tools | Controls mcp tools commands loaded behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_memdir_accessed` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_memdir_disabled` | gate | tools | Controls memdir disabled behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_memdir_file_edit` | gate | tools | Controls memdir file edit behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_memdir_file_read` | gate | tools | Controls memdir file read behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_memdir_file_write` | gate | tools | Controls memdir file write behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_memdir_loaded` | gate | tools | Controls memdir loaded behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_message_level_tool_result_budget_enforced` | gate | tools | Controls message level tool result budget enforced behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_message_selector_cancelled` | gate | tools | Controls message selector cancelled behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_message_selector_opened` | gate | tools | Controls message selector opened behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_message_selector_restore_option_selected` | gate | tools | Controls message selector restore option selected behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_message_selector_selected` | gate | tools | Controls message selector selected behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_migrate_autoupdates_to_settings` | gate | tools | Controls migrate autoupdates to settings behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_migrate_reset_auto_opt_in_for_default_offer` | gate | tools | Controls migrate reset auto opt in for default offer behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_miraculo_the_bard` | gate | tools | Controls miraculo the bard behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_miraculo_the_bard2` | gate | tools | Controls miraculo the bard2 behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_mode_cycle` | gate | tools | Controls mode cycle behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_model_command_inline` | gate | tools | Controls model command inline behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_model_command_inline_help` | gate | tools | Controls model command inline help behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_model_command_menu` | gate | tools | Controls model command menu behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_model_command_menu_effort` | gate | tools | Controls model command menu effort behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_model_fallback_triggered` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_model_picker_hotkey` | gate | tools | Controls model picker hotkey behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_model_whitespace_response` | gate | tools | Controls model whitespace response behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_moth_copse` | gate | tools | Controls moth copse behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_native_auto_updater_fail` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_native_auto_updater_lock_contention` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_native_auto_updater_start` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_native_auto_updater_up_to_date` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_native_install_binary_failure` | gate | tools | Controls native install binary failure behavior. | Heuristic inference from non-LLM flag context. | medium | 2 |
| `tengu_native_install_package_failure` | gate | tools | Controls native install package failure behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_native_staging_cleanup` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_native_stale_locks_cleanup` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_native_temp_files_cleanup` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_native_update_complete` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 2 |
| `tengu_native_update_skipped_max_version` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_native_update_skipped_minimum_version` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_native_version_cleanup` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 2 |
| `tengu_node_warning` | gate | tools | Controls node warning behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_notification_method_used` | gate | tools | Controls notification method used behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_oauth_401_recovered_from_keychain` | gate | tools | Controls oauth 401 recovered from keychain behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_oauth_api_key` | gate | tools | Controls oauth api key behavior. | Heuristic inference from non-LLM flag context. | medium | 2 |
| `tengu_oauth_auth_code_received` | gate | tools | Controls oauth auth code received behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_oauth_automatic_redirect` | gate | tools | Controls oauth automatic redirect behavior. | Heuristic inference from non-LLM flag context. | low | 2 |
| `tengu_oauth_claudeai_forced` | gate | tools | Controls oauth claudeai forced behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_oauth_claudeai_selected` | gate | tools | Controls oauth claudeai selected behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_console_forced` | gate | tools | Controls oauth console forced behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_console_selected` | gate | tools | Controls oauth console selected behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_flow_start` | gate | tools | Controls oauth flow start behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_oauth_manual_entry` | gate | tools | Controls oauth manual entry behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_oauth_platform_selected` | gate | tools | Controls oauth platform selected behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_roles_stored` | gate | tools | Controls oauth roles stored behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_oauth_storage_warning` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | medium | 1 |
| `tengu_oauth_token_refresh_failure` | gate | tools | Controls oauth token refresh failure behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_token_refresh_lock_acquired` | gate | tools | Controls oauth token refresh lock acquired behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_token_refresh_lock_acquiring` | gate | tools | Controls oauth token refresh lock acquiring behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_token_refresh_lock_released` | gate | tools | Controls oauth token refresh lock released behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_token_refresh_lock_releasing` | gate | tools | Controls oauth token refresh lock releasing behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_token_refresh_lock_retry` | gate | tools | Controls oauth token refresh lock retry behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_token_refresh_lock_retry_limit_reached` | gate | tools | Controls oauth token refresh lock retry limit reached behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_token_refresh_race_recovered` | gate | tools | Controls oauth token refresh race recovered behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_token_refresh_race_resolved` | gate | tools | Controls oauth token refresh race resolved behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_token_refresh_starting` | gate | tools | Controls oauth token refresh starting behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_oauth_tokens_inference_only` | gate | tools | Controls oauth tokens inference only behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_oauth_tokens_not_claude_ai` | gate | tools | Controls oauth tokens not claude ai behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_oauth_tokens_save_exception` | gate | tools | Controls oauth tokens save exception behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_oauth_tokens_saved` | gate | tools | Controls oauth tokens saved behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_off_switch_query` | gate | tools | Controls off switch query behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_official_marketplace_auto_install` | gate | tools | Controls official marketplace auto install behavior. | Heuristic inference from non-LLM flag context. | high | 6 |
| `tengu_onboarding_step` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | medium | 1 |
| `tengu_onyx_plover` | gate | tools | Controls onyx plover behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_opus_to_opus1m_migration` | gate | tools | Controls opus to opus1m migration behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_orphaned_messages_tombstoned` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_paper_halyard` | gate | tools | Controls paper halyard behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_partial_compact` | gate | tools | Controls partial compact behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_passport_quail` | gate | tools | Controls passport quail behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_paste_image` | gate | tools | Controls paste image behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_paste_text` | gate | tools | Controls paste text behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_pasted_image_resize_attempt` | gate | tools | Controls pasted image resize attempt behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_pdf_page_extraction` | gate | tools | Controls pdf page extraction behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_pdf_reference_attachment` | gate | tools | Controls pdf reference attachment behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_pebble_leaf_prune` | gate | tools | Controls pebble leaf prune behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_penguins_off` | gate | tools | Controls penguins off behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_permission_explainer` | experiment | tools | Enable permission explanation text for tool invocations in CLI. | Only one occurrence; behavior inferred from toolName/toolDescription string building. | medium | 1 |
| `tengu_permission_explainer_generated` | gate | tools | Controls permission explainer generated behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_permission_explainer_shortcut_used` | gate | tools | Controls permission explainer shortcut used behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_permission_request_escape` | gate | tools | Controls permission request escape behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_permission_request_option_selected` | gate | tools | Controls permission request option selected behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_pewter_ledger` | gate | tools | Controls pewter ledger behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_pid_based_version_locking` | experiment | filesystem | Enable PID-based version locking to avoid concurrent or conflicting runs | Only PID/process check context is visible. | low | 1 |
| `tengu_plan_enter` | gate | tools | Controls plan enter behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_plan_exit` | gate | safety | Controls whether bypass-permissions mode can be used. | Can disable bypass mode via gate/config and show warnings when bypass is requested. | high | 9 |
| `tengu_plan_external_editor_used` | gate | tools | Controls plan external editor used behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_plan_mode_interview_phase` | experiment | prompts | Enables an interview phase in plan mode behavior in the CLI. | Only a flag getter is shown; no downstream usage context. | medium | 1 |
| `tengu_plugin_disable_command` | gate | tools | Controls plugin disable command behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_plugin_disabled_all_cli` | gate | tools | Controls plugin disabled all cli behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_plugin_disabled_cli` | gate | tools | Controls plugin disabled cli behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_plugin_enable_command` | gate | tools | Controls plugin enable command behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_plugin_enabled_cli` | gate | tools | Controls plugin enabled cli behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_plugin_install_command` | gate | tools | Controls plugin install command behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_plugin_installed` | gate | tools | Controls plugin installed behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_plugin_installed_cli` | gate | tools | Controls plugin installed cli behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_plugin_list_command` | gate | tools | Controls plugin list command behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_plugin_uninstall_command` | gate | tools | Controls plugin uninstall command behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_plugin_uninstalled_cli` | gate | tools | Controls plugin uninstalled cli behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_plugin_update_command` | gate | tools | Controls plugin update command behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_plugin_updated_cli` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_plugins_loaded` | gate | tools | Controls plugins loaded behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_plum_vx3` | experiment | tools | Force web search tool call with zero thinking tokens and alternate model selection | Exact behavior outside web_search call path unknown. | high | 1 |
| `tengu_post_autocompact_turn` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_post_compact_survey_event` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | medium | 2 |
| `tengu_post_tool_failure_hooks_cancelled` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_post_tool_hooks_cancelled` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_pr_status_cli` | experiment | ui | Enables a configurable PR status footer display in the CLI UI | Also emits an event when the setting changes. | high | 2 |
| `tengu_pre_stop_hooks_cancelled` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_pre_tool_hooks_cancelled` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_prompt_cache_1h_config` | gate | tools | Controls prompt cache 1h config behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_prompt_suggestion` | gate | prompts | Enable prompt suggestions setting in user preferences UI. | Gates only the settings toggle visibility. | high | 3 |
| `tengu_prompt_suggestion_init` | gate | tools | Controls prompt suggestion init behavior. | Heuristic inference from non-LLM flag context. | high | 6 |
| `tengu_quartz_lantern` | experiment | telemetry | Enables computing file diffs for remote edit/write operations and logs timing telemetry | Only runs for remote entrypoint; computes diff via uO1 then logs metrics. | high | 2 |
| `tengu_query_after_attachments` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_query_before_attachments` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_quiet_fern` | experiment | ui | Enables an experimental VS Code extension UI/flow controlled via experiment gates. | Only appears in gates payload; no direct behavior shown. | medium | 1 |
| `tengu_quiet_hollow` | gate | tools | Controls quiet hollow behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_rate_limit_options_menu_cancel` | gate | tools | Controls rate limit options menu cancel behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_rate_limit_options_menu_select_extra_usage` | gate | tools | Controls rate limit options menu select extra usage behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_rate_limit_options_menu_select_upgrade` | gate | tools | Controls rate limit options menu select upgrade behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_refusal_api_response` | gate | tools | Controls refusal api response behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_reject_feedback_mode_collapsed` | gate | tools | Controls reject feedback mode collapsed behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_reject_feedback_mode_entered` | gate | tools | Controls reject feedback mode entered behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_reject_submitted` | gate | tools | Controls reject submitted behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_remote_backend` | experiment | networking | Permits starting a remote session without an initial description for the CLI remote command. | Only seen gating the missing-description error path. | high | 1 |
| `tengu_remote_create_session` | gate | tools | Controls remote create session behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_remote_setup_result` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | high | 5 |
| `tengu_repl_hook_finished` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_repo_text_file_size` | gate | tools | Controls repo text file size behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_reset_pro_to_opus_default` | gate | tools | Controls reset pro to opus default behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_resume_print` | gate | tools | Controls resume print behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_ripgrep_availability` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_ripgrep_eagain_retry` | gate | tools | Controls ripgrep eagain retry behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_run_hook` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 2 |
| `tengu_scarf_coffee` | experiment | other | Conditionally adds a capability/beta entry to a features list in CLI | Exact meaning of FiA/K entries is unclear from snippet. | medium | 1 |
| `tengu_scheduled_task_expired` | gate | tools | Controls scheduled task expired behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_scheduled_task_fire` | gate | tools | Controls scheduled task fire behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_scheduled_task_missed` | gate | tools | Controls scheduled task missed behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_scratch` | gate | filesystem | Enables writing a session-memory scratchpad with a summary.md file under a per-user Claude folder. |  | high | 1 |
| `tengu_sepia_heron` | gate | tools | Controls sepia heron behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_sepia_heron_applied` | gate | tools | Controls sepia heron applied behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_session_file_read` | gate | tools | Controls session file read behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_session_forked_branches_fetched` | gate | tools | Controls session forked branches fetched behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_session_group_expanded` | gate | tools | Controls session group expanded behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_session_linked_to_pr` | gate | tools | Controls session linked to pr behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_session_memory` | experiment | caching | Enable persistent session memory and compact summaries in CLI repl. | Inferred from file read/write and repl_main_thread gating. | medium | 2 |
| `tengu_session_memory_accessed` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_session_memory_extraction` | gate | tools | Controls session memory extraction behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_session_memory_file_read` | gate | tools | Controls session memory file read behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_session_memory_loaded` | gate | tools | Controls session memory loaded behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_session_preview_opened` | gate | tools | Controls session preview opened behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_session_renamed` | gate | tools | Controls session renamed behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_session_resumed` | gate | tools | Controls session resumed behavior. | Heuristic inference from non-LLM flag context. | high | 7 |
| `tengu_session_tagged` | gate | tools | Controls session tagged behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_session_title_generated` | gate | tools | Controls session title generated behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_setup_token_command` | gate | tools | Controls setup token command behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_shell_set_cwd` | gate | tools | Controls shell set cwd behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_single_word_prompt` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_skill_improvement_survey` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 2 |
| `tengu_skill_loaded` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | medium | 1 |
| `tengu_skill_tool_invocation` | gate | tools | Controls skill tool invocation behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_skill_tool_slash_prefix` | gate | tools | Controls skill tool slash prefix behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_slash_command_forked` | gate | tools | Controls slash command forked behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_slate_prism` | gate | tools | Controls slate prism behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_sm_compact` | experiment | prompts | Enables compact summary messages for session memory handling in CLI transcript. | Only seen as combined gate check; exact behavior elsewhere unknown. | medium | 1 |
| `tengu_sm_compact_config` | config | caching | Configures thresholds for compacting content using min/max token limits and minimum text-block messages. | Snippet only shows loading/merging these limits into a shared config object, not the compaction routine. | medium | 1 |
| `tengu_sm_compact_empty_template` | gate | tools | Controls sm compact empty template behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_sm_compact_no_session_memory` | gate | tools | Controls sm compact no session memory behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_sm_compact_resumed_session` | gate | tools | Controls sm compact resumed session behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_sm_compact_summarized_id_not_found` | gate | tools | Controls sm compact summarized id not found behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_sm_compact_threshold_exceeded` | gate | tools | Controls sm compact threshold exceeded behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_sm_config` | config | tools | Loads a config object likely related to Tengu “session memory” behavior. | Context only shows config retrieval; no direct fields or effects are visible here. | low | 1 |
| `tengu_sonnet45_to_46_migration` | gate | tools | Controls sonnet45 to 46 migration behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_speculation` | gate | tools | Controls speculation behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_startup_manual_model_config` | gate | tools | Controls startup manual model config behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_startup_perf` | gate | tools | Controls startup perf behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_startup_telemetry` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | medium | 1 |
| `tengu_status_line_mount` | gate | tools | Controls status line mount behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_stdin_interactive` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | medium | 1 |
| `tengu_stream_loop_exited_after_watchdog` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 2 |
| `tengu_stream_no_events` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_streaming_fallback_to_non_streaming` | gate | tools | Controls streaming fallback to non streaming behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_streaming_idle_timeout` | gate | tools | Controls streaming idle timeout behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_streaming_stall` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_streaming_stall_summary` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_streaming_tool_execution2` | gate | tools | Enables streaming tool execution during a session. | Observed only as a session gate named "streamingToolExecution"; exact runtime behavior not shown. | medium | 1 |
| `tengu_streaming_tool_execution_not_used` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_streaming_tool_execution_used` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_structured_output_enabled` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_structured_output_failure` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_subagent_at_mention` | gate | tools | Controls subagent at mention behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_surreal_dali` | gate | tools | Controls surreal dali behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_swinburne_dune` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 3 |
| `tengu_sync_plugin_install_timeout` | gate | tools | Gates streaming tool-execution behavior in the CLI request loop. | Exact internal execution-path behavior is inferred from usage context. | high | 1 |
| `tengu_sysprompt_block` | gate | tools | Controls sysprompt block behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_sysprompt_boundary_found` | gate | tools | Controls sysprompt boundary found behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_sysprompt_missing_boundary_marker` | gate | tools | Controls sysprompt missing boundary marker behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_sysprompt_using_tool_based_cache` | gate | tools | Controls sysprompt using tool based cache behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_system_prompt_global_cache` | experiment | caching | Enables global system prompt caching marker and tool-based cache marker behavior | Gated to firstParty and can be forced via env var. | high | 3 |
| `tengu_tag_command_add` | gate | tools | Controls tag command add behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tag_command_remove_cancelled` | gate | tools | Controls tag command remove cancelled behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tag_command_remove_confirmed` | gate | tools | Controls tag command remove confirmed behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tag_command_remove_prompt` | gate | tools | Controls tag command remove prompt behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_team_created` | gate | tools | Controls team created behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_team_deleted` | gate | tools | Controls team deleted behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_team_mem_accessed` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_team_mem_entries_capped` | gate | tools | Controls team mem entries capped behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_team_mem_file_edit` | gate | tools | Controls team mem file edit behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_team_mem_file_read` | gate | tools | Controls team mem file read behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_team_mem_file_write` | gate | tools | Controls team mem file write behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_team_mem_push_suppressed` | gate | tools | Controls team mem push suppressed behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_team_mem_secret_skipped` | gate | tools | Controls team mem secret skipped behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_team_mem_sync_pull` | gate | tools | Controls team mem sync pull behavior. | Heuristic inference from non-LLM flag context. | high | 6 |
| `tengu_team_mem_sync_push` | gate | tools | Controls team mem sync push behavior. | Heuristic inference from non-LLM flag context. | high | 8 |
| `tengu_team_memdir_disabled` | gate | tools | Controls team memdir disabled behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_teleport_bundle_mode` | gate | tools | Controls teleport bundle mode behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_teleport_cancelled` | gate | tools | Controls teleport cancelled behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_teleport_error_git_not_clean` | gate | tools | Controls teleport error git not clean behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_teleport_error_repo_mismatch_sessions_api` | gate | tools | Controls teleport error repo mismatch sessions api behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_teleport_error_repo_not_in_git_dir_sessions_api` | gate | tools | Controls teleport error repo not in git dir sessions api behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_teleport_error_session_not_found_404` | gate | tools | Controls teleport error session not found 404 behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_teleport_errors_detected` | gate | tools | Controls teleport errors detected behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_teleport_errors_resolved` | gate | tools | Controls teleport errors resolved behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_teleport_interactive_mode` | gate | tools | Controls teleport interactive mode behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_teleport_print` | gate | tools | Controls teleport print behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_teleport_resume_session` | gate | tools | Controls teleport resume session behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_teleport_source_decision` | gate | tools | Controls teleport source decision behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_thinkback` | gate | tools | Enables local 'think-back' 2025 year-in-review and the hidden thinkback animation player. |  | high | 2 |
| `tengu_thinking_toggled_hotkey` | gate | tools | Controls thinking toggled hotkey behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tide_elm` | gate | tools | Controls tide elm behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_tight_weave` | gate | tools | Controls tight weave behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_timer` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | medium | 1 |
| `tengu_toggle_todos` | gate | tools | Controls toggle todos behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_toggle_transcript` | gate | tools | Controls toggle transcript behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tool_empty_result` | gate | tools | Controls tool empty result behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tool_input_alias_applied` | gate | tools | Controls tool input alias applied behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tool_input_aliasing` | gate | tools | Controls tool input aliasing behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tool_pear` | gate | tools | Enables additional tool-definition handling for strict tools, including extra processing for supported models. | Exact effect is obfuscated; observable uses include adding a feature to the tool context list and gating a crypto hash path. | medium | 2 |
| `tengu_tool_result_pairing_repaired` | gate | tools | Controls tool result pairing repaired behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_tool_result_persisted` | gate | tools | Controls tool result persisted behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tool_result_persisted_message_budget` | gate | tools | Controls tool result persisted message budget behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_tool_search_mode_decision` | gate | tools | Controls tool search mode decision behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tool_search_outcome` | gate | tools | Controls tool search outcome behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tool_search_unsupported_models` | experiment | tools | Provides list of model substrings that disable tool search support checks | Used to filter model names by substring match. | high | 1 |
| `tengu_tool_use_can_use_tool_allowed` | gate | tools | Controls tool use can use tool allowed behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_tool_use_can_use_tool_rejected` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_tool_use_cancelled` | gate | tools | Controls tool use cancelled behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_tool_use_denied_in_config` | gate | tools | Controls tool use denied in config behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tool_use_diff_computed` | gate | tools | Controls tool use diff computed behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_tool_use_granted_by_classifier` | gate | tools | Controls tool use granted by classifier behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_tool_use_granted_by_permission_hook` | gate | tools | Controls tool use granted by permission hook behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_tool_use_granted_in_config` | gate | tools | Controls tool use granted in config behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_tool_use_progress` | gate | tools | Controls tool use progress behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tool_use_rejected_in_prompt` | gate | tools | Controls tool use rejected in prompt behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tool_use_show_permission_request` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | low | 1 |
| `tengu_toolref_defer_j8m` | gate | tools | Alters how tool-use messages are preprocessed, including injecting/deferring a tool-reference text block. | Exact text marker (gVq) and transform (Y$_) are obfuscated, so behavior is inferred from message-content edits. | medium | 2 |
| `tengu_trace_lantern` | gate | tools | Controls trace lantern behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_transcript_accessed` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 1 |
| `tengu_transcript_exit` | gate | tools | Controls transcript exit behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_transcript_input_to_teammate` | gate | tools | Controls transcript input to teammate behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_transcript_parent_cycle` | gate | tools | Controls transcript parent cycle behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_transcript_toggle_show_all` | gate | tools | Controls transcript toggle show all behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_transcript_view_enter` | gate | tools | Controls transcript view enter behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_transcript_view_exit` | gate | tools | Controls transcript view exit behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tree_sitter_security_divergence` | gate | tools | Controls tree sitter security divergence behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_trust_dialog_accept` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | low | 1 |
| `tengu_tst_hint_m7r` | gate | tools | Controls tst hint m7r behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_tst_kx7` | experiment | tools | Gates whether tool search is enabled when auto search is below threshold | Only seen in CLI auto tool-search flow. | high | 1 |
| `tengu_turtle_carbon` | gate | tools | Controls turtle carbon behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_ultrathink` | gate | tools | Controls ultrathink behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_unary_event` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | medium | 1 |
| `tengu_uncaught_exception` | gate | tools | Controls uncaught exception behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_unexpected_tool_result` | gate | tools | Controls unexpected tool result behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_unhandled_rejection` | gate | tools | Controls unhandled rejection behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_unknown_model_cost` | gate | tools | Controls unknown model cost behavior. | Heuristic inference from non-LLM flag context. | low | 1 |
| `tengu_update_check` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_version_check_failure` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tengu_version_config` | config | tools | Fetches a minimum required Claude Code version and shows an update-required message. | Minimum version appears server-configured via the config fetch. | high | 1 |
| `tengu_version_lock_acquired` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 4 |
| `tengu_voice_stream_early_retry` | gate | tools | Controls voice stream early retry behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_vscode_cc_auth` | gate | ui | Controls VS Code onboarding experience behavior. | Inference is based on gate name and surrounding VS Code context. | high | 1 |
| `tengu_vscode_onboarding` | gate | ui | Enables an onboarding experience/flow in the Claude VSCode integration. | Only seen being sent as an experiment gate; specific onboarding screens/steps aren’t shown. | medium | 1 |
| `tengu_vscode_review_upsell` | gate | prompts | Enables a review upsell prompt/flow in the Claude VS Code integration. | Inferred mainly from the flag name; the surrounding code shows VS Code integration wiring and experiment gates. | medium | 1 |
| `tengu_worktree_cleanup` | gate | tools | Controls worktree cleanup behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tengu_worktree_created` | gate | tools | Controls worktree created behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_worktree_detection` | gate | tools | Controls worktree detection behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_worktree_kept` | gate | tools | Controls worktree kept behavior. | Heuristic inference from non-LLM flag context. | high | 3 |
| `tengu_worktree_removed` | gate | tools | Controls worktree removed behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_write_claudemd` | gate | tools | Controls write claudemd behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tengu_ws_transport_closed` | gate | tools | Controls ws transport closed behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tengu_ws_transport_reconnected` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | medium | 1 |
| `tengu_ws_transport_reconnecting` | gate | tools | Controls ws transport reconnecting behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `todo_reminders` | gate | tools | Controls todo reminders behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `token_lifetime_seconds` | gate | tools | Controls token lifetime seconds behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `token_type_hint` | gate | tools | Controls token type hint behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `token_url` | gate | tools | Controls token url behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `token_usage` | gate | tools | Controls token usage behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `too_many_pings` | gate | tools | Controls version-threshold behavior for feature compatibility checks. | Inference based on version/minVersion usage context. | high | 1 |
| `tool` | gate | tools | Controls tool behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tool_decision` | gate | tools | Controls tool decision behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `tool_permission` | gate | tools | Controls tool permission behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `tool_result` | gate | telemetry | Configures telemetry/event logging behavior. | Inference based on event/logging strings and config usage context. | high | 3 |
| `tool_use` | gate | tools | Controls tool use behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `tool_use_single` | gate | tools | Controls tool use single behavior. | Heuristic inference from non-LLM flag context. | high | 7 |
| `tools` | gate | tools | Controls tools behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `transcript_prompt` | gate | tools | Controls transcript prompt behavior. | Heuristic inference from non-LLM flag context. | medium | 1 |
| `turn_start` | gate | tools | Controls turn start behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `ultra_claude_md` | gate | tools | Controls ultra claude md behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `ultrathink_effort` | gate | tools | Controls ultrathink effort behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `unified_tasks` | gate | tools | Controls unified tasks behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `universe_domain` | gate | tools | Controls universe domain behavior. | Heuristic inference from non-LLM flag context. | high | 4 |
| `use_conversation_engine` | gate | tools | Controls use conversation engine behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `user_allow_rules_to_replace` | gate | tools | Controls user allow rules to replace behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `user_deny_rules_to_replace` | gate | tools | Controls user deny rules to replace behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `user_environment_to_replace` | gate | tools | Controls user environment to replace behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `user_prompt` | gate | tools | Controls user prompt behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `verify_plan_reminder` | gate | tools | Controls verify plan reminder behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `wait_for_ready` | gate | tools | Controls wait for ready behavior. | Heuristic inference from non-LLM flag context. | high | 2 |
| `worker_threads` | gate | tools | Controls worker threads behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `workforce_pool_user_project` | gate | tools | Controls workforce pool user project behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
| `ws_already_closed` | gate | tools | Controls ws already closed behavior. | Heuristic inference from non-LLM flag context. | high | 1 |
