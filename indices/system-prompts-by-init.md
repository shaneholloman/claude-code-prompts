# System Prompts Index – by init

- Total prompt files: **538**

## Categories

- System prompts (183)
- Tool prompts (114)
- Agent prompts (6)
- Skills (4)
- System data (140)
- System reminders (91)

## System prompts (183)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-prompt-extract-repeatable-session-steps.md`](../system-prompts/system-prompt-extract-repeatable-session-steps.md) | Extract repeatable workflow from session context, then interview user to formalize a reusable skill. | 1,755 | 2.1.32 | 2.1.32 |
| [`system-prompt-summarize-recent-messages.md`](../system-prompts/system-prompt-summarize-recent-messages.md) | Create a detailed chronological summary of only the recent conversation messages with technical specifics. | 841 | 2.1.32 | 2.1.32 |
| [`system-prompt-edit-existing-plan-file.md`](../system-prompts/system-prompt-edit-existing-plan-file.md) | Plan mode: only edit the plan file while interviewing and exploring codebase. | 823 | 2.1.32 | 2.1.32 |
| [`system-prompt-security-scope-and-url-policy.md`](../system-prompts/system-prompt-security-scope-and-url-policy.md) | Follow security boundaries, require authorization, and avoid guessing URLs without confidence. | 762 | 2.1.32 | 2.1.32 |
| [`system-prompt-confirm-risky-actions.md`](../system-prompts/system-prompt-confirm-risky-actions.md) | Advises confirming with the user before taking risky or hard-to-reverse actions. | 542 | 2.1.32 | 2.1.32 |
| [`system-prompt-search-past-session-context.md`](../system-prompts/system-prompt-search-past-session-context.md) | Proactively grep session summaries and transcript logs for prior context using configured base paths. | 273 | 2.1.32 | 2.1.32 |
| [`system-prompt-coordinate-worker-next-steps.md`](../system-prompts/system-prompt-coordinate-worker-next-steps.md) | Suggest next coordinator actions based on worker status while avoiding generic coding guidance or questions. | 269 | 2.1.32 | 2.1.32 |
| [`system-prompt-maintain-persistent-memory-notes.md`](../system-prompts/system-prompt-maintain-persistent-memory-notes.md) | Use persistent memory directory, keeping concise topic notes and updating learned lessons. | 215 | 2.1.32 | 2.1.32 |
| [`system-prompt-tmux-shift-enter-setup.md`](../system-prompts/system-prompt-tmux-shift-enter-setup.md) | Describe optional terminal steps to enable Shift+Enter multiline shortcut outside tmux. | 179 | 2.1.32 | 2.1.32 |
| [`system-prompt-present-tense-recent-action.md`](../system-prompts/system-prompt-present-tense-recent-action.md) | Multiple prompts (2) | 166 | 2.1.32 | 2.1.32 |
| [`system-prompt-use-scratchpad-directory.md`](../system-prompts/system-prompt-use-scratchpad-directory.md) | Require all temporary files be written to the session scratchpad directory. | 160 | 2.1.32 | 2.1.32 |
| [`system-prompt-team-message-via-sendmessage.md`](../system-prompts/system-prompt-team-message-via-sendmessage.md) | Require using the messaging tool to communicate with teammates during team tasks. | 114 | 2.1.32 | 2.1.32 |
| [`system-prompt-start-coding-after-plan-approval.md`](../system-prompts/system-prompt-start-coding-after-plan-approval.md) | Proceed with coding after plan approval; update todos and reference saved plan content | 65 | 2.1.32 | 2.1.32 |
| [`system-prompt-spawn-and-cleanup-team.md`](../system-prompts/system-prompt-spawn-and-cleanup-team.md) | Define operations to create a team and remove team and task directories. | 19 | 2.1.32 | 2.1.32 |
| [`system-prompt-task-usage-rules.md`](../system-prompts/system-prompt-task-usage-rules.md) | Instructions on avoiding Task tool and running concurrent subagents with brief descriptions. | 1,204 | 2.1.31 | 2.1.31 |
| [`system-prompt-load-deferred-tools-first.md`](../system-prompts/system-prompt-load-deferred-tools-first.md) | Requires searching or selecting deferred tools before calling them. | 836 | 2.1.31 | 2.1.31 |
| [`system-prompt-deferred-loading-modes.md`](../system-prompts/system-prompt-deferred-loading-modes.md) | Explains keyword search and direct selection modes to load deferred tools safely. | 711 | 2.1.31 | 2.1.31 |
| [`system-prompt-prefer-dedicated-tools.md`](../system-prompts/system-prompt-prefer-dedicated-tools.md) | Directive to prefer dedicated tools over bash and manage work via Task subagents. | 490 | 2.1.31 | 2.1.31 |
| [`system-prompt-mandatory-deferred-loader.md`](../system-prompts/system-prompt-mandatory-deferred-loader.md) | Enforces searching or selecting deferred tools to load them before any direct calls | 128 | 2.1.31 | 2.1.31 |
| [`system-prompt-use-read-edit-write.md`](../system-prompts/system-prompt-use-read-edit-write.md) | Maps common shell actions to dedicated file tools and limits bash usage. | 128 | 2.1.31 | 2.1.31 |
| [`system-prompt-hooks-configuration-json.md`](../system-prompts/system-prompt-hooks-configuration-json.md) | Defines JSON structure and event types for lifecycle hooks that run commands. | 1,335 | 2.1.30 | 2.1.30 |
| [`system-prompt-mcp-cli-schema-first.md`](../system-prompts/system-prompt-mcp-cli-schema-first.md) | System rule requiring mcp-cli info before any mcp-cli tool call. | 1,298 | 2.1.30 | 2.1.30 |
| [`system-prompt-plan-mode-restrictions-2.md`](../system-prompts/system-prompt-plan-mode-restrictions-2.md) | Enforces plan-only mode, allowing only incremental edits to the specified plan file. | 1,233 | 2.1.30 | 2.1.30 |
| [`system-prompt-extract-session-analytics.md`](../system-prompts/system-prompt-extract-session-analytics.md) | Guidelines to extract and count user goals, satisfaction signals, and friction types from session. | 581 | 2.1.30 | 2.1.30 |
| [`system-prompt-software-engineering-guidelines.md`](../system-prompts/system-prompt-software-engineering-guidelines.md) | Guidelines for completing coding tasks by reading context and editing real files. | 499 | 2.1.30 | 2.1.30 |
| [`system-prompt-read-local-file-2.md`](../system-prompts/system-prompt-read-local-file-2.md) | Specification for a tool that reads local files by absolute path with optional offsets and image support. | 462 | 2.1.30 | 2.1.30 |
| [`system-prompt-md-features-section-html.md`](../system-prompts/system-prompt-md-features-section-html.md) | HTML for features and patterns sections with copy actions and injected content blocks. | 345 | 2.1.30 | 2.1.30 |
| [`system-prompt-at-a-glance-html-section.md`](../system-prompts/system-prompt-at-a-glance-html-section.md) | At-a-glance HTML dashboard with four linked sections summarizing wins, friction, quick wins, horizons. | 298 | 2.1.30 | 2.1.30 |
| [`system-prompt-keybinding-config-validation.md`](../system-prompts/system-prompt-keybinding-config-validation.md) | Validate keybinding config via …, interpret errors/warnings, and apply common issue fixes. | 252 | 2.1.30 | 2.1.30 |
| [`system-prompt-avoid-unasked-changes.md`](../system-prompts/system-prompt-avoid-unasked-changes.md) | Directs to implement only requested changes and avoid extra refactors, validation, or abstractions. | 183 | 2.1.30 | 2.1.30 |
| [`system-prompt-authorized-security-rules.md`](../system-prompts/system-prompt-authorized-security-rules.md) | Security assistance policy emphasizing authorization limits and no URL guessing. | 179 | 2.1.30 | 2.1.30 |
| [`system-prompt-sleep-until-user-message.md`](../system-prompts/system-prompt-sleep-until-user-message.md) | Instruction to wait for a duration and wake early on user input or ticks. | 169 | 2.1.30 | 2.1.30 |
| [`system-prompt-bar-row-html-snippet.md`](../system-prompts/system-prompt-bar-row-html-snippet.md) | HTML bar-row snippet rendering a label, percentage-filled bar, and value metadata text. | 141 | 2.1.30 | 2.1.30 |
| [`system-prompt-summarize-session-transcript.md`](../system-prompts/system-prompt-summarize-session-transcript.md) | Instructions to concisely summarize a Claude Code transcript chunk with key details. | 116 | 2.1.30 | 2.1.30 |
| [`system-prompt-progress-bar-row-html.md`](../system-prompts/system-prompt-progress-bar-row-html.md) | HTML progress bar row with label, width percentage, color, and displayed value. | 111 | 2.1.30 | 2.1.30 |
| [`system-prompt-redirect-detected.md`](../system-prompts/system-prompt-redirect-detected.md) | Request WebFetch rerun to retrieve content from redirected host URL with new parameters. | 92 | 2.1.30 | 2.1.30 |
| [`system-prompt-task-examples-table-rows.md`](../system-prompts/system-prompt-task-examples-table-rows.md) | Markdown table of common engineering tasks with customizable topics and extra rows. | 91 | 2.1.30 | 2.1.30 |
| [`system-prompt-launch-subagent-for-tasks.md`](../system-prompts/system-prompt-launch-subagent-for-tasks.md) | Defines Task tool subagent types and requires selecting subagent_type for autonomous tasks | 90 | 2.1.30 | 2.1.30 |
| [`system-prompt-at-a-glance-summary-block.md`](../system-prompts/system-prompt-at-a-glance-summary-block.md) | At-a-glance block listing what works, hindrances, quick wins, and ambitious workflows. | 85 | 2.1.30 | 2.1.30 |
| [`system-prompt-usage-section-html-snippet.md`](../system-prompts/system-prompt-usage-section-html-snippet.md) | HTML usage section narrative with injected text and key-insight pattern markup placeholders | 78 | 2.1.30 | 2.1.30 |
| [`system-prompt-resume-metadata.md`](../system-prompts/system-prompt-resume-metadata.md) | Provides agent resume metadata: agentId, token usage, tool uses, and duration. | 65 | 2.1.30 | 2.1.30 |
| [`system-prompt-impressive-wins-section-html.md`](../system-prompts/system-prompt-impressive-wins-section-html.md) | HTML wins section header with intro text and injected list of big wins. | 64 | 2.1.30 | 2.1.30 |
| [`system-prompt-friction-section-html-snippet.md`](../system-prompts/system-prompt-friction-section-html-snippet.md) | Friction section HTML with intro text and injected friction category blocks placeholders. | 63 | 2.1.30 | 2.1.30 |
| [`system-prompt-on-the-horizon-section.md`](../system-prompts/system-prompt-on-the-horizon-section.md) | HTML on-the-horizon section with intro paragraph and dynamic horizon content area. | 63 | 2.1.30 | 2.1.30 |
| [`system-prompt-async-launched-message.md`](../system-prompts/system-prompt-async-launched-message.md) | System notice that an async agent started, providing an internal agent resume ID. | 54 | 2.1.30 | 2.1.30 |
| [`system-prompt-help-feedback.md`](../system-prompts/system-prompt-help-feedback.md) | Help text for Claude Code usage and instructions for submitting user feedback. | 25 | 2.1.30 | 2.1.30 |
| [`system-prompt-ask-what-to-clarify.md`](../system-prompts/system-prompt-ask-what-to-clarify.md) | Ask what needs clarification, then restate questions using the user’s added context. | 74 | 2.1.26 | 2.1.26 |
| [`system-prompt-handle-subagent-exit-codes.md`](../system-prompts/system-prompt-handle-subagent-exit-codes.md) | Routes stdout and stderr visibility based on subagent exit codes from a JSON command input. | 71 | 2.1.26 | 2.1.26 |
| [`system-prompt-background-task-monitor-resume.md`](../system-prompts/system-prompt-background-task-monitor-resume.md) | Notify that a task runs in background and show how to monitor or resume it. | 57 | 2.1.26 | 2.1.26 |
| [`system-prompt-finish-plan-no-more-questions.md`](../system-prompts/system-prompt-finish-plan-no-more-questions.md) | Stop clarifying questions and finish the plan using provided Q&A context. | 53 | 2.1.26 | 2.1.26 |
| [`system-prompt-invoke-matching.md`](../system-prompts/system-prompt-invoke-matching.md) | Invoke the appropriate skill when a user request matches one. | 323 | 2.1.23 | 2.1.23 |
| [`system-prompt-secure-cli-assistance.md`](../system-prompts/system-prompt-secure-cli-assistance.md) | CLI assistant for authorized security help, refusing misuse and not inventing URLs | 226 | 2.1.23 | 2.1.23 |
| [`system-prompt-collect-process-commandline-chain.md`](../system-prompts/system-prompt-collect-process-commandline-chain.md) | Iterate up parent processes to collect command lines and join into one string. | 174 | 2.1.23 | 2.1.23 |
| [`system-prompt-list-process-ancestor-pids.md`](../system-prompts/system-prompt-list-process-ancestor-pids.md) | Walk up parent process IDs to build and output a comma-separated ancestor list. | 144 | 2.1.23 | 2.1.23 |
| [`system-prompt-teammate-task-selection-rules.md`](../system-prompts/system-prompt-teammate-task-selection-rules.md) | Guidelines for finding, prioritizing, and claiming available work items. | 140 | 2.1.21 | 2.1.21 |
| [`system-prompt-run-bash-commands-safely-3.md`](../system-prompts/system-prompt-run-bash-commands-safely-3.md) | Run bash commands with optional timeouts, persistent cwd, and mandatory path quoting checks. | 2,692 | 2.1.20 | 2.1.20 |
| [`system-prompt-verify-changes-work.md`](../system-prompts/system-prompt-verify-changes-work.md) | Directs a verification specialist to plan, run verifiers, and report whether code changes actually work. | 2,553 | 2.1.20 | 2.1.20 |
| [`system-prompt-chrome-automation-guidelines-2.md`](../system-prompts/system-prompt-chrome-automation-guidelines-2.md) | Guidelines for using Claude-in-Chrome tools including GIF recording and console log filtering. | 871 | 2.1.20 | 2.1.20 |
| [`system-prompt-plan-mode-user-approval.md`](../system-prompts/system-prompt-plan-mode-user-approval.md) | Switches to plan mode to explore options and get user approval before coding when requirements or architecture are unclear. | 757 | 2.1.20 | 2.1.20 |
| [`system-prompt-web-search-with-mandatory-sources.md`](../system-prompts/system-prompt-web-search-with-mandatory-sources.md) | Enables automatic web search and mandates a Sources section with linked result URLs. | 329 | 2.1.20 | 2.1.32 |
| [`system-prompt-session-title-and-branch.md`](../system-prompts/system-prompt-session-title-and-branch.md) | Generates a concise session title and a claude-prefixed git branch name from a description. | 319 | 2.1.20 | 2.1.20 |
| [`system-prompt-exact-string-edits-in-files.md`](../system-prompts/system-prompt-exact-string-edits-in-files.md) | Define rules for exact in-file string replacements after reading and with unique matches. | 256 | 2.1.20 | 2.1.20 |
| [`system-prompt-install-cursor-keybinding-locally-2.md`](../system-prompts/system-prompt-install-cursor-keybinding-locally-2.md) | Install Cursor Shift+Enter keybinding locally via Keyboard Shortcuts JSON array edit | 191 | 2.1.20 | 2.1.23 |
| [`system-prompt-absolute-paths-and-call-format.md`](../system-prompts/system-prompt-absolute-paths-and-call-format.md) | Sets execution and response rules: absolute paths, include snippets, avoid emojis, tool-call formatting. | 161 | 2.1.20 | 2.1.20 |
| [`system-prompt-cite-with-limited-quotes.md`](../system-prompts/system-prompt-cite-with-limited-quotes.md) | Answer strictly from provided web content with capped quotes and no song lyrics. | 150 | 2.1.20 | 2.1.25 |
| [`system-prompt-permission-denied-reasonable-alternatives.md`](../system-prompts/system-prompt-permission-denied-reasonable-alternatives.md) | Permission denial guidance to try reasonable alternatives or explain need to user. | 150 | 2.1.20 | 2.1.20 |
| [`system-prompt-socat-tcp-to-unix-bridge-2.md`](../system-prompts/system-prompt-socat-tcp-to-unix-bridge-2.md) | Start socat TCP listeners forwarding to a UNIX socket, with exit cleanup trap. | 139 | 2.1.20 | 2.1.20 |
| [`system-prompt-read-large-output-in-chunks.md`](../system-prompts/system-prompt-read-large-output-in-chunks.md) | Guides reading oversized saved output in chunks, searching with grep/jq, meeting coverage threshold | 120 | 2.1.20 | 2.1.20 |
| [`system-prompt-background-task-notification.md`](../system-prompts/system-prompt-background-task-notification.md) | Reports background command status, summary message, and output file path for results. | 102 | 2.1.20 | 2.1.20 |
| [`system-prompt-enable-chrome-automation.md`](../system-prompts/system-prompt-enable-chrome-automation.md) | Invoke claude-in-chrome skill first to enable mcp__claude-in-chrome__ browser automation tools. | 83 | 2.1.20 | 2.1.20 |
| [`system-prompt-hook-evaluation-json-response.md`](../system-prompts/system-prompt-hook-evaluation-json-response.md) | Hook evaluator requiring a JSON ok result with an optional failure reason. | 81 | 2.1.20 | 2.1.20 |
| [`system-prompt-detect-new-topic-title-3.md`](../system-prompts/system-prompt-detect-new-topic-title-3.md) | Determine if a message starts a new topic and produce a short title in JSON. | 76 | 2.1.20 | 2.1.20 |
| [`system-prompt-task-for-search.md`](../system-prompts/system-prompt-task-for-search.md) | Use Task tool for file searches and delegate matching work to specialized agents. | 51 | 2.1.20 | 2.1.20 |
| [`system-prompt-native-host-mcp-command-approval.md`](../system-prompts/system-prompt-native-host-mcp-command-approval.md) | Multiple prompts (2) | 50 | 2.1.20 | 2.1.20 |
| [`system-prompt-handle-interrupting-user-message.md`](../system-prompts/system-prompt-handle-interrupting-user-message.md) | Notify that a new user message arrived and must be addressed after finishing. | 43 | 2.1.20 | 2.1.32 |
| [`system-prompt-shutdown-request-status.md`](../system-prompts/system-prompt-shutdown-request-status.md) | Logs shutdown request delivery to specific host, includes optional details and request ID. | 42 | 2.1.20 | 2.1.20 |
| [`system-prompt-native-host-command-output.md`](../system-prompts/system-prompt-native-host-command-output.md) | Formats log output prefixing command path, tag, and concatenated expression fields. | 37 | 2.1.20 | 2.1.20 |
| [`system-prompt-background-task-input-block.md`](../system-prompts/system-prompt-background-task-input-block.md) | Template block combining background, task, and input placeholders. | 18 | 2.1.20 | 2.1.20 |
| [`system-prompt-load-deferred-tools-first-2.md`](../system-prompts/system-prompt-load-deferred-tools-first-2.md) | Search for or select deferred tools to make them available before calling. | 815 | 2.1.19 | 2.1.32 |
| [`system-prompt-summarize-coding-actions.md`](../system-prompts/system-prompt-summarize-coding-actions.md) | brief past-tense summary of completed coding work under a word limit. | 170 | 2.1.19 | 2.1.19 |
| [`system-prompt-summarize-completed-tools.md`](../system-prompts/system-prompt-summarize-completed-tools.md) | Summarize outcomes of completed MCP tool runs with tool name and result details. | 57 | 2.1.19 | 2.1.19 |
| [`system-prompt-webfetch-auth-url-warning.md`](../system-prompts/system-prompt-webfetch-auth-url-warning.md) | Warns WebFetch fails on authenticated URLs and suggests using an authenticated tool. | 361 | 2.1.16 | 2.1.16 |
| [`system-prompt-install-cursor-keybinding-locally.md`](../system-prompts/system-prompt-install-cursor-keybinding-locally.md) | Multiple prompts (3) | 183 | 2.1.16 | 2.1.23 |
| [`system-prompt-spawn-confirmation.md`](../system-prompts/system-prompt-spawn-confirmation.md) | Confirms an agent was spawned and shows its id, name, and team. | 50 | 2.1.16 | 2.1.16 |
| [`system-prompt-shutdown-approved-confirm-team-lead.md`](../system-prompts/system-prompt-shutdown-approved-confirm-team-lead.md) | Confirms shutdown approval sent to team lead, then exits the specified agent. | 46 | 2.1.16 | 2.1.16 |
| [`system-prompt-shutdown-approved-fallback.md`](../system-prompts/system-prompt-shutdown-approved-fallback.md) | Announces shutdown approval via fallback path and exits the specified agent. | 42 | 2.1.16 | 2.1.16 |
| [`system-prompt-plan-rejection-feedback.md`](../system-prompts/system-prompt-plan-rejection-feedback.md) | Records a plan rejection for EXPR_1, embedding host feedback and message fragments. | 40 | 2.1.16 | 2.1.16 |
| [`system-prompt-avoid-disabling-sandbox.md`](../system-prompts/system-prompt-avoid-disabling-sandbox.md) | Warns against disabling sandbox except under explicit user request or proven sandbox-caused failure. | 448 | 2.1.14 | 2.1.14 |
| [`system-prompt-create-shell-snapshot-file-3.md`](../system-prompts/system-prompt-create-shell-snapshot-file-3.md) | Writes a snapshot script file, clears aliases, injects dynamic sections, and verifies output exists | 251 | 2.1.14 | 2.1.14 |
| [`system-prompt-load-chrome-mcp-tools-first.md`](../system-prompts/system-prompt-load-chrome-mcp-tools-first.md) | Require ToolSearch loading of Claude-in-Chrome MCP tools before calling them. | 168 | 2.1.14 | 2.1.14 |
| [`system-prompt-extract-user-next-step.md`](../system-prompts/system-prompt-extract-user-next-step.md) | Returns only the user-stated next step if explicitly present, otherwise nothing. | 167 | 2.1.14 | 2.1.14 |
| [`system-prompt-git-status-snapshot.md`](../system-prompts/system-prompt-git-status-snapshot.md) | Initial git status snapshot showing current branch, main branch reference, and recent commits list | 107 | 2.1.14 | 2.1.14 |
| [`system-prompt-chrome-native-host-truncated.md`](../system-prompts/system-prompt-chrome-native-host-truncated.md) | Truncated Claude Chrome Native Host log snippet ending with an mcp tool marker. | 57 | 2.1.14 | 2.1.14 |
| [`system-prompt-mcp-value-range-error.md`](../system-prompts/system-prompt-mcp-value-range-error.md) | Out-of-range value error specifying MCP bounds for Claude Chrome native host. | 55 | 2.1.14 | 2.1.14 |
| [`system-prompt-continue-last-task.md`](../system-prompts/system-prompt-continue-last-task.md) | Continue from prior conversation state and resume the last task without questions. | 48 | 2.1.14 | 2.1.14 |
| [`system-prompt-json-triggered-command-exit-handling.md`](../system-prompts/system-prompt-json-triggered-command-exit-handling.md) | Defines JSON trigger input and how to handle stdout and stderr by exit code. | 42 | 2.1.10 | 2.1.10 |
| [`system-prompt-chrome-automation-guidelines.md`](../system-prompts/system-prompt-chrome-automation-guidelines.md) | Guidelines for using Claude-in-Chrome tools including GIF recording and console log filtering. | 798 | 2.1.7 | 2.1.7 |
| [`system-prompt-rank-sessions-by-query.md`](../system-prompts/system-prompt-rank-sessions-by-query.md) | Guides selecting the most relevant sessions for a query, prioritizing tag matches. | 477 | 2.1.6 | 2.1.6 |
| [`system-prompt-write-command-descriptions.md`](../system-prompts/system-prompt-write-command-descriptions.md) | Rules for generating clear active-voice descriptions of shell commands. | 211 | 2.1.3 | 2.1.3 |
| [`system-prompt-architect-configs-from-needs.md`](../system-prompts/system-prompt-architect-configs-from-needs.md) | Translate user requirements and project context into precise agent specifications. | 1,139 | 2.0.77 | 2.1.19 |
| [`system-prompt-guide-scope-docs.md`](../system-prompts/system-prompt-guide-scope-docs.md) | Defines Claude guide scope across Code, Agent SDK, and API with doc sources. | 780 | 2.0.73 | 2.1.27 |
| [`system-prompt-guide-scope-docs-2.md`](../system-prompts/system-prompt-guide-scope-docs-2.md) | Sets guide responsibilities across Claude Code, Agent SDK, and Claude API with doc sources. | 755 | 2.0.73 | 2.1.27 |
| [`system-prompt-predict-user-next-message.md`](../system-prompts/system-prompt-predict-user-next-message.md) | Predicts the next thing the user would naturally type next. | 299 | 2.0.73 | 2.1.14 |
| [`system-prompt-chrome-native-host-disabled.md`](../system-prompts/system-prompt-chrome-native-host-disabled.md) | Warn that Claude Chrome Native Host skill invocation is blocked by disable-model-invocation setting. | 45 | 2.0.73 | 2.0.73 |
| [`system-prompt-security-review-git-diff.md`](../system-prompts/system-prompt-security-review-git-diff.md) | Performs a high-confidence vulnerability review of branch changes using git status, logs, and diffs. | 2,804 | 2.0.70 | 2.0.70 |
| [`system-prompt-fetch-pr-comments.md`](../system-prompts/system-prompt-fetch-pr-comments.md) | Fetch PR-level and review comments via gh API, then format threads with diffs. | 442 | 2.0.70 | 2.1.20 |
| [`system-prompt-review-github-pull-request.md`](../system-prompts/system-prompt-review-github-pull-request.md) | Use GitHub CLI to list/view PRs, fetch diff, and deliver structured code review. | 231 | 2.0.70 | 2.1.20 |
| [`system-prompt-plan-submitted-for-approval.md`](../system-prompts/system-prompt-plan-submitted-for-approval.md) | Notifies plan submission for team lead approval; await inbox response before implementing. | 132 | 2.0.70 | 2.0.70 |
| [`system-prompt-install-tmux-in-wsl.md`](../system-prompts/system-prompt-install-tmux-in-wsl.md) | Explains installing WSL and tmux and starting a tmux session for swarms. | 58 | 2.0.70 | 2.0.70 |
| [`system-prompt-identity-banner.md`](../system-prompts/system-prompt-identity-banner.md) | Declares the CLI identity as Claude Code running on the Claude Agent SDK. | 53 | 2.0.70 | 2.0.70 |
| [`system-prompt-missing-native-host-error.md`](../system-prompts/system-prompt-missing-native-host-error.md) | Signals missing Claude Chrome Native Host tool for requested tool identifier and context. | 48 | 2.0.70 | 2.0.70 |
| [`system-prompt-not-an-object-native-host-error.md`](../system-prompts/system-prompt-not-an-object-native-host-error.md) | Native host error log stating the given value is not an Object. | 41 | 2.0.70 | 2.0.70 |
| [`system-prompt-fix-path-for-native-install.md`](../system-prompts/system-prompt-fix-path-for-native-install.md) | Adds a native install directory to PATH via an export line appended to a file. | 44 | 2.0.68 | 2.0.68 |
| [`system-prompt-dev-conversation-summary-notes.md`](../system-prompts/system-prompt-dev-conversation-summary-notes.md) | Multiple prompts (2) | 1,262 | 2.0.65 | 2.1.20 |
| [`system-prompt-enter-plan-mode-guidance.md`](../system-prompts/system-prompt-enter-plan-mode-guidance.md) | Advises entering plan mode for non-trivial implementations to get user approval first. | 1,019 | 2.0.62 | 2.0.62 |
| [`system-prompt-update-session-notes-file-3.md`](../system-prompts/system-prompt-update-session-notes-file-3.md) | Update session notes file via Edit tool while preserving exact section structure. | 762 | 2.0.58 | 2.0.58 |
| [`system-prompt-session-notes-section-template-2.md`](../system-prompts/system-prompt-session-notes-section-template-2.md) | Defines the required sections and guiding questions for session notes. | 294 | 2.0.58 | 2.0.58 |
| [`system-prompt-read-only-architecture-planning-2.md`](../system-prompts/system-prompt-read-only-architecture-planning-2.md) | Explore codebase and produce implementation plans without modifying files. | 625 | 2.0.56 | 2.0.56 |
| [`system-prompt-read-only-codebase-search.md`](../system-prompts/system-prompt-read-only-codebase-search.md) | System variant for read-only file searching and code analysis. | 482 | 2.0.56 | 2.0.56 |
| [`system-prompt-json-io-errors.md`](../system-prompts/system-prompt-json-io-errors.md) | Define tool JSON input fields and exit-code based error handling. | 80 | 2.0.56 | 2.0.56 |
| [`system-prompt-plan-mode-codebase-exploration.md`](../system-prompts/system-prompt-plan-mode-codebase-exploration.md) | Read-only plan mode: explore codebase, compare approaches, and propose an implementation strategy. | 144 | 2.0.51 | 2.1.20 |
| [`system-prompt-dangerous-delete-operation-warning.md`](../system-prompts/system-prompt-dangerous-delete-operation-warning.md) | Block auto-approval when … would delete a critical system directory, requiring explicit consent. | 42 | 2.0.50 | 2.1.20 |
| [`system-prompt-summarize-new-messages.md`](../system-prompts/system-prompt-summarize-new-messages.md) | Summarizes new conversation messages into a short tagged summary or returns empty if unchanged. | 110 | 2.0.45 | 2.0.45 |
| [`system-prompt-azure-workload-identity-error.md`](../system-prompts/system-prompt-azure-workload-identity-error.md) | Explains missing Azure workload identity parameters and required environment variables with a troubleshooting link. | 108 | 2.0.45 | 2.0.45 |
| [`system-prompt-hook-json-allow-deny.md`](../system-prompts/system-prompt-hook-json-allow-deny.md) | Specifies JSON input and output contract for a hook decision to allow or deny a command. | 61 | 2.0.45 | 2.0.45 |
| [`system-prompt-plan-mode-restrictions.md`](../system-prompts/system-prompt-plan-mode-restrictions.md) | Plan-only mode: edit existing plan file at … via … only | 221 | 2.0.43 | 2.0.43 |
| [`system-prompt-handle-truncated-output.md`](../system-prompts/system-prompt-handle-truncated-output.md) | Handle MCP output truncation by paging/filtering retrieval or warning results may be incomplete. | 68 | 2.0.43 | 2.0.43 |
| [`system-prompt-json-command-io-exit-codes.md`](../system-prompts/system-prompt-json-command-io-exit-codes.md) | Multiple prompts (2) | 46 | 2.0.43 | 2.0.44 |
| [`system-prompt-exit-transcript-rules.md`](../system-prompts/system-prompt-exit-transcript-rules.md) | Specifies how stdout and stderr are displayed for tool call inputs and responses by exit code. | 69 | 2.0.41 | 2.0.41 |
| [`system-prompt-require-mcp-cli-info-before-call.md`](../system-prompts/system-prompt-require-mcp-cli-info-before-call.md) | Enforces running mcp-cli info before any tool call to confirm parameters. | 1,269 | 2.0.36 | 2.1.26 |
| [`system-prompt-json-command-exit-handling.md`](../system-prompts/system-prompt-json-command-exit-handling.md) | Specifies JSON command input and stdout or stderr display by exit code. | 40 | 2.0.36 | 2.0.36 |
| [`system-prompt-sandbox-tmpdir-temporary-files.md`](../system-prompts/system-prompt-sandbox-tmpdir-temporary-files.md) | Defines sandbox command restrictions and mandates TMPDIR-backed temporary files location. | 128 | 2.0.34 | 2.1.14 |
| [`system-prompt-fix-missing-executable-name.md`](../system-prompts/system-prompt-fix-missing-executable-name.md) | Advise fixes when a specified CLI subcommand executable path is missing. | 91 | 2.0.34 | 2.0.34 |
| [`system-prompt-check-mcp-cli-installed.md`](../system-prompts/system-prompt-check-mcp-cli-installed.md) | Append shell snippet to snapshot file, aliasing mcp-cli if unavailable. | 90 | 2.0.34 | 2.0.34 |
| [`system-prompt-hook-json-validation-failure.md`](../system-prompts/system-prompt-hook-json-validation-failure.md) | Report hook JSON output validation failure, showing error, expected schema, and stdout | 37 | 2.0.32 | 2.0.77 |
| [`system-prompt-update-magic-doc-file.md`](../system-prompts/system-prompt-update-magic-doc-file.md) | Update Magic Doc at … with new user insights, preserving header and formatting rules. | 711 | 2.0.30 | 2.0.30 |
| [`system-prompt-document-specific-update.md`](../system-prompts/system-prompt-document-specific-update.md) | Follow document author’s specific update instructions verbatim, overriding general modification rules. | 65 | 2.0.30 | 2.0.30 |
| [`system-prompt-sandbox-required-for-commands.md`](../system-prompts/system-prompt-sandbox-required-for-commands.md) | Requires all commands to run in sandbox mode and disallows bypassing it. | 63 | 2.0.30 | 2.0.30 |
| [`system-prompt-snapshot-functions-base64-encode.md`](../system-prompts/system-prompt-snapshot-functions-base64-encode.md) | Captures user functions by base64 encoding definitions and writing eval restore lines. | 196 | 2.0.24 | 2.0.24 |
| [`system-prompt-snapshot-functions-typeset-dump.md`](../system-prompts/system-prompt-snapshot-functions-typeset-dump.md) | Captures user function definitions via typeset and writes them directly to the snapshot. | 106 | 2.0.24 | 2.0.24 |
| [`system-prompt-authorized-security-testing-guidelines.md`](../system-prompts/system-prompt-authorized-security-testing-guidelines.md) | Allow defensive and authorized security work while refusing malicious or destructive requests. | 91 | 2.0.24 | 2.0.24 |
| [`system-prompt-subagent-context-boundaries.md`](../system-prompts/system-prompt-subagent-context-boundaries.md) | Clarifies sub-agent context boundaries and limits actions to assigned task and available messages. | 114 | 2.0.8 | 2.0.8 |
| [`system-prompt-cli-identity-2.md`](../system-prompts/system-prompt-cli-identity-2.md) | Defines Claude Code as Anthropic's official CLI running in the agent SDK. | 21 | 1.0.128 | 1.0.128 |
| [`system-prompt-frustration-and-pr-detection.md`](../system-prompts/system-prompt-frustration-and-pr-detection.md) | Analyze conversation to output frustration and explicit GitHub pull request send intent flags. | 220 | 1.0.122 | 1.0.122 |
| [`system-prompt-detect-interaction-features.md`](../system-prompts/system-prompt-detect-interaction-features.md) | Instruction to analyze user messages to detect interaction features. | 16 | 1.0.122 | 2.0.22 |
| [`system-prompt-create-md-guide-2.md`](../system-prompts/system-prompt-create-md-guide-2.md) | Analyze the repo and draft or improve a CLAUDE.md with commands and architecture. | 381 | 1.0.112 | 1.0.112 |
| [`system-prompt-structured-coding-todo-list.md`](../system-prompts/system-prompt-structured-coding-todo-list.md) | Guide creating and updating a structured todo list for complex coding sessions. | 2,433 | 1.0.89 | 1.0.89 |
| [`system-prompt-github-issue-title-generator.md`](../system-prompts/system-prompt-github-issue-title-generator.md) | Generates a concise technical GitHub issue title from a bug report. | 254 | 1.0.89 | 1.0.89 |
| [`system-prompt-json-command-exit-rules.md`](../system-prompts/system-prompt-json-command-exit-rules.md) | Defines JSON input and exit code handling for a command, showing stderr only on failure. | 34 | 1.0.85 | 1.0.85 |
| [`system-prompt-fix-settings-json-validation.md`](../system-prompts/system-prompt-fix-settings-json-validation.md) | Analyze Claude Code settings.json validation failure using provided error text and schema, no env changes. | 45 | 1.0.82 | 1.0.82 |
| [`system-prompt-learn-by-doing-human-input.md`](../system-prompts/system-prompt-learn-by-doing-human-input.md) | Request 3–5 line human code contributions for key logic, tracked via TodoList prompts. | 1,137 | 1.0.78 | 1.0.86 |
| [`system-prompt-cli-educational-engineering-insights.md`](../system-prompts/system-prompt-cli-educational-engineering-insights.md) | CLI engineering assistant adds codebase-specific insights before and after coding in formatted blocks | 220 | 1.0.78 | 2.0.67 |
| [`system-prompt-create-statusline-setup-task.md`](../system-prompts/system-prompt-create-statusline-setup-task.md) | Creates a task that invokes the statusline setup subagent. | 31 | 1.0.72 | 1.0.72 |
| [`system-prompt-export-aliases-filter-winpty.md`](../system-prompts/system-prompt-export-aliases-filter-winpty.md) | Writes aliases into the snapshot while filtering winpty aliases on Windows. | 218 | 1.0.65 | 1.0.65 |
| [`system-prompt-record-shell-options-snapshot.md`](../system-prompts/system-prompt-record-shell-options-snapshot.md) | Appends current shell options and enables expand_aliases in the snapshot. | 100 | 1.0.65 | 1.0.65 |
| [`system-prompt-command-json-exit-handling.md`](../system-prompts/system-prompt-command-json-exit-handling.md) | Rules for JSON command input and exit code output handling. | 40 | 1.0.64 | 1.0.64 |
| [`system-prompt-implementation-insights.md`](../system-prompts/system-prompt-implementation-insights.md) | Enforces brief pre/post code educational insights using a named insight banner format. | 134 | 1.0.63 | 2.0.77 |
| [`system-prompt-command-exit-handling.md`](../system-prompts/system-prompt-command-exit-handling.md) | Defines JSON input expectations and exit code behaviors. | 59 | 1.0.55 | 1.0.56 |
| [`system-prompt-exit-handling.md`](../system-prompts/system-prompt-exit-handling.md) | Defines stdout and stderr visibility rules based on command exit code for tool calls. | 62 | 1.0.53 | 1.0.53 |
| [`system-prompt-compaction-command-exit-codes.md`](../system-prompts/system-prompt-compaction-command-exit-codes.md) | Defines JSON input handling and exit-code behavior for compaction commands. | 55 | 1.0.53 | 1.0.53 |
| [`system-prompt-exit-output-handling.md`](../system-prompts/system-prompt-exit-output-handling.md) | Route stdout and stderr visibility based on exit codes. | 45 | 1.0.53 | 1.0.53 |
| [`system-prompt-install-github-app.md`](../system-prompts/system-prompt-install-github-app.md) | Explains adding a workflow to enable Claude Code via @claude mentions after merge. | 393 | 1.0.44 | 1.0.44 |
| [`system-prompt-github-permission-troubleshooting.md`](../system-prompts/system-prompt-github-permission-troubleshooting.md) | Provide quick fixes for common GitHub CLI permission and authorization issues. | 54 | 1.0.28 | 1.0.28 |
| [`system-prompt-github-repo-access-help.md`](../system-prompts/system-prompt-github-repo-access-help.md) | List common GitHub CLI repository access errors and the steps to resolve them. | 52 | 1.0.28 | 1.0.28 |
| [`system-prompt-verify-repo-access-and-scope.md`](../system-prompts/system-prompt-verify-repo-access-and-scope.md) | Validate GitHub repository name, access permissions, and token scopes for private repos. | 61 | 1.0.25 | 2.1.19 |
| [`system-prompt-list-mcp-server-resources.md`](../system-prompts/system-prompt-list-mcp-server-resources.md) | Lists available resources across MCP servers with optional server filtering. | 73 | 1.0.22 | 1.0.22 |
| [`system-prompt-read-mcp-server-resource.md`](../system-prompts/system-prompt-read-mcp-server-resource.md) | Reads a resource from an MCP server by server name and URI. | 73 | 1.0.22 | 1.0.22 |
| [`system-prompt-avoid-rereading-unchanged-resource.md`](../system-prompts/system-prompt-avoid-rereading-unchanged-resource.md) | Instructs to not reread a resource unless it may have changed. | 22 | 1.0.19 | 1.0.19 |
| [`system-prompt-replace-all-occurrences-warning.md`](../system-prompts/system-prompt-replace-all-occurrences-warning.md) | Warns about multiple replacement matches when replace_all is false, requesting unique context. | 61 | 1.0.18 | 2.0.15 |
| [`system-prompt-extract-displayed-file-paths.md`](../system-prompts/system-prompt-extract-displayed-file-paths.md) | Identify and return only explicitly shown file paths when file contents are displayed. | 289 | 1.0.8 | 1.0.8 |
| [`system-prompt-write-file-with-constraints.md`](../system-prompts/system-prompt-write-file-with-constraints.md) | Defines rules for writing files, including reading before overwriting and avoiding new docs. | 145 | 1.0.7 | 1.0.7 |
| [`system-prompt-install-github-cli.md`](../system-prompts/system-prompt-install-github-cli.md) | Install GitHub CLI across macOS, Windows, and Linux. | 41 | 1.0.0 | 1.0.0 |
| [`system-prompt-admin-setup-secrets-apps.md`](../system-prompts/system-prompt-admin-setup-secrets-apps.md) | Have a repository admin install apps and configure secrets when setup fails. | 33 | 1.0.0 | 1.0.0 |
| [`system-prompt-use-owner-path-format.md`](../system-prompts/system-prompt-use-owner-path-format.md) | Use the owner and path or URL format for repository references. | 28 | 1.0.0 | 1.0.0 |
| [`system-prompt-authenticate-with-gh-cli.md`](../system-prompts/system-prompt-authenticate-with-gh-cli.md) | Authenticate to GitHub using gh auth login or environment-based methods. | 25 | 1.0.0 | 1.0.0 |
| [`system-prompt-summarize-conversations.md`](../system-prompts/system-prompt-summarize-conversations.md) | Directs the assistant to summarize conversations. | 13 | 0.2.108 | 2.0.22 |
| [`system-prompt-web-search.md`](../system-prompts/system-prompt-web-search.md) | Sets the assistant to perform web search tool use. | 11 | 0.2.108 | 2.0.22 |
| [`system-prompt-create-view-instrument-selector.md`](../system-prompts/system-prompt-create-view-instrument-selector.md) | Create a new view with specified name, optional description, and InstrumentSelector variants. | 110 | 0.2.76 | 0.2.76 |
| [`system-prompt-nested-template-functions.md`](../system-prompts/system-prompt-nested-template-functions.md) | Nested compiled template functions that concatenate output into a string buffer. | 134 | 0.2.54 | 1.0.86 |
| [`system-prompt-cite-with-limited-quotes-2.md`](../system-prompts/system-prompt-cite-with-limited-quotes-2.md) | Multiple prompts (2) | 140 | 0.2.40 | 2.1.25 |
| [`system-prompt-select-core-frequently-modified-files.md`](../system-prompts/system-prompt-select-core-frequently-modified-files.md) | Choose five diverse frequently modified core-logic filenames from git history stats. | 90 | 0.2.9 | 0.2.9 |
| [`system-prompt-file-updated-snippet-output.md`](../system-prompts/system-prompt-file-updated-snippet-output.md) | Notify that a file was updated and show numbered snippet output from cat -n. | 38 | 0.2.9 | 2.1.20 |
| [`system-prompt-classify-bash-command-prefix.md`](../system-prompts/system-prompt-classify-bash-command-prefix.md) | Determine the appropriate prefix for bash commands requested by a coding agent. | 33 | 0.2.9 | 0.2.9 |

## Tool prompts (114)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`tool-description-spawn-and-manage-teams.md`](../system-prompts/tool-description-spawn-and-manage-teams.md) | Use TeammateTool to create and manage multi-agent teams when collaboration or parallel work would help. | 1,793 | 2.1.32 | 2.1.32 |
| [`tool-description-send-messages-to-teammates.md`](../system-prompts/tool-description-send-messages-to-teammates.md) | Direct or broadcast messaging to teammates via a defined swarm protocol. | 1,199 | 2.1.32 | 2.1.32 |
| [`tool-description-load-deferred-tools-2.md`](../system-prompts/tool-description-load-deferred-tools-2.md) | Discover and load deferred tools via search or selection before invoking them | 130 | 2.1.31 | 2.1.31 |
| [`tool-description-suggest-cc-feature-improvements.md`](../system-prompts/tool-description-suggest-cc-feature-improvements.md) | Instructions to suggest improvements using specific Claude Code features like MCP servers, custom skills, and hooks. | 812 | 2.1.30 | 2.1.30 |
| [`tool-description-at-a-glance-summary-guidelines.md`](../system-prompts/tool-description-at-a-glance-summary-guidelines.md) | Draft NUM-part Claude Code “At a Glance” usage insights: working, hindrances, quick wins, ambitious workflows. | 571 | 2.1.30 | 2.1.30 |
| [`tool-description-read-local-file-path.md`](../system-prompts/tool-description-read-local-file-path.md) | Tool description for reading local files by absolute path with truncation limits. | 466 | 2.1.30 | 2.1.30 |
| [`tool-description-future-opportunities-autonomous-workflows.md`](../system-prompts/tool-description-future-opportunities-autonomous-workflows.md) | JSON template to propose big future opportunities with ambitious workflows, how-to steps, and copyable prompts. | 169 | 2.1.30 | 2.1.30 |
| [`tool-description-friction-points-json-categories.md`](../system-prompts/tool-description-friction-points-json-categories.md) | JSON schema and instructions to categorize user friction patterns with descriptions and examples in second person. | 148 | 2.1.30 | 2.1.30 |
| [`tool-description-analyze-impressive-workflows.md`](../system-prompts/tool-description-analyze-impressive-workflows.md) | Second-person analysis of usage data highlighting what you do well in key workflows. | 135 | 2.1.30 | 2.1.30 |
| [`tool-description-interaction-style-json-narrative.md`](../system-prompts/tool-description-interaction-style-json-narrative.md) | JSON instructions to describe interaction style patterns in second person with bolded key insights. | 119 | 2.1.30 | 2.1.30 |
| [`tool-description-project-areas-session-summary.md`](../system-prompts/tool-description-project-areas-session-summary.md) | JSON output spec to group sessions into project areas with counts and brief descriptions. | 104 | 2.1.30 | 2.1.30 |
| [`tool-description-memorable-moment-json.md`](../system-prompts/tool-description-memorable-moment-json.md) | JSON format request to extract a qualitative, memorable moment with brief context from usage data. | 93 | 2.1.30 | 2.1.30 |
| [`tool-description-list-available-tasks.md`](../system-prompts/tool-description-list-available-tasks.md) | List all tasks and summarize status, owner, and blockers to choose next work. | 240 | 2.1.21 | 2.1.21 |
| [`tool-description-update-task-status-details.md`](../system-prompts/tool-description-update-task-status-details.md) | Tool guidance for updating task status and details without premature completion. | 598 | 2.1.20 | 2.1.20 |
| [`tool-description-create-structured-task-list.md`](../system-prompts/tool-description-create-structured-task-list.md) | Instructions for using a tool to maintain and update structured coding session task lists | 547 | 2.1.20 | 2.1.20 |
| [`tool-description-web-search-with-mandatory-sources.md`](../system-prompts/tool-description-web-search-with-mandatory-sources.md) | Enables automatic web search and mandates a Sources section with linked result URLs. | 329 | 2.1.20 | 2.1.32 |
| [`tool-description-exact-file-string-replace.md`](../system-prompts/tool-description-exact-file-string-replace.md) | Describes exact in-file replacement tool rules, requiring prior read and unique old_string. | 228 | 2.1.20 | 2.1.22 |
| [`tool-description-write-file-safely.md`](../system-prompts/tool-description-write-file-safely.md) | Write a file to disk, overwriting existing, preferring edits and avoiding new docs. | 114 | 2.1.20 | 2.1.20 |
| [`tool-description-get-accessibility-tree.md`](../system-prompts/tool-description-get-accessibility-tree.md) | Return an accessibility tree snapshot with options to limit scope and output size. | 99 | 2.1.20 | 2.1.20 |
| [`tool-description-stop-background-task.md`](../system-prompts/tool-description-stop-background-task.md) | stops a running background task by task id and returns success status. | 46 | 2.1.19 | 2.1.19 |
| [`tool-description-fetch-task-details-and-dependencies.md`](../system-prompts/tool-description-fetch-task-details-and-dependencies.md) | Retrieve full task details and dependency context by task id. | 175 | 2.1.16 | 2.1.16 |
| [`tool-description-share-free-week-referral.md`](../system-prompts/tool-description-share-free-week-referral.md) | Offers an option to share a free week of Claude Code with friends. | 13 | 2.1.15 | 2.1.16 |
| [`tool-description-bash-command-execution.md`](../system-prompts/tool-description-bash-command-execution.md) | Tool spec for running bash commands with directory verification and path quoting rules. | 975 | 2.1.14 | 2.1.14 |
| [`tool-description-fetch-and-analyze-web-content.md`](../system-prompts/tool-description-fetch-and-analyze-web-content.md) | Describes a tool that fetches a URL, converts HTML to markdown, and analyzes it with a small model. | 291 | 2.1.14 | 2.1.14 |
| [`tool-description-fork-conversation-here.md`](../system-prompts/tool-description-fork-conversation-here.md) | Create a fork of the current conversation at the current point. | 10 | 2.1.8 | 2.1.8 |
| [`tool-description-ask-quick-side-question.md`](../system-prompts/tool-description-ask-quick-side-question.md) | Asks a brief side question without derailing the main thread. | 11 | 2.1.6 | 2.1.6 |
| [`tool-description-open-keybindings-config.md`](../system-prompts/tool-description-open-keybindings-config.md) | Opens or creates the keybindings configuration file. | 10 | 2.1.6 | 2.1.6 |
| [`tool-description-explain-shell-command.md`](../system-prompts/tool-description-explain-shell-command.md) | Explains what a given shell command does. | 8 | 2.1.6 | 2.1.6 |
| [`tool-description-request-plan-approval.md`](../system-prompts/tool-description-request-plan-approval.md) | Guidance on using the tool to submit a completed plan for user review. | 425 | 2.0.77 | 2.1.14 |
| [`tool-description-ask-user-clarifying-questions.md`](../system-prompts/tool-description-ask-user-clarifying-questions.md) | Tool guidance for asking users questions to clarify requirements during execution. | 207 | 2.0.77 | 2.0.77 |
| [`tool-description-enable-or-view-plan.md`](../system-prompts/tool-description-enable-or-view-plan.md) | Toggles plan mode or displays the current session plan. | 9 | 2.0.77 | 2.0.77 |
| [`tool-description-lsp-intelligence-operations-2.md`](../system-prompts/tool-description-lsp-intelligence-operations-2.md) | Use LSP to navigate symbols, references, hover, and call hierarchy in code. | 267 | 2.0.73 | 2.0.73 |
| [`tool-description-list-available-skills.md`](../system-prompts/tool-description-list-available-skills.md) | Display the set of available skills. | 3 | 2.0.73 | 2.0.73 |
| [`tool-description-configure-extra-usage-keep-working.md`](../system-prompts/tool-description-configure-extra-usage-keep-working.md) | Configure extra usage to keep working when limits are hit. | 10 | 2.0.72 | 2.0.72 |
| [`tool-description-show-qr-download-mobile-app.md`](../system-prompts/tool-description-show-qr-download-mobile-app.md) | Show a QR code to download the Claude mobile app. | 10 | 2.0.72 | 2.0.72 |
| [`tool-description-chrome-beta-settings.md`](../system-prompts/tool-description-chrome-beta-settings.md) | Label for the Claude in Chrome beta settings page. | 7 | 2.0.72 | 2.0.72 |
| [`tool-description-browser-mouse-keyboard-control.md`](../system-prompts/tool-description-browser-mouse-keyboard-control.md) | Interact with the browser via mouse and keyboard using screenshots for accurate clicking. | 154 | 2.0.71 | 2.0.71 |
| [`tool-description-record-and-export-gif.md`](../system-prompts/tool-description-record-and-export-gif.md) | Record browser actions and export an annotated animated GIF. | 143 | 2.0.71 | 2.0.71 |
| [`tool-description-find-page-elements.md`](../system-prompts/tool-description-find-page-elements.md) | Locate page elements by natural-language purpose or text and return reusable references. | 112 | 2.0.71 | 2.0.71 |
| [`tool-description-read-browser-console-messages.md`](../system-prompts/tool-description-read-browser-console-messages.md) | Fetch filtered console messages from a tab for debugging. | 102 | 2.0.71 | 2.0.71 |
| [`tool-description-read-network-requests.md`](../system-prompts/tool-description-read-network-requests.md) | Retrieve network request logs from a tab to inspect page traffic. | 97 | 2.0.71 | 2.0.71 |
| [`tool-description-get-mcp-tab-context.md`](../system-prompts/tool-description-get-mcp-tab-context.md) | Return context and tab IDs for the current MCP tab group. | 83 | 2.0.71 | 2.0.71 |
| [`tool-description-upload-image-to-target.md`](../system-prompts/tool-description-upload-image-to-target.md) | Upload a screenshot or image to a file input or drag-and-drop target. | 75 | 2.0.71 | 2.0.71 |
| [`tool-description-execute-page-javascript.md`](../system-prompts/tool-description-execute-page-javascript.md) | Run JavaScript in the page context and return the resulting value or errors. | 68 | 2.0.71 | 2.0.71 |
| [`tool-description-extract-page-raw-text.md`](../system-prompts/tool-description-extract-page-raw-text.md) | Extract plain-text page content prioritizing article-style text. | 59 | 2.0.71 | 2.0.71 |
| [`tool-description-run-shortcut-in-sidepanel.md`](../system-prompts/tool-description-run-shortcut-in-sidepanel.md) | Start a shortcut or workflow in a new sidepanel using the current tab. | 54 | 2.0.71 | 2.0.71 |
| [`tool-description-resize-browser-window.md`](../system-prompts/tool-description-resize-browser-window.md) | Resize the active browser window to specified dimensions. | 46 | 2.0.71 | 2.0.71 |
| [`tool-description-present-plan-for-approval.md`](../system-prompts/tool-description-present-plan-for-approval.md) | Show the user an action plan and domains for approval before proceeding. | 45 | 2.0.71 | 2.0.71 |
| [`tool-description-create-new-mcp-tab.md`](../system-prompts/tool-description-create-new-mcp-tab.md) | Create a new empty tab within the MCP tab group. | 43 | 2.0.71 | 2.0.71 |
| [`tool-description-list-shortcuts-and-workflows.md`](../system-prompts/tool-description-list-shortcuts-and-workflows.md) | List available shortcuts and workflows with commands and metadata. | 41 | 2.0.71 | 2.0.71 |
| [`tool-description-navigate-browser-url.md`](../system-prompts/tool-description-navigate-browser-url.md) | Navigate to a URL or move forward in browser history. | 41 | 2.0.71 | 2.0.71 |
| [`tool-description-fill-form-elements.md`](../system-prompts/tool-description-fill-form-elements.md) | Set form field values using element reference IDs. | 39 | 2.0.71 | 2.0.71 |
| [`tool-description-chrome-native-host-log.md`](../system-prompts/tool-description-chrome-native-host-log.md) | Format timestamped Claude Chrome Native Host log prefix with message and optional suffix. | 26 | 2.0.70 | 2.1.9 |
| [`tool-description-year-in-review-header.md`](../system-prompts/tool-description-year-in-review-header.md) | Title string for a Claude Code year in review. | 12 | 2.0.66 | 2.0.66 |
| [`tool-description-play-thinkback-animation.md`](../system-prompts/tool-description-play-thinkback-animation.md) | Trigger playback of the thinkback animation. | 6 | 2.0.66 | 2.0.66 |
| [`tool-description-get-task-output-status.md`](../system-prompts/tool-description-get-task-output-status.md) | Fetches task output and status with optional blocking for completion. | 104 | 2.0.65 | 2.0.65 |
| [`tool-description-toggle-session-search-tag.md`](../system-prompts/tool-description-toggle-session-search-tag.md) | Toggles a searchable tag on the current session. | 9 | 2.0.65 | 2.0.65 |
| [`tool-description-show-current-context-usage.md`](../system-prompts/tool-description-show-current-context-usage.md) | Display current context usage information. | 4 | 2.0.63 | 2.0.63 |
| [`tool-description-enter-plan-mode-signoff.md`](../system-prompts/tool-description-enter-plan-mode-signoff.md) | Advises entering plan mode to propose an implementation approach and get approval. | 1,023 | 2.0.62 | 2.0.62 |
| [`tool-description-install-slack-app.md`](../system-prompts/tool-description-install-slack-app.md) | Instruction to install the Claude Slack app. | 6 | 2.0.62 | 2.0.62 |
| [`tool-description-configure-mcp-connection.md`](../system-prompts/tool-description-configure-mcp-connection.md) | Run a specific MCP subcommand with arguments, prompting enter to configure | 30 | 2.0.50 | 2.0.50 |
| [`tool-description-configure-default-remote-environment.md`](../system-prompts/tool-description-configure-default-remote-environment.md) | Set the default remote environment for teleport sessions. | 9 | 2.0.47 | 2.0.47 |
| [`tool-description-structured-final-output.md`](../system-prompts/tool-description-structured-final-output.md) | Require a single tool call to return the final structured response. | 34 | 2.0.43 | 2.0.43 |
| [`tool-description-return-verification-result.md`](../system-prompts/tool-description-return-verification-result.md) | Require a single tool call to output the verification result at the end. | 24 | 2.0.43 | 2.0.43 |
| [`tool-description-rate-limit-options.md`](../system-prompts/tool-description-rate-limit-options.md) | Display available options when a rate limit is reached. | 7 | 2.0.43 | 2.0.43 |
| [`tool-description-rename-conversation.md`](../system-prompts/tool-description-rename-conversation.md) | Renames the current conversation. | 5 | 2.0.41 | 2.0.41 |
| [`tool-description-order-stickers.md`](../system-prompts/tool-description-order-stickers.md) | Requests placing an order for Claude Code stickers. | 5 | 2.0.32 | 2.0.32 |
| [`tool-description-manage-plugins.md`](../system-prompts/tool-description-manage-plugins.md) | Manage plugins for Claude Code. | 5 | 2.0.12 | 2.0.12 |
| [`tool-description-fast-glob-file-matcher.md`](../system-prompts/tool-description-fast-glob-file-matcher.md) | Glob-based file matcher returning paths sorted by modification time and supports batching searches. | 115 | 2.0.2 | 2.1.14 |
| [`tool-description-restore-previous-state.md`](../system-prompts/tool-description-restore-previous-state.md) | Restores code and/or conversation to an earlier point. | 12 | 2.0.2 | 2.0.2 |
| [`tool-description-view-update-privacy-settings.md`](../system-prompts/tool-description-view-update-privacy-settings.md) | View and update privacy settings. | 6 | 1.0.96 | 1.0.96 |
| [`tool-description-list-todo-items.md`](../system-prompts/tool-description-list-todo-items.md) | Requests listing the current todo items. | 4 | 1.0.94 | 1.0.94 |
| [`tool-description-structured-todo-list.md`](../system-prompts/tool-description-structured-todo-list.md) | Criteria for starting, updating, and avoiding a structured todo tool during coding sessions | 2,438 | 1.0.89 | 2.1.3 |
| [`tool-description-context-usage-grid.md`](../system-prompts/tool-description-context-usage-grid.md) | Renders current context usage as a colored grid visualization. | 10 | 1.0.86 | 1.0.86 |
| [`tool-description-collaborative-learning-cli.md`](../system-prompts/tool-description-collaborative-learning-cli.md) | Interactive CLI that blends task completion with learning by requesting meaningful human code contributions. | 1,009 | 1.0.78 | 2.0.32 |
| [`tool-description-educational-cli-engineering-help.md`](../system-prompts/tool-description-educational-cli-engineering-help.md) | Interactive CLI for engineering tasks with educational codebase insights under an explanatory style. | 92 | 1.0.78 | 2.0.32 |
| [`tool-description-set-output-style-menu.md`](../system-prompts/tool-description-set-output-style-menu.md) | Instruction to set the output style directly or via a selection menu. | 10 | 1.0.78 | 1.0.78 |
| [`tool-description-bus-error-message.md`](../system-prompts/tool-description-bus-error-message.md) | Reports a bus error from misaligned or invalid memory access. | 16 | 1.0.68 | 1.0.68 |
| [`tool-description-paused-by-ctrl-z-or-suspend.md`](../system-prompts/tool-description-paused-by-ctrl-z-or-suspend.md) | Marks the process as stopped via job-control suspend. | 12 | 1.0.68 | 1.0.68 |
| [`tool-description-child-process-state-change.md`](../system-prompts/tool-description-child-process-state-change.md) | Multiple prompts (2) | 10 | 1.0.68 | 1.0.68 |
| [`tool-description-ctrl-break-interruption.md`](../system-prompts/tool-description-ctrl-break-interruption.md) | Indicates the user interrupted execution with CTRL-BREAK. | 9 | 1.0.68 | 1.0.68 |
| [`tool-description-emulated-command-not-implemented.md`](../system-prompts/tool-description-emulated-command-not-implemented.md) | Indicates a command is expected to be emulated but has no implementation. | 9 | 1.0.68 | 1.0.68 |
| [`tool-description-application-specific-realtime-signal.md`](../system-prompts/tool-description-application-specific-realtime-signal.md) | Denotes receipt of an application-defined realtime signal. | 8 | 1.0.68 | 2.1.14 |
| [`tool-description-ctrl-backslash-user-interruption.md`](../system-prompts/tool-description-ctrl-backslash-user-interruption.md) | Captures a user quit signal triggered by CTRL-\ | 8 | 1.0.68 | 1.0.68 |
| [`tool-description-ctrl-c-user-interruption.md`](../system-prompts/tool-description-ctrl-c-user-interruption.md) | Captures an interactive user interrupt from CTRL-C. | 8 | 1.0.68 | 1.0.68 |
| [`tool-description-socket-out-of-band-data.md`](../system-prompts/tool-description-socket-out-of-band-data.md) | Handle socket notifications for received out-of-band data. | 8 | 1.0.68 | 1.0.68 |
| [`tool-description-background-process-terminal-output.md`](../system-prompts/tool-description-background-process-terminal-output.md) | Diagnose background process attempts to write to terminal output. | 7 | 1.0.68 | 1.0.68 |
| [`tool-description-stack-empty-or-overflowed.md`](../system-prompts/tool-description-stack-empty-or-overflowed.md) | Indicates stack underflow or overflow was detected. | 7 | 1.0.68 | 1.0.68 |
| [`tool-description-background-process-terminal-read-blocked.md`](../system-prompts/tool-description-background-process-terminal-read-blocked.md) | Indicates a background job attempted to read from the controlling terminal. | 6 | 1.0.68 | 1.0.68 |
| [`tool-description-broken-pipe-or-socket.md`](../system-prompts/tool-description-broken-pipe-or-socket.md) | Occurs when writing to a closed pipe or disconnected socket. | 5 | 1.0.68 | 1.0.68 |
| [`tool-description-device-running-out-of-power.md`](../system-prompts/tool-description-device-running-out-of-power.md) | Warns that the device is running low on power. | 5 | 1.0.68 | 1.0.68 |
| [`tool-description-floating-point-arithmetic-error.md`](../system-prompts/tool-description-floating-point-arithmetic-error.md) | Signals a floating-point arithmetic exception occurred. | 5 | 1.0.68 | 1.0.68 |
| [`tool-description-application-specific-signal.md`](../system-prompts/tool-description-application-specific-signal.md) | Multiple prompts (2) | 4 | 1.0.68 | 1.0.68 |
| [`tool-description-request-process-information.md`](../system-prompts/tool-description-request-process-information.md) | Represents a request to report current process status information. | 4 | 1.0.68 | 1.0.68 |
| [`tool-description-terminal-window-size-changed.md`](../system-prompts/tool-description-terminal-window-size-changed.md) | React to terminal window size change events. | 4 | 1.0.68 | 1.0.68 |
| [`tool-description-invalid-machine.md`](../system-prompts/tool-description-invalid-machine.md) | Reports an invalid or unsupported CPU instruction was executed. | 3 | 1.0.68 | 1.0.68 |
| [`tool-description-manage-configurations.md`](../system-prompts/tool-description-manage-configurations.md) | Create and maintain agent configuration settings. | 4 | 1.0.60 | 1.0.60 |
| [`tool-description-export-conversation-to-file.md`](../system-prompts/tool-description-export-conversation-to-file.md) | Export the current conversation to a file or clipboard. | 9 | 1.0.44 | 1.0.44 |
| [`tool-description-ripgrep-search-guidelines.md`](../system-prompts/tool-description-ripgrep-search-guidelines.md) | Guidelines for using the Grep search tool with regex, filters, and output modes. | 250 | 1.0.38 | 1.0.38 |
| [`tool-description-install-native-build.md`](../system-prompts/tool-description-install-native-build.md) | Install the native build of Claude Code. | 5 | 1.0.31 | 1.0.31 |
| [`tool-description-add-working-directory.md`](../system-prompts/tool-description-add-working-directory.md) | Add a new working directory. | 5 | 1.0.23 | 1.0.23 |
| [`tool-description-list-configured-mcp-resources.md`](../system-prompts/tool-description-list-configured-mcp-resources.md) | Tool to list MCP resources from all or a specified server including server field. | 74 | 1.0.22 | 1.0.22 |
| [`tool-description-read-resource-by-uri.md`](../system-prompts/tool-description-read-resource-by-uri.md) | Tool to read an MCP resource by server name and resource URI. | 54 | 1.0.22 | 1.0.22 |
| [`tool-description-upgrade-to-max-rate-limits.md`](../system-prompts/tool-description-upgrade-to-max-rate-limits.md) | Promotes upgrading to Max to get higher rate limits and more Opus access. | 12 | 1.0.11 | 1.0.11 |
| [`tool-description-show-status-details.md`](../system-prompts/tool-description-show-status-details.md) | Command to display Claude Code status, version, model, connectivity, and tools. | 18 | 1.0.4 | 1.0.4 |
| [`tool-description-manage-ide-integrations-status.md`](../system-prompts/tool-description-manage-ide-integrations-status.md) | Manage IDE MCP integrations and display their status. | 8 | 0.2.126 | 1.0.0 |
| [`tool-description-list-manage-background-tasks.md`](../system-prompts/tool-description-list-manage-background-tasks.md) | List and manage background tasks. | 5 | 0.2.117 | 2.0.45 |
| [`tool-description-setup-github-actions.md`](../system-prompts/tool-description-setup-github-actions.md) | Sets up Claude GitHub Actions integration for a repository. | 8 | 0.2.101 | 0.2.101 |
| [`tool-description-option-enter-newline-binding.md`](../system-prompts/tool-description-option-enter-newline-binding.md) | Enable Option+Enter to insert newlines. | 12 | 0.2.80 | 0.2.83 |
| [`tool-description-list-files-in-context.md`](../system-prompts/tool-description-list-files-in-context.md) | List all files currently available in context. | 6 | 0.2.79 | 0.2.79 |
| [`tool-description-replace-jupyter-notebook-cell.md`](../system-prompts/tool-description-replace-jupyter-notebook-cell.md) | Replaces, inserts, or deletes a specific Jupyter notebook cell by index. | 117 | 0.2.9 | 0.2.83 |
| [`tool-description-sign-in-anthropic-account.md`](../system-prompts/tool-description-sign-in-anthropic-account.md) | Signs in using an Anthropic account. | 8 | 0.2.9 | 0.2.9 |
| [`tool-description-sign-out-anthropic-account.md`](../system-prompts/tool-description-sign-out-anthropic-account.md) | Signs out from an Anthropic account. | 8 | 0.2.9 | 0.2.9 |
| [`tool-description-submit-feedback.md`](../system-prompts/tool-description-submit-feedback.md) | Submits user feedback about Claude Code. | 5 | 0.2.9 | 1.0.102 |

## Agent prompts (6)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`agent-prompt-shell-ps1-to-statusline.md`](../system-prompts/agent-prompt-shell-ps1-to-statusline.md) | Converts PS1 from shell config into a Claude Code statusLine command. | 1,542 | 2.1.19 | 2.1.19 |
| [`agent-prompt-use-current-user-config.md`](../system-prompts/agent-prompt-use-current-user-config.md) | Incorporate the user’s current custom environment configuration into relevant answers and suggestions. | 47 | 2.1.14 | 2.1.14 |
| [`agent-prompt-safe-bash-command-execution.md`](../system-prompts/agent-prompt-safe-bash-command-execution.md) | Execute shell and git commands efficiently with clear output and safety checks. | 102 | 2.0.77 | 2.0.77 |
| [`agent-prompt-read-only-architecture-planning-2.md`](../system-prompts/agent-prompt-read-only-architecture-planning-2.md) | Explore the codebase and produce an implementation plan under strict read-only constraints. | 644 | 2.0.56 | 2.0.56 |
| [`agent-prompt-read-only-codebase-search.md`](../system-prompts/agent-prompt-read-only-codebase-search.md) | Search and analyze an existing codebase in strict read-only mode using provided tools. | 503 | 2.0.56 | 2.0.56 |
| [`agent-prompt-codebase-search-analysis-guide.md`](../system-prompts/agent-prompt-codebase-search-analysis-guide.md) | Guidance for searching and analyzing multiple files in a codebase without creating files. | 287 | 1.0.45 | 2.0.70 |

## Skills (4)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`skill-update-settings-json-hooks.md`](../system-prompts/skill-update-settings-json-hooks.md) | Guidelines for updating settings.json and adding hooks for automated events. | 3,374 | 2.1.30 | 2.1.30 |
| [`skill-debug-session.md`](../system-prompts/skill-debug-session.md) | Guides debugging a reported Claude Code session issue using the session log and settings. | 243 | 2.1.30 | 2.1.30 |
| [`skill-customize-keyboard-shortcuts.md`](../system-prompts/skill-customize-keyboard-shortcuts.md) | Guides safe creation or editing of keybindings with required schema fields and keystroke syntax. | 824 | 2.1.20 | 2.1.20 |
| [`skill-update-local-memory-file.md`](../system-prompts/skill-update-local-memory-file.md) | Skill instructions to update CLAUDE.local.md from repeated session patterns using AskUserQuestion. | 1,103 | 2.1.3 | 2.1.3 |

## System data (140)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-data-workspace-platform-info.md`](../system-prompts/system-data-workspace-platform-info.md) | Lists workspace paths, git status, platform metadata, current date, MCP info, and latest model IDs. | 191 | 2.1.32 | 2.1.32 |
| [`system-data-macos-sandbox-policy-rules.md`](../system-prompts/system-data-macos-sandbox-policy-rules.md) | Sandbox policy denying by default, allowing process control and whitelisted Mach service lookups. | 1,797 | 2.1.31 | 2.1.31 |
| [`system-data-allowed-shell-commands.md`](../system-prompts/system-data-allowed-shell-commands.md) | List of permitted shell commands including basic utilities and docker queries. | 92 | 2.1.31 | 2.1.31 |
| [`system-data-insights-report-html-styles.md`](../system-prompts/system-data-insights-report-html-styles.md) | HTML and CSS styling template defining fonts, colors, spacing, and layout for a report. | 6,853 | 2.1.30 | 2.1.30 |
| [`system-data-report-page-css-styles.md`](../system-prompts/system-data-report-page-css-styles.md) | CSS stylesheet snippet defining layout, typography, and navigation styles. | 4,570 | 2.1.30 | 2.1.30 |
| [`system-data-copy-toggle-collapsible-js.md`](../system-prompts/system-data-copy-toggle-collapsible-js.md) | JavaScript for toggling collapsibles and copying code or selected command text. | 1,359 | 2.1.30 | 2.1.30 |
| [`system-data-common-pronouns-and-verbs.md`](../system-prompts/system-data-common-pronouns-and-verbs.md) | List of high-frequency English function words, pronouns, and basic verbs. | 375 | 2.1.30 | 2.1.30 |
| [`system-data-keyboard-shortcuts-list.md`](../system-prompts/system-data-keyboard-shortcuts-list.md) | Enumerates application and chat commands for navigation, history, confirmation, and UI toggles. | 372 | 2.1.30 | 2.1.30 |
| [`system-data-feedback-collapsible-section-html.md`](../system-prompts/system-data-feedback-collapsible-section-html.md) | HTML feedback section with collapsible headers and injected suggestion blocks for teams. | 356 | 2.1.30 | 2.1.30 |
| [`system-data-usage-report-ready-message.md`](../system-prompts/system-data-usage-report-ready-message.md) | Provides usage insights data and instructs outputting an exact shareable report-ready message. | 144 | 2.1.30 | 2.1.30 |
| [`system-data-coding-task-intent-list-3.md`](../system-prompts/system-data-coding-task-intent-list-3.md) | Enumerates coding help intents: lint/type fixes, refactors, questions, logging, edits, tests, utilities | 101 | 2.1.30 | 2.1.31 |
| [`system-data-misc-terms-and-status-lines.md`](../system-prompts/system-data-misc-terms-and-status-lines.md) | Keyword list with dynamic function labels, load failure notice, and MCP server count. | 85 | 2.1.30 | 2.1.30 |
| [`system-data-disabled-plugins-actions-failed.md`](../system-prompts/system-data-disabled-plugins-actions-failed.md) | Disabled EXPR_1 plugins; EXPR_2 failed on linting, typechecks, refactors, tests, and logging tasks | 85 | 2.1.26 | 2.1.26 |
| [`system-data-settings-files-and-permissions.md`](../system-prompts/system-data-settings-files-and-permissions.md) | Explains settings file locations, load order, and permissions JSON schema. | 755 | 2.1.23 | 2.1.23 |
| [`system-data-progress-verb-word-list.md`](../system-prompts/system-data-progress-verb-word-list.md) | List of whimsical present-participle activity words. | 860 | 2.1.20 | 2.1.20 |
| [`system-data-remote-task-notification-output-2.md`](../system-prompts/system-data-remote-task-notification-output-2.md) | Remote agent task notification includes status, summary, and output file path to read results | 161 | 2.1.20 | 2.1.20 |
| [`system-data-task-notification-output-file-2.md`](../system-prompts/system-data-task-notification-output-file-2.md) | Task notification with status summary and output filename to retrieve results | 136 | 2.1.20 | 2.1.20 |
| [`system-data-environment-directory-details.md`](../system-prompts/system-data-environment-directory-details.md) | Multiple prompts (2) | 114 | 2.1.20 | 2.1.20 |
| [`system-data-coding-task-intent-list-2.md`](../system-prompts/system-data-coding-task-intent-list-2.md) | Enumerates coding help intents: lint/type fixes, refactors, questions, logging, edits, tests, utilities | 87 | 2.1.15 | 2.1.32 |
| [`system-data-configured-dev-features-context.md`](../system-prompts/system-data-configured-dev-features-context.md) | Surface user-configured dev tasks and reference them when answering related questions | 107 | 2.1.14 | 2.1.14 |
| [`system-data-embedded-mcp.md`](../system-prompts/system-data-embedded-mcp.md) | Function template listing coding-assistant commands for linting, refactoring, logging, edits, and tests | 102 | 2.1.14 | 2.1.14 |
| [`system-data-mcp-server-3.md`](../system-prompts/system-data-mcp-server-3.md) | MCP server instruction list for linting, typechecks, refactors, logging, edits, and tests. | 90 | 2.1.7 | 2.1.7 |
| [`system-data-coding-task-intent-list-4.md`](../system-prompts/system-data-coding-task-intent-list-4.md) | Enumerates coding help intents: lint/type fixes, refactors, questions, logging, edits, tests, utilities | 87 | 2.1.7 | 2.1.30 |
| [`system-data-coding-task-intent-list.md`](../system-prompts/system-data-coding-task-intent-list.md) | Enumerates coding help intents: lint/type fixes, refactors, questions, logging, edits, tests, utilities | 73 | 2.1.7 | 2.1.32 |
| [`system-data-github-anthropics-path-entries.md`](../system-prompts/system-data-github-anthropics-path-entries.md) | Repeated GitHub host and organization path strings for anthropics. | 137 | 2.0.77 | 2.0.77 |
| [`system-data-long-numeric-placeholder-list.md`](../system-prompts/system-data-long-numeric-placeholder-list.md) | Provides a long list of numeric placeholders with no added context. | 286 | 2.0.72 | 2.0.72 |
| [`system-data-mouse-actions-command-list.md`](../system-prompts/system-data-mouse-actions-command-list.md) | List of supported UI actions including clicks, typing, scrolling, keys, and screenshots. | 244 | 2.0.71 | 2.0.71 |
| [`system-data-template-function-compiled-output.md`](../system-prompts/system-data-template-function-compiled-output.md) | Lodash template compiler output embedding passthrough markers and nine injected expression segments. | 126 | 2.0.66 | 2.0.66 |
| [`system-data-get-guardrail-response-fields.md`](../system-prompts/system-data-get-guardrail-response-fields.md) | Response fields returned when retrieving a Bedrock guardrail. | 239 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-customization-job-response.md`](../system-prompts/system-data-bedrock-customization-job-response.md) | Model customization job response fields for status, datasets, metrics, and output model details. | 238 | 2.0.63 | 2.0.63 |
| [`system-data-get-provisioned-throughput-response-fields.md`](../system-prompts/system-data-get-provisioned-throughput-response-fields.md) | Provides throughput, ARNs, status, and commitment details for a provisioned model. | 188 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-get-custom-response-fields.md`](../system-prompts/system-data-bedrock-get-custom-response-fields.md) | Field list for GetCustomModelResponse including modelArn, metrics, and status. | 182 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-update-guardrail-request-fields.md`](../system-prompts/system-data-bedrock-update-guardrail-request-fields.md) | Field list for UpdateGuardrailRequest including guardrailIdentifier and policy configs. | 180 | 2.0.63 | 2.0.63 |
| [`system-data-create-guardrail-request-fields.md`](../system-prompts/system-data-create-guardrail-request-fields.md) | Describes configuration fields used to create a Bedrock guardrail. | 180 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-provisioned-summary-fields.md`](../system-prompts/system-data-bedrock-provisioned-summary-fields.md) | Defines attributes included in a Bedrock provisioned model summary. | 175 | 2.0.63 | 2.0.63 |
| [`system-data-automated-reasoning-policy-annotation-actions.md`](../system-prompts/system-data-automated-reasoning-policy-annotation-actions.md) | Action annotations for automated reasoning policy updates and ingestion. | 173 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-get-evaluation-job-response.md`](../system-prompts/system-data-bedrock-get-evaluation-job-response.md) | Evaluation job response fields covering config, encryption, timestamps, and failures. | 173 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-invocation-job-summary.md`](../system-prompts/system-data-bedrock-invocation-job-summary.md) | Fields for Bedrock GetModelInvocationJobResponse job details. | 172 | 2.0.63 | 2.1.26 |
| [`system-data-bedrock-invocation-job-summary-2.md`](../system-prompts/system-data-bedrock-invocation-job-summary-2.md) | Fields for Bedrock GetModelInvocationJobResponse job details. | 171 | 2.0.63 | 2.1.26 |
| [`system-data-bedrockruntime-guardrail-usage-units.md`](../system-prompts/system-data-bedrockruntime-guardrail-usage-units.md) | Usage unit counters for Bedrock Runtime guardrail policies. | 170 | 2.0.63 | 2.0.63 |
| [`system-data-cognito-identity-pool-fields.md`](../system-prompts/system-data-cognito-identity-pool-fields.md) | Lists properties of a Cognito Identity Pool configuration. | 168 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-create-customization-job-fields.md`](../system-prompts/system-data-bedrock-create-customization-job-fields.md) | Field list for CreateModelCustomizationJobRequest including jobName and data configs. | 164 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-evaluation-job-summary.md`](../system-prompts/system-data-bedrock-evaluation-job-summary.md) | Evaluation job summary fields including status, identifiers, task types, and config summary. | 162 | 2.0.63 | 2.0.63 |
| [`system-data-get-import-job-response-fields.md`](../system-prompts/system-data-get-import-job-response-fields.md) | Response fields for retrieving a Bedrock model import job. | 161 | 2.0.63 | 2.0.63 |
| [`system-data-cognito-create-identity-pool-input.md`](../system-prompts/system-data-cognito-create-identity-pool-input.md) | Create identity pool input fields for auth options, providers, and tags. | 156 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-list-custom-models-request-fields.md`](../system-prompts/system-data-bedrock-list-custom-models-request-fields.md) | Field list for ListCustomModelsRequest including time filters, sorting, and pagination. | 151 | 2.0.63 | 2.0.63 |
| [`system-data-update-policy-test-case-request.md`](../system-prompts/system-data-update-policy-test-case-request.md) | Specifies fields to update an automated reasoning policy test case. | 151 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-copy-job-summary-fields.md`](../system-prompts/system-data-bedrock-copy-job-summary-fields.md) | Field list for ModelCopyJobSummary including jobArn, status, and target model details. | 147 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-copy-job-response-fields.md`](../system-prompts/system-data-bedrock-copy-job-response-fields.md) | Field list for GetModelCopyJobResponse including jobArn and status. | 146 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-customization-job-summary-fields.md`](../system-prompts/system-data-bedrock-customization-job-summary-fields.md) | Field list for ModelCustomizationJobSummary including jobArn, status, and timestamps. | 141 | 2.0.63 | 2.0.63 |
| [`system-data-list-copy-jobs-request-filters.md`](../system-prompts/system-data-list-copy-jobs-request-filters.md) | Specifies request parameters for filtering and sorting model copy jobs. | 141 | 2.0.63 | 2.0.63 |
| [`system-data-sts-assume-role-request-fields.md`](../system-prompts/system-data-sts-assume-role-request-fields.md) | Parameters for AWS STS AssumeRoleRequest including session and policy options. | 140 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-foundation-details.md`](../system-prompts/system-data-bedrock-foundation-details.md) | Foundation model metadata including modalities, streaming support, and lifecycle. | 137 | 2.0.63 | 2.1.31 |
| [`system-data-get-policy-build-workflow-response.md`](../system-prompts/system-data-get-policy-build-workflow-response.md) | Lists fields returned when fetching an automated reasoning policy build workflow. | 136 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-foundation-details-2.md`](../system-prompts/system-data-bedrock-foundation-details-2.md) | Foundation model metadata including modalities, streaming support, and lifecycle. | 135 | 2.0.63 | 2.1.31 |
| [`system-data-invoke-response-stream-request-fields.md`](../system-prompts/system-data-invoke-response-stream-request-fields.md) | Fields for Bedrock runtime InvokeModelWithResponseStream request. | 135 | 2.0.63 | 2.0.63 |
| [`system-data-bedrockruntime-converse-request-fields-2.md`](../system-prompts/system-data-bedrockruntime-converse-request-fields-2.md) | Field list for ConverseRequest including modelId, messages, and configs. | 134 | 2.0.63 | 2.1.32 |
| [`system-data-bedrockruntime-converse-request-fields.md`](../system-prompts/system-data-bedrockruntime-converse-request-fields.md) | Field list for ConverseRequest including modelId, messages, and configs. | 133 | 2.0.63 | 2.1.32 |
| [`system-data-bedrockruntime-invoke-request-fields.md`](../system-prompts/system-data-bedrockruntime-invoke-request-fields.md) | Field list for InvokeModelRequest including body, modelId, and guardrail settings. | 132 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-evaluation-job-request.md`](../system-prompts/system-data-bedrock-evaluation-job-request.md) | Inputs for creating a Bedrock evaluation job request. | 131 | 2.0.63 | 2.0.63 |
| [`system-data-list-provisioned-throughputs-request-filters.md`](../system-prompts/system-data-list-provisioned-throughputs-request-filters.md) | Request parameters for listing provisioned model throughputs. | 131 | 2.0.63 | 2.0.63 |
| [`system-data-reasoning-policy-quality-report-metrics.md`](../system-prompts/system-data-reasoning-policy-quality-report-metrics.md) | Captures counts and issues reported for automated reasoning policy definition quality. | 130 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-list-evaluation-jobs-request.md`](../system-prompts/system-data-bedrock-list-evaluation-jobs-request.md) | List evaluation jobs request filters, pagination, and sorting parameters. | 127 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-imported-response-fields.md`](../system-prompts/system-data-bedrock-imported-response-fields.md) | Lists fields returned for an imported Bedrock model response. | 126 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-list-custom-deployments.md`](../system-prompts/system-data-bedrock-list-custom-deployments.md) | List custom model deployments request with time filters, status, and pagination. | 126 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-marketplace-endpoint-fields.md`](../system-prompts/system-data-bedrock-marketplace-endpoint-fields.md) | Fields describing a Bedrock marketplace model endpoint status and config. | 124 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-async-invoke-summary.md`](../system-prompts/system-data-bedrock-async-invoke-summary.md) | Async invoke summary fields including ARN, status, timing, and output config. | 121 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-get-async-invoke-response.md`](../system-prompts/system-data-bedrock-get-async-invoke-response.md) | Async invoke response fields including status, timestamps, and output config. | 121 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-guardrail-content-filter-config.md`](../system-prompts/system-data-bedrock-guardrail-content-filter-config.md) | Configuration fields for Bedrock guardrail content filtering behavior. | 121 | 2.0.63 | 2.1.28 |
| [`system-data-bedrock-create-policy-test-case-fields.md`](../system-prompts/system-data-bedrock-create-policy-test-case-fields.md) | Field list for CreateAutomatedReasoningPolicyTestCaseRequest including policyArn and expected results. | 120 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-guardrail-content-filter-config-2.md`](../system-prompts/system-data-bedrock-guardrail-content-filter-config-2.md) | Configuration fields for Bedrock guardrail content filtering behavior. | 120 | 2.0.63 | 2.1.28 |
| [`system-data-bedrock-get-custom-deployment.md`](../system-prompts/system-data-bedrock-get-custom-deployment.md) | Custom model deployment response fields including ARN, status, timestamps, and failure message. | 119 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-converse-stream-output-events.md`](../system-prompts/system-data-bedrock-converse-stream-output-events.md) | Enumerates streaming events and error variants for ConverseStreamOutput. | 117 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-inference-profile-response.md`](../system-prompts/system-data-bedrock-inference-profile-response.md) | Response fields describing a Bedrock inference profile. | 115 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-bidirectional-stream-output.md`](../system-prompts/system-data-bedrock-bidirectional-stream-output.md) | Bidirectional streaming invoke output with chunk and exception fields. | 109 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-create-invocation-job-request.md`](../system-prompts/system-data-bedrock-create-invocation-job-request.md) | Request fields for creating a Bedrock model invocation job. | 106 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-import-job-request.md`](../system-prompts/system-data-bedrock-import-job-request.md) | Model import job request fields including names, role, sources, tags, and VPC config. | 104 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-response-stream-chunks-errors.md`](../system-prompts/system-data-bedrock-response-stream-chunks-errors.md) | Defines response stream chunk output and possible streaming exceptions. | 100 | 2.0.63 | 2.0.63 |
| [`system-data-nature-and-animal-wordlist.md`](../system-prompts/system-data-nature-and-animal-wordlist.md) | List of nature, space, weather, and animal nouns for naming. | 1,163 | 2.0.58 | 2.0.58 |
| [`system-data-whimsical-adjective-wordlist.md`](../system-prompts/system-data-whimsical-adjective-wordlist.md) | Collection of upbeat descriptive adjectives for naming or styling. | 628 | 2.0.58 | 2.0.58 |
| [`system-data-playful-action-verbs-list.md`](../system-prompts/system-data-playful-action-verbs-list.md) | Whimsical gerund verb list describing playful activities. | 325 | 2.0.50 | 2.0.50 |
| [`system-data-azure-access-token-script.md`](../system-prompts/system-data-azure-access-token-script.md) | Invoke PowerShell to get Az access token, optional tenant, secure-string conversion output JSON. | 327 | 2.0.45 | 2.1.20 |
| [`system-data-http-headers-listing.md`](../system-prompts/system-data-http-headers-listing.md) | Lists common request, tracing, CORS, and response headers alongside placeholder URLs. | 238 | 2.0.45 | 2.0.45 |
| [`system-data-azure-auth-env-vars.md`](../system-prompts/system-data-azure-auth-env-vars.md) | Lists Azure authentication environment variables for tenant, client, secrets, and certs. | 78 | 2.0.45 | 2.0.45 |
| [`system-data-github-actions-review.md`](../system-prompts/system-data-github-actions-review.md) | GitHub Actions PR workflow checking out repo and running Claude code-review plugin. | 405 | 2.0.36 | 2.0.36 |
| [`system-data-filesystem-api-operations-list.md`](../system-prompts/system-data-filesystem-api-operations-list.md) | List of filesystem functions for access, reading, writing, and metadata operations. | 101 | 2.0.24 | 2.0.24 |
| [`system-data-stream-zip-parse-errors.md`](../system-prompts/system-data-stream-zip-parse-errors.md) | Lists possible stream and archive validation error messages. | 72 | 2.0.17 | 2.0.17 |
| [`system-data-mention-triggered-github-workflow.md`](../system-prompts/system-data-mention-triggered-github-workflow.md) | Runs Claude Code action on issues or comments mentioning @claude, using Anthropic API key. | 494 | 2.0.8 | 2.0.8 |
| [`system-data-truncated-numeric-placeholders.md`](../system-prompts/system-data-truncated-numeric-placeholders.md) | Truncated stream of numeric placeholders. | 1,119 | 1.0.59 | 1.0.59 |
| [`system-data-extended-numeric-placeholders.md`](../system-prompts/system-data-extended-numeric-placeholders.md) | Extended list of numeric placeholder values. | 678 | 1.0.59 | 1.0.59 |
| [`system-data-numeric-placeholders-sequence.md`](../system-prompts/system-data-numeric-placeholders-sequence.md) | Sequence of numeric placeholder lines. | 454 | 1.0.59 | 1.0.59 |
| [`system-data-numeric-placeholders-dump.md`](../system-prompts/system-data-numeric-placeholders-dump.md) | Multiple prompts (10) | 447 | 1.0.59 | 1.0.59 |
| [`system-data-repeated-number-placeholders.md`](../system-prompts/system-data-repeated-number-placeholders.md) | Series of repeated numeric placeholder lines. | 223 | 1.0.59 | 1.0.59 |
| [`system-data-character-mapping-table.md`](../system-prompts/system-data-character-mapping-table.md) | Contains numeric sequences and letter markers resembling a mapping table. | 184,755 | 1.0.32 | 1.0.32 |
| [`system-data-numeric-placeholder-list.md`](../system-prompts/system-data-numeric-placeholder-list.md) | Repeated numeric placeholders in a long list. | 573 | 0.2.125 | 0.2.125 |
| [`system-data-http-header-field-list.md`](../system-prompts/system-data-http-header-field-list.md) | List of HTTP request and response header fields including CORS and CSP. | 501 | 0.2.125 | 0.2.125 |
| [`system-data-linter-formatter-list.md`](../system-prompts/system-data-linter-formatter-list.md) | Lists common linters, formatters, and code quality tools. | 98 | 0.2.123 | 0.2.123 |
| [`system-data-underscore-template-runtime.md`](../system-prompts/system-data-underscore-template-runtime.md) | Scaffold compiled template function using escape, join, and print output buffering. | 133 | 0.2.54 | 2.0.66 |
| [`system-data-javascript-builtins-list.md`](../system-prompts/system-data-javascript-builtins-list.md) | Enumeration of common JavaScript globals, typed arrays, collections, and utility functions. | 91 | 0.2.54 | 0.2.54 |
| [`system-data-dom-exception-messages-codes.md`](../system-prompts/system-data-dom-exception-messages-codes.md) | DOM exception names with placeholder numeric codes and messages. | 532 | 0.2.33 | 0.2.33 |
| [`system-data-dom-exception-names-list.md`](../system-prompts/system-data-dom-exception-names-list.md) | List of DOM exception constants including security and network errors. | 184 | 0.2.33 | 0.2.33 |
| [`system-data-dom-media-input-events-list.md`](../system-prompts/system-data-dom-media-input-events-list.md) | List of common DOM, media, and form event names. | 153 | 0.2.33 | 0.2.33 |
| [`system-data-html-block-elements-list.md`](../system-prompts/system-data-html-block-elements-list.md) | List of uppercase HTML structural and block-level tag names. | 148 | 0.2.33 | 0.2.33 |
| [`system-data-wolfram-language-symbols-list.md`](../system-prompts/system-data-wolfram-language-symbols-list.md) | Alphabetical list of Wolfram Language built-in symbol names. | 35,789 | 0.2.9 | 0.2.9 |
| [`system-data-stan-functions-reference-list.md`](../system-prompts/system-data-stan-functions-reference-list.md) | Partial catalog of Stan math, RNG, and distribution functions. | 2,155 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-placeholder-sequence.md`](../system-prompts/system-data-numeric-placeholder-sequence.md) | Repeated numeric placeholder tokens in a long sequence. | 1,791 | 0.2.9 | 0.2.9 |
| [`system-data-html-doctype-variants-list.md`](../system-prompts/system-data-html-doctype-variants-list.md) | Strings enumerating HTML doctype variants including strict, levels, and internet explorer. | 1,099 | 0.2.9 | 2.1.32 |
| [`system-data-html-doctype-variants-list-2.md`](../system-prompts/system-data-html-doctype-variants-list-2.md) | Strings enumerating HTML doctype variants including strict, levels, and internet explorer. | 1,063 | 0.2.9 | 2.1.32 |
| [`system-data-sql-keywords-current-array.md`](../system-prompts/system-data-sql-keywords-current-array.md) | List of SQL reserved words and functions including current and array terms. | 1,000 | 0.2.9 | 0.2.9 |
| [`system-data-repeated-numeric-placeholders.md`](../system-prompts/system-data-repeated-numeric-placeholders.md) | Long sequence of repeated numeric placeholder tokens. | 895 | 0.2.9 | 0.2.9 |
| [`system-data-julia-base-types-list.md`](../system-prompts/system-data-julia-base-types-list.md) | List of Julia core types and standard library names. | 723 | 0.2.9 | 0.2.9 |
| [`system-data-perl-builtin-functions-list.md`](../system-prompts/system-data-perl-builtin-functions-list.md) | List of Perl keywords and built-in functions. | 682 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-placeholder-block.md`](../system-prompts/system-data-numeric-placeholder-block.md) | Block of repeated numeric placeholder tokens. | 531 | 0.2.9 | 0.2.9 |
| [`system-data-hex-color-swatches-ccff.md`](../system-prompts/system-data-hex-color-swatches-ccff.md) | Sequence of hexadecimal color codes in CC/FF step combinations. | 387 | 0.2.9 | 0.2.9 |
| [`system-data-sql-functions-json-regression.md`](../system-prompts/system-data-sql-functions-json-regression.md) | Catalog of SQL functions including JSON, analytics, and regression aggregates. | 297 | 0.2.9 | 0.2.9 |
| [`system-data-stan-distributions-list.md`](../system-prompts/system-data-stan-distributions-list.md) | Enumerates probability distributions used in modeling. | 244 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-placeholders-repeated.md`](../system-prompts/system-data-numeric-placeholders-repeated.md) | Repeated numeric placeholder entries. | 237 | 0.2.9 | 0.2.9 |
| [`system-data-css-selectors-pseudo-classes.md`](../system-prompts/system-data-css-selectors-pseudo-classes.md) | Comprehensive list of CSS pseudo-classes and pseudo-elements. | 228 | 0.2.9 | 0.2.9 |
| [`system-data-javascript-builtins-and-typed-arrays.md`](../system-prompts/system-data-javascript-builtins-and-typed-arrays.md) | Enumerates JavaScript globals, built-in objects, errors, and typed arrays. | 216 | 0.2.9 | 0.2.9 |
| [`system-data-css-pseudo-class-keywords.md`](../system-prompts/system-data-css-pseudo-class-keywords.md) | List of CSS selector pseudo-classes and state keywords. | 186 | 0.2.9 | 0.2.9 |
| [`system-data-swift-keywords-list-2.md`](../system-prompts/system-data-swift-keywords-list-2.md) | List of Swift language keywords and declarations. | 171 | 0.2.9 | 2.1.32 |
| [`system-data-swift-keywords-list-3.md`](../system-prompts/system-data-swift-keywords-list-3.md) | List of Swift language keywords and declarations. | 166 | 0.2.9 | 2.1.32 |
| [`system-data-swift-keywords-list.md`](../system-prompts/system-data-swift-keywords-list.md) | List of Swift language keywords and declarations. | 162 | 0.2.9 | 2.1.32 |
| [`system-data-html-element-name-list.md`](../system-prompts/system-data-html-element-name-list.md) | List of common HTML element tag names. | 160 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-constants-and-paths.md`](../system-prompts/system-data-numeric-constants-and-paths.md) | Lists core constants and environment paths like Inf, NaN, missing, and LOAD_PATH. | 159 | 0.2.9 | 0.2.9 |
| [`system-data-swift-standard-library-functions.md`](../system-prompts/system-data-swift-standard-library-functions.md) | List of Swift standard library functions and assertions utilities. | 151 | 0.2.9 | 0.2.9 |
| [`system-data-swift-attribute-annotations.md`](../system-prompts/system-data-swift-attribute-annotations.md) | List of Swift attribute keywords and Cocoa/Interface Builder annotations including autoclosure and objcMembers. | 127 | 0.2.9 | 0.2.25 |
| [`system-data-media-query-features-list.md`](../system-prompts/system-data-media-query-features-list.md) | List CSS media query features and prefers settings. | 124 | 0.2.9 | 0.2.9 |
| [`system-data-csharp-keywords-list.md`](../system-prompts/system-data-csharp-keywords-list.md) | List of C# language keywords and modifiers. | 113 | 0.2.9 | 0.2.9 |
| [`system-data-javascript-builtins-and-typedarrays.md`](../system-prompts/system-data-javascript-builtins-and-typedarrays.md) | List of JavaScript built-ins and typed array constructors. | 111 | 0.2.9 | 0.2.9 |
| [`system-data-roman-numeral-sequence.md`](../system-prompts/system-data-roman-numeral-sequence.md) | Roman numerals listed sequentially from i through xl. | 108 | 0.2.9 | 0.2.9 |
| [`system-data-cloud-throttling-exception-names.md`](../system-prompts/system-data-cloud-throttling-exception-names.md) | Collection of throttling and limit-exceeded exception identifiers. | 93 | 0.2.9 | 0.2.9 |
| [`system-data-swift-compiler-directives-list.md`](../system-prompts/system-data-swift-compiler-directives-list.md) | List of Swift compiler directives and magic literals. | 83 | 0.2.9 | 0.2.9 |
| [`system-data-csharp-query-keywords-list.md`](../system-prompts/system-data-csharp-query-keywords-list.md) | Lists query and async-related language keywords. | 81 | 0.2.9 | 0.2.9 |
| [`system-data-javascript-keyword-list.md`](../system-prompts/system-data-javascript-keyword-list.md) | List of JavaScript reserved words and control-flow keywords. | 76 | 0.2.9 | 0.2.9 |
| [`system-data-julia-keywords-list.md`](../system-prompts/system-data-julia-keywords-list.md) | List of Julia language keywords and core syntactic forms. | 69 | 0.2.9 | 0.2.9 |
| [`system-data-sql-current-context-functions.md`](../system-prompts/system-data-sql-current-context-functions.md) | Lists SQL current context and time functions. | 69 | 0.2.9 | 0.2.9 |
| [`system-data-sql-data-types-list.md`](../system-prompts/system-data-sql-data-types-list.md) | Lists SQL numeric, character, binary, and temporal types. | 64 | 0.2.9 | 0.2.9 |
| [`system-data-dart-core-types-list.md`](../system-prompts/system-data-dart-core-types-list.md) | List of Dart core types and common classes. | 61 | 0.2.9 | 0.2.9 |
| [`system-data-sql-ddl-null-ordering.md`](../system-prompts/system-data-sql-ddl-null-ordering.md) | SQL DDL and query phrases including constraints and null ordering options. | 53 | 0.2.9 | 0.2.9 |

## System reminders (91)

_Sorted by init (newest first). Showing **45** reminders with more than **30** tokens._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-reminder-interactive-cli-security-guardrails.md`](../system-prompts/system-reminder-interactive-cli-security-guardrails.md) | Sets CLI response style with security testing scope limits and url generation restrictions. | 2,685 | 2.1.32 | 2.1.32 |
| [`system-reminder-interactive-cli-security-guardrails-2.md`](../system-prompts/system-reminder-interactive-cli-security-guardrails-2.md) | Sets CLI response style with security testing scope limits and url generation restrictions. | 2,675 | 2.1.32 | 2.1.32 |
| [`system-reminder-interactive-cli-security-guardrails-3.md`](../system-prompts/system-reminder-interactive-cli-security-guardrails-3.md) | Sets CLI response style with security testing scope limits and url generation restrictions. | 2,675 | 2.1.32 | 2.1.32 |
| [`system-reminder-iterative-plan-file-workflow.md`](../system-prompts/system-reminder-iterative-plan-file-workflow.md) | Plan-only mode: edit just the designated plan file, explore codebase, and interview user iteratively. | 796 | 2.1.32 | 2.1.32 |
| [`system-reminder-task-stopped.md`](../system-prompts/system-reminder-task-stopped.md) | Multiple prompts (2) | 34 | 2.1.32 | 2.1.32 |
| [`system-reminder-architect-guidelines.md`](../system-prompts/system-reminder-architect-guidelines.md) | Guidance for converting user requirements and project context into precise agent specifications. | 1,495 | 2.1.31 | 2.1.31 |
| [`system-reminder-permission-behavior.md`](../system-prompts/system-reminder-permission-behavior.md) | Explains user-visible output, permission prompts, and not retrying denied tool calls. | 347 | 2.1.31 | 2.1.31 |
| [`system-reminder-plan-mode-only-edit-plan-file.md`](../system-prompts/system-reminder-plan-mode-only-edit-plan-file.md) | Enforce plan-only workflow: read-only actions, edit only plan file, phased parallel agents. | 1,094 | 2.1.30 | 2.1.30 |
| [`system-reminder-session-outcome-json.md`](../system-prompts/system-reminder-session-outcome-json.md) | Request JSON evaluation of user goals, outcomes, satisfaction, and session friction. | 259 | 2.1.30 | 2.1.30 |
| [`system-reminder-read-large-pdf-pages.md`](../system-prompts/system-reminder-read-large-pdf-pages.md) | Instructs reading a large PDF by page ranges with per-request limits. | 115 | 2.1.30 | 2.1.30 |
| [`system-reminder-single-turn-direct-answer.md`](../system-prompts/system-reminder-single-turn-direct-answer.md) | Answer a side question once with no tools or follow-ups. | 166 | 2.1.23 | 2.1.23 |
| [`system-reminder-bash-command-prefix-detection.md`](../system-prompts/system-reminder-bash-command-prefix-detection.md) | Policy spec for extracting command prefixes and flagging injection patterns. | 852 | 2.1.20 | 2.1.20 |
| [`system-reminder-handle-interrupting-user-message.md`](../system-prompts/system-reminder-handle-interrupting-user-message.md) | Notify that a new user message arrived and must be addressed after finishing. | 43 | 2.1.20 | 2.1.32 |
| [`system-reminder-web-page-content-from-mcp.md`](../system-prompts/system-reminder-web-page-content-from-mcp.md) | Inject MCP-fetched page payload and path into system reminder web content template | 39 | 2.1.20 | 2.1.20 |
| [`system-reminder-shutdown-team-before-response.md`](../system-prompts/system-reminder-shutdown-team-before-response.md) | Requires shutting down the team before delivering the final user response. | 151 | 2.1.16 | 2.1.16 |
| [`system-reminder-task-tracking.md`](../system-prompts/system-reminder-task-tracking.md) | Suggests creating and updating tasks to track progress when relevant. | 98 | 2.1.16 | 2.1.16 |
| [`system-reminder-plan-mode-end-with-actions.md`](../system-prompts/system-reminder-plan-mode-end-with-actions.md) | Requires ending each turn with a question or plan-approval action in plan mode. | 69 | 2.1.16 | 2.1.16 |
| [`system-reminder-verify-stop-condition-plan.md`](../system-prompts/system-reminder-verify-stop-condition-plan.md) | Checks conversation and codebase to confirm the planned work is completed. | 114 | 2.1.14 | 2.1.14 |
| [`system-reminder-truncated-mcp-log-lines.md`](../system-prompts/system-reminder-truncated-mcp-log-lines.md) | Truncated text block showing character count and an mcp command marker call. | 37 | 2.1.14 | 2.1.14 |
| [`system-reminder-enable-chrome-browser-automation.md`](../system-prompts/system-reminder-enable-chrome-browser-automation.md) | Require enabling the Chrome browser skill before using browser tools. | 69 | 2.1.7 | 2.1.7 |
| [`system-reminder-verify-plan-completion.md`](../system-prompts/system-reminder-verify-plan-completion.md) | After implementing a plan, call the specified tool to verify completion. | 32 | 2.1.2 | 2.1.2 |
| [`system-reminder-empty-todo-list-2.md`](../system-prompts/system-reminder-empty-todo-list-2.md) | Notes the todo list is empty and suggests using it internally without telling the user. | 68 | 2.0.77 | 2.0.77 |
| [`system-reminder-ignore-local-command-messages-2.md`](../system-prompts/system-reminder-ignore-local-command-messages-2.md) | Warns that locally generated command messages should be ignored unless explicitly requested. | 52 | 2.0.77 | 2.0.77 |
| [`system-reminder-delegate-mode-task-coordination.md`](../system-prompts/system-reminder-delegate-mode-task-coordination.md) | Delegate mode limits tools to teammate coordination and task management for team "…". | 159 | 2.0.70 | 2.0.70 |
| [`system-reminder-exit-delegate-mode.md`](../system-prompts/system-reminder-exit-delegate-mode.md) | Announces delegate mode exit and restores access to all tools. | 43 | 2.0.70 | 2.0.70 |
| [`system-reminder-exited-plan-mode-actions.md`](../system-prompts/system-reminder-exited-plan-mode-actions.md) | Indicates plan mode has ended and provides path to the saved plan file. | 47 | 2.0.62 | 2.0.62 |
| [`system-reminder-team-coordination-workflow.md`](../system-prompts/system-reminder-team-coordination-workflow.md) | Multiple prompts (2) | 213 | 2.0.60 | 2.0.60 |
| [`system-reminder-continue-from-plan-file.md`](../system-prompts/system-reminder-continue-from-plan-file.md) | Continue unfinished relevant work by resuming from an existing plan file’s contents. | 46 | 2.0.56 | 2.0.56 |
| [`system-reminder-resume-planning-from-existing-file.md`](../system-prompts/system-reminder-resume-planning-from-existing-file.md) | Review prior plan at EXPR_1, reconcile with new request, then update or overwrite before EXPR_2. | 234 | 2.0.52 | 2.0.52 |
| [`system-reminder-plan-only-no-edits.md`](../system-prompts/system-reminder-plan-only-no-edits.md) | Plan mode: only edit designated plan file, otherwise perform read-only actions and ask clarifications. | 190 | 2.0.43 | 2.0.43 |
| [`system-reminder-nudge-todo-tracking.md`](../system-prompts/system-reminder-nudge-todo-tracking.md) | Suggests using and cleaning up the todo list when it would help track progress. | 91 | 2.0.33 | 2.0.33 |
| [`system-reminder-budget-remaining.md`](../system-prompts/system-reminder-budget-remaining.md) | Multiple prompts (2) | 40 | 2.0.30 | 2.0.30 |
| [`system-reminder-malware-analysis-only.md`](../system-prompts/system-reminder-malware-analysis-only.md) | Analyze suspected malware but refuse to improve or extend it. | 80 | 2.0.24 | 2.0.24 |
| [`system-reminder-hook-blocking-error.md`](../system-prompts/system-reminder-hook-blocking-error.md) | Multiple prompts (2) | 39 | 2.0.17 | 2.0.17 |
| [`system-reminder-token-usage-remaining-line.md`](../system-prompts/system-reminder-token-usage-remaining-line.md) | Multiple prompts (2) | 37 | 2.0.17 | 2.0.17 |
| [`system-reminder-use-context-only-when-relevant.md`](../system-prompts/system-reminder-use-context-only-when-relevant.md) | Multiple prompts (2) | 69 | 2.0.2 | 2.0.2 |
| [`system-reminder-preserve-intentional-file-changes.md`](../system-prompts/system-reminder-preserve-intentional-file-changes.md) | Honor intentional modifications to EXPR_1; consider listed diffs without mentioning them to user. | 84 | 1.0.114 | 1.0.114 |
| [`system-reminder-access-prior-large-note.md`](../system-prompts/system-reminder-access-prior-large-note.md) | Reminds that … was previously read; use … tool to retrieve full contents. | 42 | 1.0.85 | 1.0.85 |
| [`system-reminder-todo-list-updated-silently-2.md`](../system-prompts/system-reminder-todo-list-updated-silently-2.md) | Internal notice that todo list updated; continue tasks without telling user. | 43 | 1.0.69 | 2.0.77 |
| [`system-reminder-selected-lines-context-note.md`](../system-prompts/system-reminder-selected-lines-context-note.md) | Shows user-selected line range from a file and cautions it may be unrelated. | 46 | 1.0.65 | 1.0.65 |
| [`system-reminder-invoke-requested.md`](../system-prompts/system-reminder-invoke-requested.md) | Invoke the specified agent when the user requests it, passing required context. | 32 | 1.0.62 | 1.0.62 |
| [`system-reminder-file-offset-shorter-warning.md`](../system-prompts/system-reminder-file-offset-shorter-warning.md) | Warn that a file is shorter than the requested offset and report line count. | 42 | 1.0.53 | 1.0.53 |
| [`system-reminder-mcp-resource-no-displayable-content.md`](../system-prompts/system-reminder-mcp-resource-no-displayable-content.md) | MCP resource tag pointing to server and URI, with no displayable content. | 31 | 1.0.19 | 1.0.19 |
| [`system-reminder-underscore-template-function-wrapper.md`](../system-prompts/system-reminder-underscore-template-function-wrapper.md) | Compiled Underscore template function skeleton that escapes values and accumulates output. | 70 | 0.2.106 | 0.2.106 |
| [`system-reminder-hide-file-truncation-note.md`](../system-prompts/system-reminder-hide-file-truncation-note.md) | Warn file content is truncated and instruct using a command to read more. | 56 | 0.2.106 | 0.2.106 |

<details>
<summary>Show 46 low-token reminders (≤ 30 tokens)</summary>

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-reminder-user-stopped-task-notice.md`](../system-prompts/system-reminder-user-stopped-task-notice.md) | Notify that task "…" (…) was halted at the user’s request. | 20 | 2.1.32 | 2.1.32 |
| [`system-reminder-enable-path-variable.md`](../system-prompts/system-reminder-enable-path-variable.md) | Insert EXPR_1 content, then remind to enable PATH or alternative configuration. | 16 | 2.1.32 | 2.1.32 |
| [`system-reminder-available-deferred-tools-tag.md`](../system-prompts/system-reminder-available-deferred-tools-tag.md) | Template block listing available deferred tools and a configurable path tag. | 23 | 2.1.31 | 2.1.31 |
| [`system-reminder-found-mcp-servers-desktop.md`](../system-prompts/system-reminder-found-mcp-servers-desktop.md) | Report the number of MCP servers detected in Claude Desktop. | 14 | 2.1.26 | 2.1.26 |
| [`system-reminder-list-available-skills.md`](../system-prompts/system-reminder-list-available-skills.md) | List available Skill tool capabilities by injecting provided skills block. | 20 | 2.1.23 | 2.1.23 |
| [`system-reminder-failed-to-load-message.md`](../system-prompts/system-reminder-failed-to-load-message.md) | Dynamic resource or module name used in a failed-to-load system reminder message. | 9 | 2.1.21 | 2.1.21 |
| [`system-reminder-with-path.md`](../system-prompts/system-reminder-with-path.md) | System reminder wrapper containing multiple placeholder fields and a path tag. | 20 | 2.1.20 | 2.1.20 |
| [`system-reminder-user-intent-from-last-message.md`](../system-prompts/system-reminder-user-intent-from-last-message.md) | Label line capturing inferred user intent from the assistant’s prior message. | 16 | 2.1.19 | 2.1.19 |
| [`system-reminder-list-existing-tasks.md`](../system-prompts/system-reminder-list-existing-tasks.md) | Lists existing tasks for reference before planning or execution begins. | 13 | 2.1.16 | 2.1.16 |
| [`system-reminder-image-source-citation.md`](../system-prompts/system-reminder-image-source-citation.md) | Displays an image source reference value for the current context. | 11 | 2.1.15 | 2.1.15 |
| [`system-reminder-server-status-display.md`](../system-prompts/system-reminder-server-status-display.md) | Reports the current server status value as a labeled status line. | 9 | 2.1.15 | 2.1.15 |
| [`system-reminder-implement-provided-plan.md`](../system-prompts/system-reminder-implement-provided-plan.md) | Directive to implement the provided plan text exactly as given. | 13 | 2.1.10 | 2.1.23 |
| [`system-reminder-enable-path-variable-2.md`](../system-prompts/system-reminder-enable-path-variable-2.md) | Reminder snippet about turning on a PATH setting. | 9 | 2.1.3 | 2.1.32 |
| [`system-reminder-continue-after-token-limit.md`](../system-prompts/system-reminder-continue-after-token-limit.md) | Instructs to continue work in smaller chunks after output cutoff. | 28 | 2.0.77 | 2.0.77 |
| [`system-reminder-follow-invoked-skills-guidelines.md`](../system-prompts/system-reminder-follow-invoked-skills-guidelines.md) | Reminder to keep adhering to the session’s previously invoked skills guidelines. | 23 | 2.0.72 | 2.0.72 |
| [`system-reminder-check-task-output.md`](../system-prompts/system-reminder-check-task-output.md) | Directs the user to check output via TaskOutput. | 11 | 2.0.65 | 2.0.65 |
| [`system-reminder-retirement-warning.md`](../system-prompts/system-reminder-retirement-warning.md) | Warns a specified model will retire on a given date and suggests switching. | 28 | 2.0.62 | 2.0.62 |
| [`system-reminder-stop-hook-feedback.md`](../system-prompts/system-reminder-stop-hook-feedback.md) | Provide stop-hook feedback text to be displayed or logged. | 11 | 2.0.41 | 2.0.41 |
| [`system-reminder-mcp-binary-content-placeholder.md`](../system-prompts/system-reminder-mcp-binary-content-placeholder.md) | Binary MCP content marker with two embedded parameter segments. | 21 | 2.0.34 | 2.0.34 |
| [`system-reminder-usd-budget-remaining.md`](../system-prompts/system-reminder-usd-budget-remaining.md) | Formats USD budget summary showing used, total, and remaining amounts. | 26 | 2.0.30 | 2.0.30 |
| [`system-reminder-hook-additional-context-2.md`](../system-prompts/system-reminder-hook-additional-context-2.md) | Multiple prompts (2) | 30 | 2.0.17 | 2.0.17 |
| [`system-reminder-hook-stopped-continuation-2.md`](../system-prompts/system-reminder-hook-stopped-continuation-2.md) | Multiple prompts (2) | 30 | 2.0.17 | 2.0.17 |
| [`system-reminder-hook-success.md`](../system-prompts/system-reminder-hook-success.md) | Multiple prompts (2) | 29 | 2.0.17 | 2.0.17 |
| [`system-reminder-hook-blocking-command-error.md`](../system-prompts/system-reminder-hook-blocking-command-error.md) | Report a blocking hook error triggered by a specific command execution. | 25 | 2.0.17 | 2.0.17 |
| [`system-reminder-token-usage-remaining.md`](../system-prompts/system-reminder-token-usage-remaining.md) | Shows token usage totals and remaining token budget in a single status line. | 23 | 2.0.17 | 2.0.17 |
| [`system-reminder-hook-additional-context.md`](../system-prompts/system-reminder-hook-additional-context.md) | Attach additional context details for a specified hook invocation. | 16 | 2.0.17 | 2.0.17 |
| [`system-reminder-hook-stopped-continuation.md`](../system-prompts/system-reminder-hook-stopped-continuation.md) | State why a hook stopped the continuation of an ongoing process. | 16 | 2.0.17 | 2.0.17 |
| [`system-reminder-hook-success-message.md`](../system-prompts/system-reminder-hook-success-message.md) | Confirm a hook ran successfully and provide its resulting output. | 15 | 2.0.17 | 2.0.17 |
| [`system-reminder-other-users-modified-files.md`](../system-prompts/system-reminder-other-users-modified-files.md) | Display the list of files modified by other users. | 13 | 1.0.109 | 2.1.15 |
| [`system-reminder-user-modified-files.md`](../system-prompts/system-reminder-user-modified-files.md) | Display the list of files modified by the current user. | 12 | 1.0.109 | 1.0.109 |
| [`system-reminder-clipboard-image-not-found.md`](../system-prompts/system-reminder-clipboard-image-not-found.md) | States clipboard lacks an image and instructs using EXPR_1 to paste one | 17 | 1.0.93 | 1.0.93 |
| [`system-reminder-active-style-guidelines.md`](../system-prompts/system-reminder-active-style-guidelines.md) | Reminder that the active output style must be followed exactly for responses. | 21 | 1.0.78 | 1.0.78 |
| [`system-reminder-continued-session-warning.md`](../system-prompts/system-reminder-continued-session-warning.md) | Warns session resumed on another machine and reports updated working directory path. | 26 | 1.0.68 | 1.0.68 |
| [`system-reminder-template-variable-blocks.md`](../system-prompts/system-reminder-template-variable-blocks.md) | Renders three injected text blocks followed by a trailing numeric value. | 27 | 1.0.52 | 2.1.15 |
| [`system-reminder-show-existing-todo-list.md`](../system-prompts/system-reminder-show-existing-todo-list.md) | Shows the current todo list contents inside a bracketed placeholder. | 19 | 1.0.52 | 1.0.94 |
| [`system-reminder-ide-file-opened-context.md`](../system-prompts/system-reminder-ide-file-opened-context.md) | Indicates the user opened a specific IDE file that may relate to task. | 27 | 1.0.32 | 1.0.32 |
| [`system-reminder-mcp-resource-no-content.md`](../system-prompts/system-reminder-mcp-resource-no-content.md) | MCP resource tag referencing server and URI placeholders, indicating no content available. | 29 | 1.0.19 | 1.0.19 |
| [`system-reminder-full-resource-contents-header.md`](../system-prompts/system-reminder-full-resource-contents-header.md) | Introduces the full contents of a referenced resource. | 5 | 1.0.19 | 1.0.19 |
| [`system-reminder-report-new-diagnostic-issues.md`](../system-prompts/system-reminder-report-new-diagnostic-issues.md) | Announces newly detected diagnostic issues and prints the associated details block. | 27 | 1.0.18 | 1.0.94 |
| [`system-reminder-jt-join-type-options.md`](../system-prompts/system-reminder-jt-join-type-options.md) | Enumeration of JT join type options. | 18 | 0.2.119 | 0.2.119 |
| [`system-reminder-call-error-result.md`](../system-prompts/system-reminder-call-error-result.md) | Template line reporting an error result from a specified tool call. | 13 | 0.2.119 | 0.2.119 |
| [`system-reminder-empty-existing-file-warning.md`](../system-prompts/system-reminder-empty-existing-file-warning.md) | Warns that a referenced file exists but has no contents. | 22 | 0.2.115 | 1.0.53 |
| [`system-reminder-repeat-url-and-expression.md`](../system-prompts/system-reminder-repeat-url-and-expression.md) | Outputs two URL lines followed by an injected expression value. | 20 | 0.2.108 | 2.0.17 |
| [`system-reminder-show-variable-contents.md`](../system-prompts/system-reminder-show-variable-contents.md) | Show contents of a referenced variable or expression with its resolved value. | 16 | 0.2.107 | 0.2.107 |
| [`system-reminder-call-echo-line.md`](../system-prompts/system-reminder-call-echo-line.md) | Log line noting a tool invocation and the exact input provided. | 20 | 0.2.106 | 2.1.20 |
| [`system-reminder-call-result.md`](../system-prompts/system-reminder-call-result.md) | Report the result returned from invoking a specified tool. | 18 | 0.2.106 | 2.0.77 |

</details>
