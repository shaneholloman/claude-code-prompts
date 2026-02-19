# System Prompts Index – by init

- Total prompt files: **483**

## Categories

- System prompts (132)
- Tool prompts (113)
- Agent prompts (7)
- System data (145)
- System reminders (86)

## System prompts (132)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-prompt-safe-persistent-bash-commands.md`](../system-prompts/system-prompt-safe-persistent-bash-commands.md) | Run terminal commands in persistent bash with safety checks, quoting, and directory validation. | 2,583 | 2.0.77 | 2.0.77 |
| [`system-prompt-plan-mode-incremental-plan-file.md`](../system-prompts/system-prompt-plan-mode-incremental-plan-file.md) | Plan-mode guardrails: only edit designated plan file; parallel read-only subagent exploration phases. | 1,173 | 2.0.77 | 2.0.77 |
| [`system-prompt-architect-configs-from-needs.md`](../system-prompts/system-prompt-architect-configs-from-needs.md) | Architect elite AI agents by extracting intent and shaping expert personas with project context. | 1,149 | 2.0.77 | 2.0.77 |
| [`system-prompt-launch-subagent-for-multistep-tasks.md`](../system-prompts/system-prompt-launch-subagent-for-multistep-tasks.md) | Directs when to spawn Task subagents, choose types, and prefer Read/Glob for targeted searches | 1,146 | 2.0.77 | 2.0.77 |
| [`system-prompt-architect-configs-from-needs-2.md`](../system-prompts/system-prompt-architect-configs-from-needs-2.md) | Translate user requirements and project context into precise agent specifications. | 1,139 | 2.0.77 | 2.0.77 |
| [`system-prompt-ufe-enum-tokens-atuser-atgroup.md`](../system-prompts/system-prompt-ufe-enum-tokens-atuser-atgroup.md) | Long enumeration of internal tokens and flags including atUser and atGroup placeholders. | 992 | 2.0.77 | 2.0.77 |
| [`system-prompt-invoke-relevant-skills.md`](../system-prompts/system-prompt-invoke-relevant-skills.md) | Immediately invoke the relevant Skill tool for slash-command tasks before any textual response. | 445 | 2.0.77 | 2.0.77 |
| [`system-prompt-signal-plan-ready-for-approval.md`](../system-prompts/system-prompt-signal-plan-ready-for-approval.md) | Guidance on using the tool to submit a completed plan for user review. | 425 | 2.0.77 | 2.0.77 |
| [`system-prompt-load-chrome-tools-via-mcpsearch.md`](../system-prompts/system-prompt-load-chrome-tools-via-mcpsearch.md) | Instruction to load Chrome MCP tools with MCPSearch before calling them. | 168 | 2.0.77 | 2.0.77 |
| [`system-prompt-terminal-shortcut-setup.md`](../system-prompts/system-prompt-terminal-shortcut-setup.md) | Details setting up Shift+Enter multiline shortcut by running configuration outside tmux in supported terminals | 157 | 2.0.77 | 2.0.77 |
| [`system-prompt-async-output-file-check.md`](../system-prompts/system-prompt-async-output-file-check.md) | Announces async agent launch and how to check progress via its output file. | 118 | 2.0.77 | 2.0.77 |
| [`system-prompt-simple-conversation-title.md`](../system-prompts/system-prompt-simple-conversation-title.md) | Generate a NUM–NUM word conversation title using the last EXPR_1 of EXPR_2 messages. | 115 | 2.0.77 | 2.0.77 |
| [`system-prompt-background-command-task-notification.md`](../system-prompts/system-prompt-background-command-task-notification.md) | Reports background command status, quoting the command and directing to output file path | 113 | 2.0.77 | 2.0.77 |
| [`system-prompt-task-notification-output-file.md`](../system-prompts/system-prompt-task-notification-output-file.md) | Emits task notification with pipe task-id, status, summary, and output file path. | 103 | 2.0.77 | 2.0.77 |
| [`system-prompt-verification-failed-review-issues.md`](../system-prompts/system-prompt-verification-failed-review-issues.md) | Notifies plan verification failure with MCP reason code requiring review and fixes | 74 | 2.0.77 | 2.0.77 |
| [`system-prompt-continue-conversation-without-questions.md`](../system-prompts/system-prompt-continue-conversation-without-questions.md) | Resume prior Claude Chrome Native Host conversation, continuing last task without further questions. | 58 | 2.0.77 | 2.0.77 |
| [`system-prompt-rank-sessions-by-query.md`](../system-prompts/system-prompt-rank-sessions-by-query.md) | Guides selecting the most relevant sessions for a query, prioritizing tag matches. | 482 | 2.0.74 | 2.0.74 |
| [`system-prompt-wait-for-plan-approval.md`](../system-prompts/system-prompt-wait-for-plan-approval.md) | Wait for team lead approval of submitted plan before implementation; monitor inbox response. | 152 | 2.0.74 | 2.0.74 |
| [`system-prompt-guide-scope-docs-2.md`](../system-prompts/system-prompt-guide-scope-docs-2.md) | Defines Claude guide scope across Code, Agent SDK, and API with doc sources. | 780 | 2.0.73 | 2.0.73 |
| [`system-prompt-guide-scope-docs.md`](../system-prompts/system-prompt-guide-scope-docs.md) | Sets guide responsibilities across Claude Code, Agent SDK, and Claude API with doc sources. | 755 | 2.0.73 | 2.0.73 |
| [`system-prompt-chrome-native-host-disabled.md`](../system-prompts/system-prompt-chrome-native-host-disabled.md) | Warn that Claude Chrome Native Host skill invocation is blocked by disable-model-invocation setting. | 45 | 2.0.73 | 2.0.73 |
| [`system-prompt-bash-command-prefix-risk-policy.md`](../system-prompts/system-prompt-bash-command-prefix-risk-policy.md) | Policy spec for extracting shell command prefixes and detecting command injection risk. | 873 | 2.0.71 | 2.0.71 |
| [`system-prompt-chrome-automation-guidelines.md`](../system-prompts/system-prompt-chrome-automation-guidelines.md) | Guidelines for using Claude-in-Chrome tools including GIF recording and console log filtering. | 795 | 2.0.71 | 2.0.71 |
| [`system-prompt-fetch-pr-comments.md`](../system-prompts/system-prompt-fetch-pr-comments.md) | Retrieve and format pull request comments and review threads via GitHub CLI. | 451 | 2.0.71 | 2.0.71 |
| [`system-prompt-review-github-pull-request.md`](../system-prompts/system-prompt-review-github-pull-request.md) | Use GitHub CLI to list/view PRs, fetch diff, and deliver structured code review. | 240 | 2.0.71 | 2.0.71 |
| [`system-prompt-plan-mode-exploration-steps.md`](../system-prompts/system-prompt-plan-mode-exploration-steps.md) | Plan-mode guidelines for read-only exploration, trade-offs, and approval before edits. | 152 | 2.0.71 | 2.0.71 |
| [`system-prompt-web-content-quote-limits-2.md`](../system-prompts/system-prompt-web-content-quote-limits-2.md) | Answer only from supplied page content with limited quotes and no lyrics. | 148 | 2.0.71 | 2.0.77 |
| [`system-prompt-web-content-quote-limits.md`](../system-prompts/system-prompt-web-content-quote-limits.md) | Answer only from supplied page content with limited quotes and no lyrics. | 148 | 2.0.71 | 2.0.77 |
| [`system-prompt-read-pipe-content-in-chunks.md`](../system-prompts/system-prompt-read-pipe-content-in-chunks.md) | Read pipe-saved output in sequential chunks until required percentage is processed. | 139 | 2.0.71 | 2.0.71 |
| [`system-prompt-socat-tcp-to-unix-bridge-2.md`](../system-prompts/system-prompt-socat-tcp-to-unix-bridge-2.md) | Start socat TCP listeners forwarding to a UNIX socket, with exit cleanup trap. | 139 | 2.0.71 | 2.0.71 |
| [`system-prompt-next-step-suggester.md`](../system-prompts/system-prompt-next-step-suggester.md) | Generates a short casual user follow-up prompt based on the conversation context. | 119 | 2.0.71 | 2.0.71 |
| [`system-prompt-git-status-branch-snapshot.md`](../system-prompts/system-prompt-git-status-branch-snapshot.md) | Show initial git status, branch info, and recent commits snapshot for the conversation. | 109 | 2.0.71 | 2.0.71 |
| [`system-prompt-summarize-bash-output.md`](../system-prompts/system-prompt-summarize-bash-output.md) | Decide whether to summarize bash output, then summarize only relevant details. | 64 | 2.0.71 | 2.0.71 |
| [`system-prompt-dangerous-pipe-operation-warning.md`](../system-prompts/system-prompt-dangerous-pipe-operation-warning.md) | Block auto-approval when … would delete a critical system directory, requiring explicit consent. | 51 | 2.0.71 | 2.0.72 |
| [`system-prompt-file-updated-cat-snippet.md`](../system-prompts/system-prompt-file-updated-cat-snippet.md) | Multiple prompts (2) | 47 | 2.0.71 | 2.0.71 |
| [`system-prompt-background-task-pipe-input.md`](../system-prompts/system-prompt-background-task-pipe-input.md) | Background task input referencing the browser bridge pipe and a path placeholder. | 28 | 2.0.71 | 2.0.71 |
| [`system-prompt-security-review-git-diff.md`](../system-prompts/system-prompt-security-review-git-diff.md) | Performs a high-confidence vulnerability review of branch changes using git status, logs, and diffs. | 2,804 | 2.0.70 | 2.0.70 |
| [`system-prompt-absolute-paths-and-call-format.md`](../system-prompts/system-prompt-absolute-paths-and-call-format.md) | Sets execution and response rules: absolute paths, include snippets, avoid emojis, tool-call formatting. | 161 | 2.0.70 | 2.0.70 |
| [`system-prompt-previous-session-notes-header.md`](../system-prompts/system-prompt-previous-session-notes-header.md) | Renders previous session header and notes link with host label and extra content. | 54 | 2.0.70 | 2.0.70 |
| [`system-prompt-identity-banner.md`](../system-prompts/system-prompt-identity-banner.md) | Declares the CLI identity as Claude Code running on the Claude Agent SDK. | 53 | 2.0.70 | 2.0.70 |
| [`system-prompt-missing-native-host-error.md`](../system-prompts/system-prompt-missing-native-host-error.md) | Signals missing Claude Chrome Native Host tool for requested tool identifier and context. | 48 | 2.0.70 | 2.0.70 |
| [`system-prompt-chrome-native-host-truncation.md`](../system-prompts/system-prompt-chrome-native-host-truncation.md) | Formats a Claude Chrome Native Host log message with timestamp, segments, truncation notice, and tail. | 47 | 2.0.70 | 2.0.70 |
| [`system-prompt-value-range-native-host-error.md`](../system-prompts/system-prompt-value-range-native-host-error.md) | Native host validation error indicating a value is outside the allowed numeric range. | 45 | 2.0.70 | 2.0.70 |
| [`system-prompt-not-an-object-native-host-error.md`](../system-prompts/system-prompt-not-an-object-native-host-error.md) | Native host error log stating the given value is not an Object. | 41 | 2.0.70 | 2.0.70 |
| [`system-prompt-fix-path-for-native-install.md`](../system-prompts/system-prompt-fix-path-for-native-install.md) | Adds a native install directory to PATH via an export line appended to a file. | 44 | 2.0.68 | 2.0.68 |
| [`system-prompt-background-task-running-notice.md`](../system-prompts/system-prompt-background-task-running-notice.md) | Informs background task started, gives monitoring path/ID, and resume command format. | 60 | 2.0.66 | 2.0.77 |
| [`system-prompt-dev-conversation-summary-2.md`](../system-prompts/system-prompt-dev-conversation-summary-2.md) | Multiple prompts (2) | 1,262 | 2.0.65 | 2.0.77 |
| [`system-prompt-enter-plan-mode-guidance.md`](../system-prompts/system-prompt-enter-plan-mode-guidance.md) | Advises entering plan mode for non-trivial implementations to get user approval first. | 1,019 | 2.0.62 | 2.0.62 |
| [`system-prompt-sandbox-tmpdir-temporary-files.md`](../system-prompts/system-prompt-sandbox-tmpdir-temporary-files.md) | Describes sandbox command usage restrictions and TMPDIR-based handling for temporary files. | 125 | 2.0.62 | 2.0.62 |
| [`system-prompt-fix-missing-executable-name.md`](../system-prompts/system-prompt-fix-missing-executable-name.md) | Advise fixes when a specified CLI subcommand executable path is missing. | 76 | 2.0.62 | 2.0.62 |
| [`system-prompt-update-session-notes-file-3.md`](../system-prompts/system-prompt-update-session-notes-file-3.md) | Update session notes file via Edit tool while preserving exact section structure. | 762 | 2.0.58 | 2.0.58 |
| [`system-prompt-session-notes-section-template-2.md`](../system-prompts/system-prompt-session-notes-section-template-2.md) | Defines the required sections and guiding questions for session notes. | 294 | 2.0.58 | 2.0.58 |
| [`system-prompt-read-only-architecture-planning-2.md`](../system-prompts/system-prompt-read-only-architecture-planning-2.md) | Explore codebase and produce implementation plans without modifying files. | 625 | 2.0.56 | 2.0.56 |
| [`system-prompt-read-only-codebase-search.md`](../system-prompts/system-prompt-read-only-codebase-search.md) | System variant for read-only file searching and code analysis. | 482 | 2.0.56 | 2.0.56 |
| [`system-prompt-verify-stop-condition-json.md`](../system-prompts/system-prompt-verify-stop-condition-json.md) | Verify plan completion via transcript and code inspection, then output ok using specified tool. | 121 | 2.0.56 | 2.0.68 |
| [`system-prompt-json-io-errors.md`](../system-prompts/system-prompt-json-io-errors.md) | Define tool JSON input fields and exit-code based error handling. | 80 | 2.0.56 | 2.0.56 |
| [`system-prompt-use-current-user-config-extra.md`](../system-prompts/system-prompt-use-current-user-config-extra.md) | Incorporate user environment configuration details and proactively recommend configured features when relevant. | 59 | 2.0.56 | 2.0.56 |
| [`system-prompt-create-shell-snapshot-file-3.md`](../system-prompts/system-prompt-create-shell-snapshot-file-3.md) | Writes a snapshot script file, clears aliases, injects dynamic sections, and verifies output exists | 241 | 2.0.50 | 2.0.50 |
| [`system-prompt-session-title-branch-namer.md`](../system-prompts/system-prompt-session-title-branch-namer.md) | Generates a concise coding session title and matching claude prefixed git branch name. | 369 | 2.0.45 | 2.0.45 |
| [`system-prompt-summarize-new-messages.md`](../system-prompts/system-prompt-summarize-new-messages.md) | Summarizes new conversation messages into a short tagged summary or returns empty if unchanged. | 110 | 2.0.45 | 2.0.45 |
| [`system-prompt-azure-workload-identity-error.md`](../system-prompts/system-prompt-azure-workload-identity-error.md) | Explains missing Azure workload identity parameters and required environment variables with a troubleshooting link. | 108 | 2.0.45 | 2.0.45 |
| [`system-prompt-hook-json-allow-deny.md`](../system-prompts/system-prompt-hook-json-allow-deny.md) | Specifies JSON input and output contract for a hook decision to allow or deny a command. | 61 | 2.0.45 | 2.0.45 |
| [`system-prompt-plan-mode-restrictions.md`](../system-prompts/system-prompt-plan-mode-restrictions.md) | Plan-only mode: edit existing plan file at … via … only | 221 | 2.0.43 | 2.0.43 |
| [`system-prompt-handle-truncated-output.md`](../system-prompts/system-prompt-handle-truncated-output.md) | Handle MCP output truncation by paging/filtering retrieval or warning results may be incomplete. | 68 | 2.0.43 | 2.0.43 |
| [`system-prompt-start-coding-after-plan-approval.md`](../system-prompts/system-prompt-start-coding-after-plan-approval.md) | Proceed with coding after plan approval; update todos and reference saved plan content | 59 | 2.0.43 | 2.0.43 |
| [`system-prompt-json-command-io-exit-codes.md`](../system-prompts/system-prompt-json-command-io-exit-codes.md) | Multiple prompts (2) | 46 | 2.0.43 | 2.0.44 |
| [`system-prompt-json-only-hook-evaluation.md`](../system-prompts/system-prompt-json-only-hook-evaluation.md) | Instruction to return a single valid JSON verdict for a hook condition. | 137 | 2.0.41 | 2.0.41 |
| [`system-prompt-exit-transcript-rules.md`](../system-prompts/system-prompt-exit-transcript-rules.md) | Specifies how stdout and stderr are displayed for tool call inputs and responses by exit code. | 69 | 2.0.41 | 2.0.41 |
| [`system-prompt-require-mcp-cli-info-before-call-2.md`](../system-prompts/system-prompt-require-mcp-cli-info-before-call-2.md) | System instruction to run mcp-cli info before any mcp-cli tool call. | 1,298 | 2.0.36 | 2.0.77 |
| [`system-prompt-require-mcp-cli-info-before-call.md`](../system-prompts/system-prompt-require-mcp-cli-info-before-call.md) | Enforces running mcp-cli info before any tool call to confirm parameters. | 1,269 | 2.0.36 | 2.0.75 |
| [`system-prompt-json-command-exit-handling.md`](../system-prompts/system-prompt-json-command-exit-handling.md) | Specifies JSON command input and stdout or stderr display by exit code. | 40 | 2.0.36 | 2.0.36 |
| [`system-prompt-avoid-disabling-sandbox.md`](../system-prompts/system-prompt-avoid-disabling-sandbox.md) | Enforce sandboxed command execution; only disable sandbox upon explicit request or proven need. | 453 | 2.0.34 | 2.0.34 |
| [`system-prompt-check-mcp-cli-installed.md`](../system-prompts/system-prompt-check-mcp-cli-installed.md) | Append shell snippet to snapshot file, aliasing mcp-cli if unavailable. | 90 | 2.0.34 | 2.0.34 |
| [`system-prompt-hook-json-validation-failure.md`](../system-prompts/system-prompt-hook-json-validation-failure.md) | Report hook JSON output validation failure, showing error, expected schema, and stdout | 37 | 2.0.32 | 2.0.77 |
| [`system-prompt-update-magic-doc-file.md`](../system-prompts/system-prompt-update-magic-doc-file.md) | Update Magic Doc at … with new user insights, preserving header and formatting rules. | 711 | 2.0.30 | 2.0.30 |
| [`system-prompt-exit-plan-mode-to.md`](../system-prompts/system-prompt-exit-plan-mode-to.md) | Directs using an action to exit planning only after an unambiguous implementation plan is complete. | 354 | 2.0.30 | 2.0.30 |
| [`system-prompt-document-specific-update.md`](../system-prompts/system-prompt-document-specific-update.md) | Follow document author’s specific update instructions verbatim, overriding general modification rules. | 65 | 2.0.30 | 2.0.30 |
| [`system-prompt-sandbox-required-for-commands.md`](../system-prompts/system-prompt-sandbox-required-for-commands.md) | Requires all commands to run in sandbox mode and disallows bypassing it. | 63 | 2.0.30 | 2.0.30 |
| [`system-prompt-snapshot-functions-base64-encode.md`](../system-prompts/system-prompt-snapshot-functions-base64-encode.md) | Captures user functions by base64 encoding definitions and writing eval restore lines. | 196 | 2.0.24 | 2.0.24 |
| [`system-prompt-snapshot-functions-typeset-dump.md`](../system-prompts/system-prompt-snapshot-functions-typeset-dump.md) | Captures user function definitions via typeset and writes them directly to the snapshot. | 106 | 2.0.24 | 2.0.24 |
| [`system-prompt-authorized-security-testing-guidelines.md`](../system-prompts/system-prompt-authorized-security-testing-guidelines.md) | Allow defensive and authorized security work while refusing malicious or destructive requests. | 91 | 2.0.24 | 2.0.24 |
| [`system-prompt-detect-new-topic-title-2.md`](../system-prompts/system-prompt-detect-new-topic-title-2.md) | Detects whether a message starts a new topic and outputs a JSON title. | 101 | 2.0.22 | 2.0.22 |
| [`system-prompt-subagent-context-boundaries.md`](../system-prompts/system-prompt-subagent-context-boundaries.md) | Clarifies sub-agent context boundaries and limits actions to assigned task and available messages. | 114 | 2.0.8 | 2.0.8 |
| [`system-prompt-read-local-files-by-path.md`](../system-prompts/system-prompt-read-local-files-by-path.md) | Reads local filesystem files by absolute path with optional line ranges and image viewing. | 411 | 2.0.2 | 2.0.2 |
| [`system-prompt-cli-identity-2.md`](../system-prompts/system-prompt-cli-identity-2.md) | Defines Claude Code as Anthropic's official CLI running in the agent SDK. | 21 | 1.0.128 | 1.0.128 |
| [`system-prompt-frustration-and-pr-detection.md`](../system-prompts/system-prompt-frustration-and-pr-detection.md) | Analyze conversation to output frustration and explicit GitHub pull request send intent flags. | 220 | 1.0.122 | 1.0.122 |
| [`system-prompt-detect-interaction-features.md`](../system-prompts/system-prompt-detect-interaction-features.md) | Instruction to analyze user messages to detect interaction features. | 16 | 1.0.122 | 2.0.22 |
| [`system-prompt-create-md-guide-2.md`](../system-prompts/system-prompt-create-md-guide-2.md) | Analyze the repo and draft or improve a CLAUDE.md with commands and architecture. | 381 | 1.0.112 | 1.0.112 |
| [`system-prompt-dev-conversation-summary.md`](../system-prompts/system-prompt-dev-conversation-summary.md) | Produce a chronological, technically detailed conversation summary with analysis wrapped in tags. | 1,273 | 1.0.103 | 2.0.77 |
| [`system-prompt-command-purpose-in-words.md`](../system-prompts/system-prompt-command-purpose-in-words.md) | Guidelines to describe a shell command’s function in a fixed word range with examples. | 80 | 1.0.102 | 1.0.102 |
| [`system-prompt-structured-coding-todo-list.md`](../system-prompts/system-prompt-structured-coding-todo-list.md) | Guide creating and updating a structured todo list for complex coding sessions. | 2,433 | 1.0.89 | 1.0.89 |
| [`system-prompt-github-issue-title-generator.md`](../system-prompts/system-prompt-github-issue-title-generator.md) | Generates a concise technical GitHub issue title from a bug report. | 254 | 1.0.89 | 1.0.89 |
| [`system-prompt-json-command-exit-rules.md`](../system-prompts/system-prompt-json-command-exit-rules.md) | Defines JSON input and exit code handling for a command, showing stderr only on failure. | 34 | 1.0.85 | 1.0.85 |
| [`system-prompt-fix-settings-json-validation.md`](../system-prompts/system-prompt-fix-settings-json-validation.md) | Analyze Claude Code settings.json validation failure using provided error text and schema, no env changes. | 45 | 1.0.82 | 1.0.82 |
| [`system-prompt-learn-by-doing-human-input.md`](../system-prompts/system-prompt-learn-by-doing-human-input.md) | Request 3–5 line human code contributions for key logic, tracked via TodoList prompts. | 1,137 | 1.0.78 | 1.0.86 |
| [`system-prompt-cli-educational-engineering-insights.md`](../system-prompts/system-prompt-cli-educational-engineering-insights.md) | CLI engineering assistant adds codebase-specific insights before and after coding in formatted blocks | 220 | 1.0.78 | 2.0.67 |
| [`system-prompt-simple-conversation-title-2.md`](../system-prompts/system-prompt-simple-conversation-title-2.md) | Generate a NUM–NUM word conversation title using the last EXPR_1 of EXPR_2 messages. | 60 | 1.0.77 | 2.0.77 |
| [`system-prompt-relay-user-message-context.md`](../system-prompts/system-prompt-relay-user-message-context.md) | Address the user’s provided message and continue ongoing tasks accordingly. | 25 | 1.0.73 | 2.0.77 |
| [`system-prompt-create-statusline-setup-task.md`](../system-prompts/system-prompt-create-statusline-setup-task.md) | Creates a task that invokes the statusline setup subagent. | 31 | 1.0.72 | 1.0.72 |
| [`system-prompt-export-aliases-filter-winpty.md`](../system-prompts/system-prompt-export-aliases-filter-winpty.md) | Writes aliases into the snapshot while filtering winpty aliases on Windows. | 218 | 1.0.65 | 1.0.65 |
| [`system-prompt-record-shell-options-snapshot.md`](../system-prompts/system-prompt-record-shell-options-snapshot.md) | Appends current shell options and enables expand_aliases in the snapshot. | 100 | 1.0.65 | 1.0.65 |
| [`system-prompt-check-rg-and-alias.md`](../system-prompts/system-prompt-check-rg-and-alias.md) | Append snapshot logic to check for rg command and define a fallback alias. | 82 | 1.0.65 | 1.0.65 |
| [`system-prompt-command-json-exit-handling.md`](../system-prompts/system-prompt-command-json-exit-handling.md) | Rules for JSON command input and exit code output handling. | 40 | 1.0.64 | 1.0.64 |
| [`system-prompt-implementation-insights.md`](../system-prompts/system-prompt-implementation-insights.md) | Enforces brief pre/post code educational insights using a named insight banner format. | 134 | 1.0.63 | 2.0.77 |
| [`system-prompt-command-exit-handling.md`](../system-prompts/system-prompt-command-exit-handling.md) | Defines JSON input expectations and exit code behaviors. | 59 | 1.0.55 | 1.0.56 |
| [`system-prompt-exit-handling.md`](../system-prompts/system-prompt-exit-handling.md) | Defines stdout and stderr visibility rules based on command exit code for tool calls. | 62 | 1.0.53 | 1.0.53 |
| [`system-prompt-compaction-command-exit-codes.md`](../system-prompts/system-prompt-compaction-command-exit-codes.md) | Defines JSON input handling and exit-code behavior for compaction commands. | 55 | 1.0.53 | 1.0.53 |
| [`system-prompt-handle-exit-codes-and-output.md`](../system-prompts/system-prompt-handle-exit-codes-and-output.md) | Routes stdout and stderr visibility based on exit code and continues execution when needed. | 49 | 1.0.53 | 1.0.53 |
| [`system-prompt-exit-output-handling.md`](../system-prompts/system-prompt-exit-output-handling.md) | Route stdout and stderr visibility based on exit codes. | 45 | 1.0.53 | 1.0.53 |
| [`system-prompt-redirect-detected.md`](../system-prompts/system-prompt-redirect-detected.md) | Request WebFetch rerun to retrieve content from redirected host URL with new parameters. | 97 | 1.0.52 | 2.0.15 |
| [`system-prompt-install-github-app.md`](../system-prompts/system-prompt-install-github-app.md) | Explains adding a workflow to enable Claude Code via @claude mentions after merge. | 393 | 1.0.44 | 1.0.44 |
| [`system-prompt-github-permission-troubleshooting.md`](../system-prompts/system-prompt-github-permission-troubleshooting.md) | Provide quick fixes for common GitHub CLI permission and authorization issues. | 54 | 1.0.28 | 1.0.28 |
| [`system-prompt-github-repo-access-help.md`](../system-prompts/system-prompt-github-repo-access-help.md) | List common GitHub CLI repository access errors and the steps to resolve them. | 52 | 1.0.28 | 1.0.28 |
| [`system-prompt-verify-repo-access-and-scope.md`](../system-prompts/system-prompt-verify-repo-access-and-scope.md) | Validate GitHub repository name, access permissions, and token scopes for private repos. | 61 | 1.0.25 | 2.0.41 |
| [`system-prompt-list-mcp-server-resources.md`](../system-prompts/system-prompt-list-mcp-server-resources.md) | Lists available resources across MCP servers with optional server filtering. | 73 | 1.0.22 | 1.0.22 |
| [`system-prompt-read-mcp-server-resource.md`](../system-prompts/system-prompt-read-mcp-server-resource.md) | Reads a resource from an MCP server by server name and URI. | 73 | 1.0.22 | 1.0.22 |
| [`system-prompt-avoid-rereading-unchanged-resource.md`](../system-prompts/system-prompt-avoid-rereading-unchanged-resource.md) | Instructs to not reread a resource unless it may have changed. | 22 | 1.0.19 | 1.0.19 |
| [`system-prompt-replace-all-occurrences-warning.md`](../system-prompts/system-prompt-replace-all-occurrences-warning.md) | Warns about multiple replacement matches when replace_all is false, requesting unique context. | 61 | 1.0.18 | 2.0.15 |
| [`system-prompt-extract-displayed-file-paths.md`](../system-prompts/system-prompt-extract-displayed-file-paths.md) | Identify and return only explicitly shown file paths when file contents are displayed. | 289 | 1.0.8 | 1.0.8 |
| [`system-prompt-exact-string-edits-in-files.md`](../system-prompts/system-prompt-exact-string-edits-in-files.md) | Define rules for exact in-file string replacements after reading and with unique matches. | 258 | 1.0.8 | 1.0.8 |
| [`system-prompt-write-file-with-constraints.md`](../system-prompts/system-prompt-write-file-with-constraints.md) | Defines rules for writing files, including reading before overwriting and avoiding new docs. | 145 | 1.0.7 | 1.0.7 |
| [`system-prompt-install-github-cli.md`](../system-prompts/system-prompt-install-github-cli.md) | Install GitHub CLI across macOS, Windows, and Linux. | 41 | 1.0.0 | 1.0.0 |
| [`system-prompt-admin-setup-secrets-apps.md`](../system-prompts/system-prompt-admin-setup-secrets-apps.md) | Have a repository admin install apps and configure secrets when setup fails. | 33 | 1.0.0 | 1.0.0 |
| [`system-prompt-use-owner-path-format.md`](../system-prompts/system-prompt-use-owner-path-format.md) | Use the owner and path or URL format for repository references. | 28 | 1.0.0 | 1.0.0 |
| [`system-prompt-authenticate-with-gh-cli.md`](../system-prompts/system-prompt-authenticate-with-gh-cli.md) | Authenticate to GitHub using gh auth login or environment-based methods. | 25 | 1.0.0 | 1.0.0 |
| [`system-prompt-summarize-conversations.md`](../system-prompts/system-prompt-summarize-conversations.md) | Directs the assistant to summarize conversations. | 13 | 0.2.108 | 2.0.22 |
| [`system-prompt-web-search.md`](../system-prompts/system-prompt-web-search.md) | Sets the assistant to perform web search tool use. | 11 | 0.2.108 | 2.0.22 |
| [`system-prompt-summarize-coding-chat-status.md`](../system-prompts/system-prompt-summarize-coding-chat-status.md) | Condense a coding conversation into a character-limited status recap. | 33 | 0.2.91 | 0.2.91 |
| [`system-prompt-create-view-instrument-selector.md`](../system-prompts/system-prompt-create-view-instrument-selector.md) | Create a new view with specified name, optional description, and InstrumentSelector variants. | 110 | 0.2.76 | 0.2.76 |
| [`system-prompt-nested-template-functions.md`](../system-prompts/system-prompt-nested-template-functions.md) | Nested compiled template functions that concatenate output into a string buffer. | 134 | 0.2.54 | 1.0.86 |
| [`system-prompt-select-core-frequently-modified-files.md`](../system-prompts/system-prompt-select-core-frequently-modified-files.md) | Choose five diverse frequently modified core-logic filenames from git history stats. | 90 | 0.2.9 | 0.2.9 |
| [`system-prompt-classify-bash-command-prefix.md`](../system-prompts/system-prompt-classify-bash-command-prefix.md) | Determine the appropriate prefix for bash commands requested by a coding agent. | 33 | 0.2.9 | 0.2.9 |

## Tool prompts (113)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`tool-description-run-bash-commands-safely.md`](../system-prompts/tool-description-run-bash-commands-safely.md) | Run bash commands in persistent shell, verifying directories and quoting paths safely. | 995 | 2.0.77 | 2.0.77 |
| [`tool-description-request-plan-approval.md`](../system-prompts/tool-description-request-plan-approval.md) | Use a tool to signal planning finished and request user approval, without including plan content. | 431 | 2.0.77 | 2.0.77 |
| [`tool-description-ask-user-clarifying-questions.md`](../system-prompts/tool-description-ask-user-clarifying-questions.md) | Tool guidance for asking users questions to clarify requirements during execution. | 207 | 2.0.77 | 2.0.77 |
| [`tool-description-enable-or-view-plan.md`](../system-prompts/tool-description-enable-or-view-plan.md) | Toggles plan mode or displays the current session plan. | 9 | 2.0.77 | 2.0.77 |
| [`tool-description-update-or-resolve-task.md`](../system-prompts/tool-description-update-or-resolve-task.md) | Describes updating task fields, adding context, and marking tasks resolved when finished. | 413 | 2.0.74 | 2.0.74 |
| [`tool-description-create-tracked-task.md`](../system-prompts/tool-description-create-tracked-task.md) | Defines how to create a new task with a clear subject and detailed description. | 169 | 2.0.74 | 2.0.74 |
| [`tool-description-lsp-intelligence-operations-2.md`](../system-prompts/tool-description-lsp-intelligence-operations-2.md) | Use LSP to navigate symbols, references, hover, and call hierarchy in code. | 267 | 2.0.73 | 2.0.73 |
| [`tool-description-list-available-skills.md`](../system-prompts/tool-description-list-available-skills.md) | Display the set of available skills. | 3 | 2.0.73 | 2.0.73 |
| [`tool-description-deprecated-structured-todo-list.md`](../system-prompts/tool-description-deprecated-structured-todo-list.md) | Deprecated tool notice describing replacement task tools and when to use task lists. | 2,520 | 2.0.72 | 2.0.72 |
| [`tool-description-configure-extra-usage-keep-working.md`](../system-prompts/tool-description-configure-extra-usage-keep-working.md) | Configure extra usage to keep working when limits are hit. | 10 | 2.0.72 | 2.0.72 |
| [`tool-description-show-qr-download-mobile-app.md`](../system-prompts/tool-description-show-qr-download-mobile-app.md) | Show a QR code to download the Claude mobile app. | 10 | 2.0.72 | 2.0.72 |
| [`tool-description-chrome-beta-settings.md`](../system-prompts/tool-description-chrome-beta-settings.md) | Label for the Claude in Chrome beta settings page. | 7 | 2.0.72 | 2.0.72 |
| [`tool-description-browser-mouse-keyboard-control.md`](../system-prompts/tool-description-browser-mouse-keyboard-control.md) | Interact with the browser via mouse and keyboard using screenshots for accurate clicking. | 154 | 2.0.71 | 2.0.71 |
| [`tool-description-record-and-export-gif.md`](../system-prompts/tool-description-record-and-export-gif.md) | Record browser actions and export an annotated animated GIF. | 143 | 2.0.71 | 2.0.71 |
| [`tool-description-find-page-elements.md`](../system-prompts/tool-description-find-page-elements.md) | Locate page elements by natural-language purpose or text and return reusable references. | 112 | 2.0.71 | 2.0.71 |
| [`tool-description-read-browser-console-messages.md`](../system-prompts/tool-description-read-browser-console-messages.md) | Fetch filtered console messages from a tab for debugging. | 102 | 2.0.71 | 2.0.71 |
| [`tool-description-get-accessibility-tree.md`](../system-prompts/tool-description-get-accessibility-tree.md) | Return an accessibility tree snapshot with options to limit scope and output size. | 97 | 2.0.71 | 2.0.71 |
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
| [`tool-description-mcp-loader-selector.md`](../system-prompts/tool-description-mcp-loader-selector.md) | Discover and load MCP tools by direct selection or keyword search before use. | 511 | 2.0.70 | 2.0.70 |
| [`tool-description-get-task-details-by-id-2.md`](../system-prompts/tool-description-get-task-details-by-id-2.md) | Fetches full task details, comments, and dependency context by task ID. | 222 | 2.0.70 | 2.0.70 |
| [`tool-description-chrome-native-host-log.md`](../system-prompts/tool-description-chrome-native-host-log.md) | Format timestamped Claude Chrome Native Host log prefix with message and optional suffix. | 26 | 2.0.70 | 2.0.72 |
| [`tool-description-explore-features-progress-tracker.md`](../system-prompts/tool-description-explore-features-progress-tracker.md) | Entry point to explore Claude Code features and track progress. | 9 | 2.0.70 | 2.0.70 |
| [`tool-description-year-in-review-header.md`](../system-prompts/tool-description-year-in-review-header.md) | Title string for a Claude Code year in review. | 12 | 2.0.66 | 2.0.66 |
| [`tool-description-play-thinkback-animation.md`](../system-prompts/tool-description-play-thinkback-animation.md) | Trigger playback of the thinkback animation. | 6 | 2.0.66 | 2.0.66 |
| [`tool-description-get-task-output-status.md`](../system-prompts/tool-description-get-task-output-status.md) | Fetches task output and status with optional blocking for completion. | 104 | 2.0.65 | 2.0.65 |
| [`tool-description-toggle-session-search-tag.md`](../system-prompts/tool-description-toggle-session-search-tag.md) | Toggles a searchable tag on the current session. | 9 | 2.0.65 | 2.0.65 |
| [`tool-description-show-usage-stats.md`](../system-prompts/tool-description-show-usage-stats.md) | Display Claude Code usage statistics and activity. | 8 | 2.0.63 | 2.0.63 |
| [`tool-description-show-current-context-usage.md`](../system-prompts/tool-description-show-current-context-usage.md) | Display current context usage information. | 4 | 2.0.63 | 2.0.63 |
| [`tool-description-enter-plan-mode-signoff.md`](../system-prompts/tool-description-enter-plan-mode-signoff.md) | Advises entering plan mode to propose an implementation approach and get approval. | 1,023 | 2.0.62 | 2.0.62 |
| [`tool-description-fetch-and-analyze-web-content.md`](../system-prompts/tool-description-fetch-and-analyze-web-content.md) | Describes a tool that fetches a URL, converts HTML to markdown, and analyzes it with a small model. | 259 | 2.0.62 | 2.0.62 |
| [`tool-description-install-slack-app.md`](../system-prompts/tool-description-install-slack-app.md) | Instruction to install the Claude Slack app. | 6 | 2.0.62 | 2.0.62 |
| [`tool-description-share-free-week-invite.md`](../system-prompts/tool-description-share-free-week-invite.md) | Offers an option to share a free week of Claude Code with friends. | 9 | 2.0.58 | 2.0.58 |
| [`tool-description-web-search-with-mandatory-sources.md`](../system-prompts/tool-description-web-search-with-mandatory-sources.md) | Search the web with current year and append mandatory Sources links section. | 338 | 2.0.56 | 2.0.56 |
| [`tool-description-configure-default-remote-environment.md`](../system-prompts/tool-description-configure-default-remote-environment.md) | Set the default remote environment for teleport sessions. | 9 | 2.0.47 | 2.0.47 |
| [`tool-description-structured-final-output.md`](../system-prompts/tool-description-structured-final-output.md) | Require a single tool call to return the final structured response. | 34 | 2.0.43 | 2.0.43 |
| [`tool-description-return-verification-result.md`](../system-prompts/tool-description-return-verification-result.md) | Require a single tool call to output the verification result at the end. | 24 | 2.0.43 | 2.0.43 |
| [`tool-description-rate-limit-options.md`](../system-prompts/tool-description-rate-limit-options.md) | Display available options when a rate limit is reached. | 7 | 2.0.43 | 2.0.43 |
| [`tool-description-rename-conversation.md`](../system-prompts/tool-description-rename-conversation.md) | Renames the current conversation. | 5 | 2.0.41 | 2.0.41 |
| [`tool-description-order-stickers.md`](../system-prompts/tool-description-order-stickers.md) | Requests placing an order for Claude Code stickers. | 5 | 2.0.32 | 2.0.32 |
| [`tool-description-configure-expression.md`](../system-prompts/tool-description-configure-expression.md) | Show two expressions and prompt to press Enter to configure them. | 20 | 2.0.24 | 2.0.24 |
| [`tool-description-manage-plugins.md`](../system-prompts/tool-description-manage-plugins.md) | Manage plugins for Claude Code. | 5 | 2.0.12 | 2.0.12 |
| [`tool-description-read-local-file-path.md`](../system-prompts/tool-description-read-local-file-path.md) | Tool description for reading local files by absolute path with truncation limits. | 415 | 2.0.2 | 2.0.2 |
| [`tool-description-fast-glob-file-matching-2.md`](../system-prompts/tool-description-fast-glob-file-matching-2.md) | Glob-based file matcher returning paths sorted by modification time and supports batching searches. | 115 | 2.0.2 | 2.0.2 |
| [`tool-description-restore-previous-state.md`](../system-prompts/tool-description-restore-previous-state.md) | Restores code and/or conversation to an earlier point. | 12 | 2.0.2 | 2.0.2 |
| [`tool-description-show-plan-usage-limits.md`](../system-prompts/tool-description-show-plan-usage-limits.md) | Display plan usage and limits. | 4 | 2.0.0 | 2.0.0 |
| [`tool-description-view-update-privacy-settings.md`](../system-prompts/tool-description-view-update-privacy-settings.md) | View and update privacy settings. | 6 | 1.0.96 | 1.0.96 |
| [`tool-description-list-todo-items.md`](../system-prompts/tool-description-list-todo-items.md) | Requests listing the current todo items. | 4 | 1.0.94 | 1.0.94 |
| [`tool-description-context-usage-grid.md`](../system-prompts/tool-description-context-usage-grid.md) | Renders current context usage as a colored grid visualization. | 10 | 1.0.86 | 1.0.86 |
| [`tool-description-collaborative-learning-cli.md`](../system-prompts/tool-description-collaborative-learning-cli.md) | Interactive CLI that blends task completion with learning by requesting meaningful human code contributions. | 1,009 | 1.0.78 | 2.0.32 |
| [`tool-description-educational-cli-engineering-help.md`](../system-prompts/tool-description-educational-cli-engineering-help.md) | Interactive CLI for engineering tasks with educational codebase insights under an explanatory style. | 92 | 1.0.78 | 2.0.32 |
| [`tool-description-set-output-style-menu.md`](../system-prompts/tool-description-set-output-style-menu.md) | Instruction to set the output style directly or via a selection menu. | 10 | 1.0.78 | 1.0.78 |
| [`tool-description-bus-error-message.md`](../system-prompts/tool-description-bus-error-message.md) | Reports a bus error from misaligned or invalid memory access. | 16 | 1.0.68 | 1.0.68 |
| [`tool-description-paused-by-ctrl-z-or-suspend.md`](../system-prompts/tool-description-paused-by-ctrl-z-or-suspend.md) | Marks the process as stopped via job-control suspend. | 12 | 1.0.68 | 1.0.68 |
| [`tool-description-child-process-state-change.md`](../system-prompts/tool-description-child-process-state-change.md) | Multiple prompts (2) | 10 | 1.0.68 | 1.0.68 |
| [`tool-description-ctrl-break-interruption.md`](../system-prompts/tool-description-ctrl-break-interruption.md) | Indicates the user interrupted execution with CTRL-BREAK. | 9 | 1.0.68 | 1.0.68 |
| [`tool-description-emulated-command-not-implemented.md`](../system-prompts/tool-description-emulated-command-not-implemented.md) | Indicates a command is expected to be emulated but has no implementation. | 9 | 1.0.68 | 1.0.68 |
| [`tool-description-application-specific-realtime-signal.md`](../system-prompts/tool-description-application-specific-realtime-signal.md) | Denotes receipt of an application-defined realtime signal. | 8 | 1.0.68 | 2.0.72 |
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
| [`tool-description-kill-background-bash-shell.md`](../system-prompts/tool-description-kill-background-bash-shell.md) | Terminate a running background bash shell by shell id and return status. | 65 | 1.0.60 | 1.0.113 |
| [`tool-description-manage-configurations.md`](../system-prompts/tool-description-manage-configurations.md) | Create and maintain agent configuration settings. | 4 | 1.0.60 | 1.0.60 |
| [`tool-description-verify-setup.md`](../system-prompts/tool-description-verify-setup.md) | Diagnoses and verifies Claude Code installation and configuration settings. | 11 | 1.0.49 | 1.0.49 |
| [`tool-description-export-conversation-to-file.md`](../system-prompts/tool-description-export-conversation-to-file.md) | Export the current conversation to a file or clipboard. | 9 | 1.0.44 | 1.0.44 |
| [`tool-description-ripgrep-search-guidelines.md`](../system-prompts/tool-description-ripgrep-search-guidelines.md) | Guidelines for using the Grep search tool with regex, filters, and output modes. | 250 | 1.0.38 | 1.0.38 |
| [`tool-description-manage-hook-configurations.md`](../system-prompts/tool-description-manage-hook-configurations.md) | Tool description for managing hook configurations for tool events. | 7 | 1.0.38 | 1.0.38 |
| [`tool-description-install-native-build.md`](../system-prompts/tool-description-install-native-build.md) | Install the native build of Claude Code. | 5 | 1.0.31 | 1.0.31 |
| [`tool-description-resume-conversation-session.md`](../system-prompts/tool-description-resume-conversation-session.md) | Requests resuming a prior conversation. | 3 | 1.0.26 | 1.0.26 |
| [`tool-description-add-working-directory.md`](../system-prompts/tool-description-add-working-directory.md) | Add a new working directory. | 5 | 1.0.23 | 1.0.23 |
| [`tool-description-list-configured-mcp-resources.md`](../system-prompts/tool-description-list-configured-mcp-resources.md) | Tool to list MCP resources from all or a specified server including server field. | 74 | 1.0.22 | 1.0.22 |
| [`tool-description-read-resource-by-uri.md`](../system-prompts/tool-description-read-resource-by-uri.md) | Tool to read an MCP resource by server name and resource URI. | 54 | 1.0.22 | 1.0.22 |
| [`tool-description-upgrade-to-max-rate-limits.md`](../system-prompts/tool-description-upgrade-to-max-rate-limits.md) | Promotes upgrading to Max to get higher rate limits and more Opus access. | 12 | 1.0.11 | 1.0.11 |
| [`tool-description-exact-file-string-replacement.md`](../system-prompts/tool-description-exact-file-string-replacement.md) | Describes exact in-file replacement tool rules, requiring prior read and unique old_string. | 263 | 1.0.8 | 1.0.8 |
| [`tool-description-write-file-after-reading-existing.md`](../system-prompts/tool-description-write-file-after-reading-existing.md) | Write files, reading existing contents first, and avoid unrequested new or documentation files. | 150 | 1.0.7 | 1.0.9 |
| [`tool-description-manage-permissions.md`](../system-prompts/tool-description-manage-permissions.md) | Controls allow and deny rules for tool permissions. | 8 | 1.0.7 | 1.0.7 |
| [`tool-description-show-status-details.md`](../system-prompts/tool-description-show-status-details.md) | Command to display Claude Code status, version, model, connectivity, and tools. | 18 | 1.0.4 | 1.0.4 |
| [`tool-description-set.md`](../system-prompts/tool-description-set.md) | Set the Claude Code model selection. | 7 | 1.0.0 | 1.0.0 |
| [`tool-description-manage-ide-integrations-status.md`](../system-prompts/tool-description-manage-ide-integrations-status.md) | Manage IDE MCP integrations and display their status. | 8 | 0.2.126 | 1.0.0 |
| [`tool-description-list-manage-background-tasks.md`](../system-prompts/tool-description-list-manage-background-tasks.md) | List and manage background tasks. | 5 | 0.2.117 | 2.0.45 |
| [`tool-description-setup-github-actions.md`](../system-prompts/tool-description-setup-github-actions.md) | Sets up Claude GitHub Actions integration for a repository. | 8 | 0.2.101 | 0.2.101 |
| [`tool-description-option-enter-newline-binding.md`](../system-prompts/tool-description-option-enter-newline-binding.md) | Enable Option+Enter to insert newlines. | 12 | 0.2.80 | 0.2.83 |
| [`tool-description-list-files-in-context.md`](../system-prompts/tool-description-list-files-in-context.md) | List all files currently available in context. | 6 | 0.2.79 | 0.2.79 |
| [`tool-description-clear-chat-keep-summary.md`](../system-prompts/tool-description-clear-chat-keep-summary.md) | Clears conversation history while retaining a summary in context. | 24 | 0.2.54 | 0.2.57 |
| [`tool-description-toggle-vim-editing-mode.md`](../system-prompts/tool-description-toggle-vim-editing-mode.md) | Switch between Vim and normal editing modes. | 8 | 0.2.54 | 0.2.54 |
| [`tool-description-edit-memory-files.md`](../system-prompts/tool-description-edit-memory-files.md) | Edit Claude memory files. | 4 | 0.2.54 | 0.2.54 |
| [`tool-description-replace-jupyter-notebook-cell.md`](../system-prompts/tool-description-replace-jupyter-notebook-cell.md) | Replaces, inserts, or deletes a specific Jupyter notebook cell by index. | 117 | 0.2.9 | 0.2.83 |
| [`tool-description-show-session-cost-and-duration.md`](../system-prompts/tool-description-show-session-cost-and-duration.md) | Displays the current session total cost and duration. | 10 | 0.2.9 | 0.2.9 |
| [`tool-description-sign-in-anthropic-account.md`](../system-prompts/tool-description-sign-in-anthropic-account.md) | Signs in using an Anthropic account. | 8 | 0.2.9 | 0.2.9 |
| [`tool-description-sign-out-anthropic-account.md`](../system-prompts/tool-description-sign-out-anthropic-account.md) | Signs out from an Anthropic account. | 8 | 0.2.9 | 0.2.9 |
| [`tool-description-clear-conversation-history.md`](../system-prompts/tool-description-clear-conversation-history.md) | Clears conversation history to free up context. | 7 | 0.2.9 | 0.2.9 |
| [`tool-description-show-help-and-commands.md`](../system-prompts/tool-description-show-help-and-commands.md) | Displays help text and available commands. | 5 | 0.2.9 | 0.2.9 |
| [`tool-description-submit-feedback.md`](../system-prompts/tool-description-submit-feedback.md) | Submits user feedback about Claude Code. | 5 | 0.2.9 | 1.0.102 |

## Agent prompts (7)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`agent-prompt-convert-psone-to-statusline.md`](../system-prompts/agent-prompt-convert-psone-to-statusline.md) | Converts shell PS1 config into a Claude Code statusLine command with colors preserved. | 1,417 | 2.0.77 | 2.0.77 |
| [`agent-prompt-parallel-transcript-plan-verification.md`](../system-prompts/agent-prompt-parallel-transcript-plan-verification.md) | Verify plan completion by spawning parallel transcript checks and aggregating pass or fail. | 238 | 2.0.77 | 2.0.77 |
| [`agent-prompt-safe-bash-command-execution.md`](../system-prompts/agent-prompt-safe-bash-command-execution.md) | Execute shell and git commands efficiently with clear output and safety checks. | 102 | 2.0.77 | 2.0.77 |
| [`agent-prompt-read-only-architecture-planning-2.md`](../system-prompts/agent-prompt-read-only-architecture-planning-2.md) | Explore the codebase and produce an implementation plan under strict read-only constraints. | 644 | 2.0.56 | 2.0.56 |
| [`agent-prompt-read-only-codebase-search.md`](../system-prompts/agent-prompt-read-only-codebase-search.md) | Search and analyze an existing codebase in strict read-only mode using provided tools. | 503 | 2.0.56 | 2.0.56 |
| [`agent-prompt-use-current-user-config.md`](../system-prompts/agent-prompt-use-current-user-config.md) | Incorporate the user’s current custom environment configuration into relevant answers and suggestions. | 52 | 2.0.56 | 2.0.60 |
| [`agent-prompt-codebase-search-analysis-guide.md`](../system-prompts/agent-prompt-codebase-search-analysis-guide.md) | Guidance for searching and analyzing multiple files in a codebase without creating files. | 287 | 1.0.45 | 2.0.70 |

## System data (145)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-data-update-repo-file-api.md`](../system-prompts/system-data-update-repo-file-api.md) | Template for an API request to update repository file content and branch. | 2,464 | 2.0.77 | 2.0.77 |
| [`system-data-update-repo-file-via-api-2.md`](../system-prompts/system-data-update-repo-file-via-api-2.md) | PUT request template to update repository file content on a branch. | 2,450 | 2.0.77 | 2.0.77 |
| [`system-data-file-matching-glob-rules.md`](../system-prompts/system-data-file-matching-glob-rules.md) | Defines project file listing and glob handling including hidden paths. | 2,377 | 2.0.77 | 2.0.77 |
| [`system-data-search-files-with-globs-4.md`](../system-prompts/system-data-search-files-with-globs-4.md) | Repeated ripgrep file-listing flags with glob exclusions and injected expression segments | 2,372 | 2.0.77 | 2.0.77 |
| [`system-data-search-files-with-globs-3.md`](../system-prompts/system-data-search-files-with-globs-3.md) | Repeated ripgrep file-listing flags with glob exclusions and injected expression segments | 1,131 | 2.0.77 | 2.0.77 |
| [`system-data-progress-verb-word-list.md`](../system-prompts/system-data-progress-verb-word-list.md) | List of whimsical present-participle activity words. | 856 | 2.0.77 | 2.0.77 |
| [`system-data-write-short-conversation-title.md`](../system-prompts/system-data-write-short-conversation-title.md) | Asks for a fixed-length title summarizing the recent conversation. | 728 | 2.0.77 | 2.0.77 |
| [`system-data-outgoing-calls-task-status.md`](../system-prompts/system-data-outgoing-calls-task-status.md) | Displays outgoing calls with task status and a follow-on repo update request. | 694 | 2.0.77 | 2.0.77 |
| [`system-data-write-conversation-title-from-calls.md`](../system-prompts/system-data-write-conversation-title-from-calls.md) | Request to generate a short conversation title after listing outgoing calls and usage. | 646 | 2.0.77 | 2.0.77 |
| [`system-data-outgoing-calls-task-report.md`](../system-prompts/system-data-outgoing-calls-task-report.md) | Formatted outgoing calls listing with task number, status, description, and extra trailing field. | 583 | 2.0.77 | 2.0.77 |
| [`system-data-outgoing-calls-task-status-2.md`](../system-prompts/system-data-outgoing-calls-task-status-2.md) | Formatted report listing outgoing calls with task id, status, and description. | 582 | 2.0.77 | 2.0.77 |
| [`system-data-search-files-with-globs-2.md`](../system-prompts/system-data-search-files-with-globs-2.md) | Repeated ripgrep file-listing flags with glob exclusions and injected expression segments | 579 | 2.0.77 | 2.0.77 |
| [`system-data-outgoing-calls-task-report-2.md`](../system-prompts/system-data-outgoing-calls-task-report-2.md) | Formatted outgoing calls listing with task number, status, description, and extra trailing field. | 576 | 2.0.77 | 2.0.77 |
| [`system-data-outgoing-calls-task-report-3.md`](../system-prompts/system-data-outgoing-calls-task-report-3.md) | Formatted outgoing calls listing with task number, status, description, and extra trailing field. | 576 | 2.0.77 | 2.0.77 |
| [`system-data-search-files-with-globs.md`](../system-prompts/system-data-search-files-with-globs.md) | Repeated ripgrep file-listing flags with glob exclusions and injected expression segments | 565 | 2.0.77 | 2.0.77 |
| [`system-data-multiple-repo-file-updates.md`](../system-prompts/system-data-multiple-repo-file-updates.md) | Three GitHub API PUT calls update repository files with commit message, content, and branch. | 185 | 2.0.77 | 2.0.77 |
| [`system-data-remote-task-notification-output.md`](../system-prompts/system-data-remote-task-notification-output.md) | Remote agent task notification reporting status, summary text, and output file path. | 150 | 2.0.77 | 2.0.77 |
| [`system-data-github-anthropics-path-entries.md`](../system-prompts/system-data-github-anthropics-path-entries.md) | Repeated GitHub host and organization path strings for anthropics. | 137 | 2.0.77 | 2.0.77 |
| [`system-data-task-notification-output-file.md`](../system-prompts/system-data-task-notification-output-file.md) | Browser bridge task notification with pipe task-id, output path, status, and result file pointer. | 125 | 2.0.77 | 2.0.77 |
| [`system-data-conversation-title-generator-variables.md`](../system-prompts/system-data-conversation-title-generator-variables.md) | Multiple prompts (2) | 123 | 2.0.77 | 2.0.77 |
| [`system-data-conversation-title-word-limit.md`](../system-prompts/system-data-conversation-title-word-limit.md) | Writes a fixed-length title for a conversation based on recent messages. | 122 | 2.0.77 | 2.0.77 |
| [`system-data-verify-plan-task-completion.md`](../system-prompts/system-data-verify-plan-task-completion.md) | Verify planned tasks completed by cross-checking transcript, user prompts, and claude-md artifacts. | 102 | 2.0.77 | 2.0.77 |
| [`system-data-put-repo-file-update.md`](../system-prompts/system-data-put-repo-file-update.md) | API PUT request template to update repository content at a path. | 83 | 2.0.77 | 2.0.77 |
| [`system-data-long-numeric-placeholder-list.md`](../system-prompts/system-data-long-numeric-placeholder-list.md) | Provides a long list of numeric placeholders with no added context. | 286 | 2.0.72 | 2.0.72 |
| [`system-data-az-access-token-script.md`](../system-prompts/system-data-az-access-token-script.md) | PowerShell command that fetches an Azure access token and outputs JSON. | 337 | 2.0.71 | 2.0.71 |
| [`system-data-mouse-actions-command-list.md`](../system-prompts/system-data-mouse-actions-command-list.md) | List of supported UI actions including clicks, typing, scrolling, keys, and screenshots. | 244 | 2.0.71 | 2.0.71 |
| [`system-data-template-function-compiled-output.md`](../system-prompts/system-data-template-function-compiled-output.md) | Lodash template compiler output embedding passthrough markers and nine injected expression segments. | 126 | 2.0.66 | 2.0.66 |
| [`system-data-common-shell-and-docker-commands.md`](../system-prompts/system-data-common-shell-and-docker-commands.md) | List of common Unix utilities plus Docker ps/images and basic system info commands. | 79 | 2.0.66 | 2.0.66 |
| [`system-data-get-guardrail-response-fields.md`](../system-prompts/system-data-get-guardrail-response-fields.md) | Response fields returned when retrieving a Bedrock guardrail. | 239 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-customization-job-response.md`](../system-prompts/system-data-bedrock-customization-job-response.md) | Model customization job response fields for status, datasets, metrics, and output model details. | 238 | 2.0.63 | 2.0.63 |
| [`system-data-get-provisioned-throughput-response-fields.md`](../system-prompts/system-data-get-provisioned-throughput-response-fields.md) | Provides throughput, ARNs, status, and commitment details for a provisioned model. | 188 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-get-custom-response-fields.md`](../system-prompts/system-data-bedrock-get-custom-response-fields.md) | Field list for GetCustomModelResponse including modelArn, metrics, and status. | 182 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-update-guardrail-request-fields.md`](../system-prompts/system-data-bedrock-update-guardrail-request-fields.md) | Field list for UpdateGuardrailRequest including guardrailIdentifier and policy configs. | 180 | 2.0.63 | 2.0.63 |
| [`system-data-create-guardrail-request-fields.md`](../system-prompts/system-data-create-guardrail-request-fields.md) | Describes configuration fields used to create a Bedrock guardrail. | 180 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-provisioned-summary-fields.md`](../system-prompts/system-data-bedrock-provisioned-summary-fields.md) | Defines attributes included in a Bedrock provisioned model summary. | 175 | 2.0.63 | 2.0.63 |
| [`system-data-automated-reasoning-policy-annotation-actions.md`](../system-prompts/system-data-automated-reasoning-policy-annotation-actions.md) | Action annotations for automated reasoning policy updates and ingestion. | 173 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-get-evaluation-job-response.md`](../system-prompts/system-data-bedrock-get-evaluation-job-response.md) | Evaluation job response fields covering config, encryption, timestamps, and failures. | 173 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-invocation-job-summary.md`](../system-prompts/system-data-bedrock-invocation-job-summary.md) | Fields for Bedrock GetModelInvocationJobResponse job details. | 172 | 2.0.63 | 2.0.77 |
| [`system-data-bedrock-invocation-job-response.md`](../system-prompts/system-data-bedrock-invocation-job-response.md) | Fields for Bedrock GetModelInvocationJobResponse job details. | 171 | 2.0.63 | 2.0.76 |
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
| [`system-data-bedrock-foundation-details.md`](../system-prompts/system-data-bedrock-foundation-details.md) | Foundation model metadata including modalities, streaming support, and lifecycle. | 137 | 2.0.63 | 2.0.77 |
| [`system-data-get-policy-build-workflow-response.md`](../system-prompts/system-data-get-policy-build-workflow-response.md) | Lists fields returned when fetching an automated reasoning policy build workflow. | 136 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-foundation-details-2.md`](../system-prompts/system-data-bedrock-foundation-details-2.md) | Foundation model metadata including modalities, streaming support, and lifecycle. | 135 | 2.0.63 | 2.0.77 |
| [`system-data-invoke-response-stream-request-fields.md`](../system-prompts/system-data-invoke-response-stream-request-fields.md) | Fields for Bedrock runtime InvokeModelWithResponseStream request. | 135 | 2.0.63 | 2.0.63 |
| [`system-data-bedrockruntime-converse-request-fields.md`](../system-prompts/system-data-bedrockruntime-converse-request-fields.md) | Field list for ConverseRequest including modelId, messages, and configs. | 134 | 2.0.63 | 2.0.77 |
| [`system-data-bedrockruntime-converse-request-fields-2.md`](../system-prompts/system-data-bedrockruntime-converse-request-fields-2.md) | Field list for ConverseRequest including modelId, messages, and configs. | 133 | 2.0.63 | 2.0.77 |
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
| [`system-data-bedrock-guardrail-content-filter-config.md`](../system-prompts/system-data-bedrock-guardrail-content-filter-config.md) | Configuration fields for Bedrock guardrail content filtering behavior. | 121 | 2.0.63 | 2.0.77 |
| [`system-data-bedrock-create-policy-test-case-fields.md`](../system-prompts/system-data-bedrock-create-policy-test-case-fields.md) | Field list for CreateAutomatedReasoningPolicyTestCaseRequest including policyArn and expected results. | 120 | 2.0.63 | 2.0.63 |
| [`system-data-bedrock-guardrail-content-filter-config-2.md`](../system-prompts/system-data-bedrock-guardrail-content-filter-config-2.md) | Configuration fields for Bedrock guardrail content filtering behavior. | 120 | 2.0.63 | 2.0.77 |
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
| [`system-data-runtime-environment-info.md`](../system-prompts/system-data-runtime-environment-info.md) | Multiple prompts (2) | 109 | 2.0.50 | 2.0.62 |
| [`system-data-http-headers-listing.md`](../system-prompts/system-data-http-headers-listing.md) | Lists common request, tracing, CORS, and response headers alongside placeholder URLs. | 238 | 2.0.45 | 2.0.45 |
| [`system-data-azure-auth-env-vars.md`](../system-prompts/system-data-azure-auth-env-vars.md) | Lists Azure authentication environment variables for tenant, client, secrets, and certs. | 78 | 2.0.45 | 2.0.45 |
| [`system-data-github-actions-review.md`](../system-prompts/system-data-github-actions-review.md) | GitHub Actions PR workflow checking out repo and running Claude code-review plugin. | 405 | 2.0.36 | 2.0.36 |
| [`system-data-filesystem-api-operations-list.md`](../system-prompts/system-data-filesystem-api-operations-list.md) | List of filesystem functions for access, reading, writing, and metadata operations. | 101 | 2.0.24 | 2.0.24 |
| [`system-data-macos-sandbox-policy-rules.md`](../system-prompts/system-data-macos-sandbox-policy-rules.md) | Sandbox profile allowing specific process permissions and Mach service lookups. | 1,787 | 2.0.17 | 2.0.17 |
| [`system-data-stream-zip-parse-errors.md`](../system-prompts/system-data-stream-zip-parse-errors.md) | Lists possible stream and archive validation error messages. | 72 | 2.0.17 | 2.0.17 |
| [`system-data-mention-triggered-github-workflow.md`](../system-prompts/system-data-mention-triggered-github-workflow.md) | Runs Claude Code action on issues or comments mentioning @claude, using Anthropic API key. | 494 | 2.0.8 | 2.0.8 |
| [`system-data-urls-and-placeholder-metrics.md`](../system-prompts/system-data-urls-and-placeholder-metrics.md) | Repeated URL fields followed by two expression slots and sixteen numeric value entries | 139 | 1.0.63 | 2.0.77 |
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
| [`system-data-http-request-timing-events.md`](../system-prompts/system-data-http-request-timing-events.md) | Lists HTTP request lifecycle timing event markers. | 113 | 0.2.30 | 0.2.30 |
| [`system-data-wolfram-language-symbols-list.md`](../system-prompts/system-data-wolfram-language-symbols-list.md) | Alphabetical list of Wolfram Language built-in symbol names. | 35,789 | 0.2.9 | 0.2.9 |
| [`system-data-stan-functions-reference-list.md`](../system-prompts/system-data-stan-functions-reference-list.md) | Partial catalog of Stan math, RNG, and distribution functions. | 2,155 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-placeholder-sequence.md`](../system-prompts/system-data-numeric-placeholder-sequence.md) | Repeated numeric placeholder tokens in a long sequence. | 1,791 | 0.2.9 | 0.2.9 |
| [`system-data-html-doctype-variants-list.md`](../system-prompts/system-data-html-doctype-variants-list.md) | Strings enumerating HTML doctype variants including strict, levels, and internet explorer. | 1,099 | 0.2.9 | 2.0.77 |
| [`system-data-html-doctype-variants-list-2.md`](../system-prompts/system-data-html-doctype-variants-list-2.md) | Strings enumerating HTML doctype variants including strict, levels, and internet explorer. | 1,063 | 0.2.9 | 2.0.77 |
| [`system-data-sql-keywords-current-array.md`](../system-prompts/system-data-sql-keywords-current-array.md) | List of SQL reserved words and functions including current and array terms. | 1,000 | 0.2.9 | 0.2.9 |
| [`system-data-repeated-numeric-placeholders.md`](../system-prompts/system-data-repeated-numeric-placeholders.md) | Long sequence of repeated numeric placeholder tokens. | 895 | 0.2.9 | 0.2.9 |
| [`system-data-julia-base-types-list.md`](../system-prompts/system-data-julia-base-types-list.md) | List of Julia core types and standard library names. | 723 | 0.2.9 | 0.2.9 |
| [`system-data-perl-builtin-functions-list.md`](../system-prompts/system-data-perl-builtin-functions-list.md) | List of Perl keywords and built-in functions. | 682 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-placeholder-block.md`](../system-prompts/system-data-numeric-placeholder-block.md) | Block of repeated numeric placeholder tokens. | 531 | 0.2.9 | 0.2.9 |
| [`system-data-hex-color-swatches-ccff.md`](../system-prompts/system-data-hex-color-swatches-ccff.md) | Sequence of hexadecimal color codes in CC/FF step combinations. | 387 | 0.2.9 | 0.2.9 |
| [`system-data-months-weekdays-number-mapping.md`](../system-prompts/system-data-months-weekdays-number-mapping.md) | Month and weekday names paired with numeric placeholders. | 341 | 0.2.9 | 0.2.9 |
| [`system-data-sql-functions-json-regression.md`](../system-prompts/system-data-sql-functions-json-regression.md) | Catalog of SQL functions including JSON, analytics, and regression aggregates. | 297 | 0.2.9 | 0.2.9 |
| [`system-data-stan-distributions-list.md`](../system-prompts/system-data-stan-distributions-list.md) | Enumerates probability distributions used in modeling. | 244 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-placeholders-repeated.md`](../system-prompts/system-data-numeric-placeholders-repeated.md) | Repeated numeric placeholder entries. | 237 | 0.2.9 | 0.2.9 |
| [`system-data-css-selectors-pseudo-classes.md`](../system-prompts/system-data-css-selectors-pseudo-classes.md) | Comprehensive list of CSS pseudo-classes and pseudo-elements. | 228 | 0.2.9 | 0.2.9 |
| [`system-data-javascript-builtins-and-typed-arrays.md`](../system-prompts/system-data-javascript-builtins-and-typed-arrays.md) | Enumerates JavaScript globals, built-in objects, errors, and typed arrays. | 216 | 0.2.9 | 0.2.9 |
| [`system-data-css-pseudo-class-keywords.md`](../system-prompts/system-data-css-pseudo-class-keywords.md) | List of CSS selector pseudo-classes and state keywords. | 186 | 0.2.9 | 0.2.9 |
| [`system-data-swift-keywords-list.md`](../system-prompts/system-data-swift-keywords-list.md) | List of Swift language keywords and declarations. | 171 | 0.2.9 | 2.0.74 |
| [`system-data-swift-keywords-list-3.md`](../system-prompts/system-data-swift-keywords-list-3.md) | List of Swift language keywords and declarations. | 166 | 0.2.9 | 2.0.72 |
| [`system-data-swift-keywords-list-2.md`](../system-prompts/system-data-swift-keywords-list-2.md) | List of Swift language keywords and declarations. | 162 | 0.2.9 | 2.0.74 |
| [`system-data-html-element-name-list.md`](../system-prompts/system-data-html-element-name-list.md) | List of common HTML element tag names. | 160 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-constants-and-paths.md`](../system-prompts/system-data-numeric-constants-and-paths.md) | Lists core constants and environment paths like Inf, NaN, missing, and LOAD_PATH. | 159 | 0.2.9 | 0.2.9 |
| [`system-data-swift-standard-library-functions.md`](../system-prompts/system-data-swift-standard-library-functions.md) | List of Swift standard library functions and assertions utilities. | 151 | 0.2.9 | 0.2.9 |
| [`system-data-swift-attribute-annotations.md`](../system-prompts/system-data-swift-attribute-annotations.md) | List of Swift attribute keywords and Cocoa/Interface Builder annotations including autoclosure and objcMembers. | 127 | 0.2.9 | 0.2.25 |
| [`system-data-media-query-features-list.md`](../system-prompts/system-data-media-query-features-list.md) | List CSS media query features and prefers settings. | 124 | 0.2.9 | 0.2.9 |
| [`system-data-mongodb-collection-methods-list.md`](../system-prompts/system-data-mongodb-collection-methods-list.md) | Lists MongoDB collection operations and index methods. | 116 | 0.2.9 | 0.2.9 |
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

## System reminders (86)

_Sorted by init (newest first). Showing **40** reminders with more than **30** tokens._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-reminder-interactive-cli-security-guardrails.md`](../system-prompts/system-reminder-interactive-cli-security-guardrails.md) | Sets CLI response style with security testing scope limits and url generation restrictions. | 2,886 | 2.0.77 | 2.0.77 |
| [`system-reminder-cli-security-safety-rules.md`](../system-prompts/system-reminder-cli-security-safety-rules.md) | Interactive CLI assistant with authorized security-testing limits and strict URL-generation restrictions. | 2,444 | 2.0.77 | 2.0.77 |
| [`system-reminder-plan-mode-only-edit-plan.md`](../system-prompts/system-reminder-plan-mode-only-edit-plan.md) | Plan mode: only edit designated plan file, use specified subagent types per phase. | 1,034 | 2.0.77 | 2.0.77 |
| [`system-reminder-github-api-put-file-update-2.md`](../system-prompts/system-reminder-github-api-put-file-update-2.md) | Template API PUT request to update repo content with message, content, and branch. | 76 | 2.0.77 | 2.0.77 |
| [`system-reminder-empty-todo-list-2.md`](../system-prompts/system-reminder-empty-todo-list-2.md) | Notes the todo list is empty and suggests using it internally without telling the user. | 68 | 2.0.77 | 2.0.77 |
| [`system-reminder-github-api-put-file-update.md`](../system-prompts/system-reminder-github-api-put-file-update.md) | Template API PUT request to update repo content with message, content, and branch. | 61 | 2.0.77 | 2.0.77 |
| [`system-reminder-ignore-local-command-messages-2.md`](../system-prompts/system-reminder-ignore-local-command-messages-2.md) | Warns that locally generated command messages should be ignored unless explicitly requested. | 52 | 2.0.77 | 2.0.77 |
| [`system-reminder-plan-mode-read-only-workflow.md`](../system-prompts/system-reminder-plan-mode-read-only-workflow.md) | Enforces plan mode: read-only outside plan file, follow phased workflow, end with questions or token. | 47 | 2.0.77 | 2.0.77 |
| [`system-reminder-plugin-install-status-restart.md`](../system-prompts/system-reminder-plugin-install-status-restart.md) | Reports installed plugin count, failures list, and restart instruction to load plugins. | 45 | 2.0.77 | 2.0.77 |
| [`system-reminder-structured-verification-result-call.md`](../system-prompts/system-reminder-structured-verification-result-call.md) | Requires emitting a structured verification result with success flag or failure reason. | 39 | 2.0.77 | 2.0.77 |
| [`system-reminder-read-unread-collab-messages.md`](../system-prompts/system-reminder-read-unread-collab-messages.md) | Alerts user to unread collab messages and directs using CollabRead to review them. | 33 | 2.0.77 | 2.0.77 |
| [`system-reminder-predict-next-user-input.md`](../system-prompts/system-reminder-predict-next-user-input.md) | Predicts the next thing the user would naturally type next. | 299 | 2.0.73 | 2.0.73 |
| [`system-reminder-web-page-content-pipe.md`](../system-prompts/system-reminder-web-page-content-pipe.md) | Wrapper containing captured web page content plus pipe bridge reference and extra data. | 37 | 2.0.71 | 2.0.71 |
| [`system-reminder-scale-image-coordinates.md`](../system-prompts/system-reminder-scale-image-coordinates.md) | Maps coordinates from displayed image size back to original resolution using a scaling factor. | 49 | 2.0.70 | 2.0.70 |
| [`system-reminder-user-project-local-scope-markers.md`](../system-prompts/system-reminder-user-project-local-scope-markers.md) | Repeated user, project, and local scope markers with placeholder insertions. | 46 | 2.0.70 | 2.0.70 |
| [`system-reminder-exit-delegate-mode.md`](../system-prompts/system-reminder-exit-delegate-mode.md) | Announces delegate mode exit and restores access to all tools. | 43 | 2.0.70 | 2.0.70 |
| [`system-reminder-exited-plan-mode-actions.md`](../system-prompts/system-reminder-exited-plan-mode-actions.md) | Indicates plan mode has ended and provides path to the saved plan file. | 47 | 2.0.62 | 2.0.62 |
| [`system-reminder-continue-from-plan-file.md`](../system-prompts/system-reminder-continue-from-plan-file.md) | Continue unfinished relevant work by resuming from an existing plan file’s contents. | 46 | 2.0.56 | 2.0.56 |
| [`system-reminder-resume-planning-from-existing-file.md`](../system-prompts/system-reminder-resume-planning-from-existing-file.md) | Review prior plan at EXPR_1, reconcile with new request, then update or overwrite before EXPR_2. | 234 | 2.0.52 | 2.0.52 |
| [`system-reminder-verify-stop-condition-plan.md`](../system-prompts/system-reminder-verify-stop-condition-plan.md) | Verify the agent completed the plan by checking transcript and codebase, then report status. | 119 | 2.0.51 | 2.0.52 |
| [`system-reminder-plan-only-no-edits.md`](../system-prompts/system-reminder-plan-only-no-edits.md) | Plan mode: only edit designated plan file, otherwise perform read-only actions and ask clarifications. | 190 | 2.0.43 | 2.0.43 |
| [`system-reminder-nudge-todo-tracking.md`](../system-prompts/system-reminder-nudge-todo-tracking.md) | Suggests using and cleaning up the todo list when it would help track progress. | 91 | 2.0.33 | 2.0.33 |
| [`system-reminder-budget-remaining.md`](../system-prompts/system-reminder-budget-remaining.md) | Multiple prompts (2) | 40 | 2.0.30 | 2.0.30 |
| [`system-reminder-malware-analysis-only.md`](../system-prompts/system-reminder-malware-analysis-only.md) | Analyze suspected malware but refuse to improve or extend it. | 80 | 2.0.24 | 2.0.24 |
| [`system-reminder-hook-blocking-error.md`](../system-prompts/system-reminder-hook-blocking-error.md) | Multiple prompts (2) | 39 | 2.0.17 | 2.0.17 |
| [`system-reminder-token-usage-remaining-line.md`](../system-prompts/system-reminder-token-usage-remaining-line.md) | Multiple prompts (2) | 37 | 2.0.17 | 2.0.17 |
| [`system-reminder-use-context-only-when-relevant.md`](../system-prompts/system-reminder-use-context-only-when-relevant.md) | Multiple prompts (2) | 69 | 2.0.2 | 2.0.2 |
| [`system-reminder-preserve-intentional-file-changes.md`](../system-prompts/system-reminder-preserve-intentional-file-changes.md) | Honor intentional modifications to EXPR_1; consider listed diffs without mentioning them to user. | 84 | 1.0.114 | 1.0.114 |
| [`system-reminder-fixed-length-conversation-title.md`](../system-prompts/system-reminder-fixed-length-conversation-title.md) | Write a title of the requested word count summarizing the given conversation. | 35 | 1.0.109 | 1.0.109 |
| [`system-reminder-session-memory-preview-guidance.md`](../system-prompts/system-reminder-session-memory-preview-guidance.md) | Notes that past session summaries may be unrelated and require reading full memory when needed. | 99 | 1.0.91 | 1.0.94 |
| [`system-reminder-access-prior-large-note.md`](../system-prompts/system-reminder-access-prior-large-note.md) | Reminds that … was previously read; use … tool to retrieve full contents. | 42 | 1.0.85 | 1.0.85 |
| [`system-reminder-todo-list-updated-silently-2.md`](../system-prompts/system-reminder-todo-list-updated-silently-2.md) | Internal notice that todo list updated; continue tasks without telling user. | 43 | 1.0.69 | 2.0.77 |
| [`system-reminder-selected-lines-context-note.md`](../system-prompts/system-reminder-selected-lines-context-note.md) | Shows user-selected line range from a file and cautions it may be unrelated. | 46 | 1.0.65 | 1.0.65 |
| [`system-reminder-invoke-requested.md`](../system-prompts/system-reminder-invoke-requested.md) | Invoke the specified agent when the user requests it, passing required context. | 32 | 1.0.62 | 1.0.62 |
| [`system-reminder-xml-bash-output-summarizer.md`](../system-prompts/system-reminder-xml-bash-output-summarizer.md) | Determine if command output is log spew and respond with XML indicating summary decision and content. | 657 | 1.0.60 | 1.0.109 |
| [`system-reminder-summarize-bash-output.md`](../system-prompts/system-reminder-summarize-bash-output.md) | Assess whether command output merits summarization, then summarize key relevant details. | 55 | 1.0.60 | 2.0.70 |
| [`system-reminder-file-offset-shorter-warning.md`](../system-prompts/system-reminder-file-offset-shorter-warning.md) | Warn that a file is shorter than the requested offset and report line count. | 42 | 1.0.53 | 1.0.53 |
| [`system-reminder-mcp-resource-no-displayable-content.md`](../system-prompts/system-reminder-mcp-resource-no-displayable-content.md) | MCP resource tag pointing to server and URI, with no displayable content. | 31 | 1.0.19 | 1.0.19 |
| [`system-reminder-underscore-template-function-wrapper.md`](../system-prompts/system-reminder-underscore-template-function-wrapper.md) | Compiled Underscore template function skeleton that escapes values and accumulates output. | 70 | 0.2.106 | 0.2.106 |
| [`system-reminder-hide-file-truncation-note.md`](../system-prompts/system-reminder-hide-file-truncation-note.md) | Warn file content is truncated and instruct using a command to read more. | 56 | 0.2.106 | 0.2.106 |

<details>
<summary>Show 46 low-token reminders (≤ 30 tokens)</summary>

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-reminder-continue-after-token-limit.md`](../system-prompts/system-reminder-continue-after-token-limit.md) | Instructs to continue work in smaller chunks after output cutoff. | 28 | 2.0.77 | 2.0.77 |
| [`system-reminder-new-collab-messages-alert.md`](../system-prompts/system-reminder-new-collab-messages-alert.md) | Signals that new collab messages arrived via stdio. | 18 | 2.0.77 | 2.0.77 |
| [`system-reminder-full-file-lines-omitted.md`](../system-prompts/system-reminder-full-file-lines-omitted.md) | Indicates how many additional lines exist in the full file. | 13 | 2.0.77 | 2.0.77 |
| [`system-reminder-follow-invoked-skills-guidelines.md`](../system-prompts/system-reminder-follow-invoked-skills-guidelines.md) | Reminder to keep adhering to the session’s previously invoked skills guidelines. | 23 | 2.0.72 | 2.0.72 |
| [`system-reminder-called-pipe-input.md`](../system-prompts/system-reminder-called-pipe-input.md) | Reminder that the browser bridge pipe tool was called with given input. | 29 | 2.0.71 | 2.0.77 |
| [`system-reminder-pipe-path.md`](../system-prompts/system-reminder-pipe-path.md) | System reminder containing the pipe bridge name and a path placeholder. | 28 | 2.0.71 | 2.0.71 |
| [`system-reminder-pipe-bridge-arguments.md`](../system-prompts/system-reminder-pipe-bridge-arguments.md) | Pipe bridge endpoint reminder showing provided arguments for browser MCP tool. | 24 | 2.0.71 | 2.0.71 |
| [`system-reminder-check-task-output.md`](../system-prompts/system-reminder-check-task-output.md) | Directs the user to check output via TaskOutput. | 11 | 2.0.65 | 2.0.65 |
| [`system-reminder-retirement-warning.md`](../system-prompts/system-reminder-retirement-warning.md) | Warns a specified model will retire on a given date and suggests switching. | 28 | 2.0.62 | 2.0.62 |
| [`system-reminder-handle-truncated-message.md`](../system-prompts/system-reminder-handle-truncated-message.md) | Show a truncated content segment while preserving the surrounding context and truncation count. | 27 | 2.0.56 | 2.0.56 |
| [`system-reminder-file-function-source-fields.md`](../system-prompts/system-reminder-file-function-source-fields.md) | Lists file name, function name, and source fields. | 6 | 2.0.55 | 2.0.55 |
| [`system-reminder-flag-emoji-regex-call-error.md`](../system-prompts/system-reminder-flag-emoji-regex-call-error.md) | Error about calling flag emoji regex due to unbound types. | 29 | 2.0.47 | 2.0.47 |
| [`system-reminder-flag-emoji-regex-construct-error.md`](../system-prompts/system-reminder-flag-emoji-regex-construct-error.md) | Error about constructing flag emoji regex due to unbound types. | 29 | 2.0.47 | 2.0.47 |
| [`system-reminder-surrogate-pair-call-type-error.md`](../system-prompts/system-reminder-surrogate-pair-call-type-error.md) | Error about calling surrogate pair pattern due to unbound types. | 27 | 2.0.47 | 2.0.47 |
| [`system-reminder-stop-hook-feedback.md`](../system-prompts/system-reminder-stop-hook-feedback.md) | Provide stop-hook feedback text to be displayed or logged. | 11 | 2.0.41 | 2.0.41 |
| [`system-reminder-enter-or-backspace-choice.md`](../system-prompts/system-reminder-enter-or-backspace-choice.md) | UI instruction showing Enter action and Backspace to unset a field. | 24 | 2.0.37 | 2.0.37 |
| [`system-reminder-usd-budget-remaining.md`](../system-prompts/system-reminder-usd-budget-remaining.md) | Formats USD budget summary showing used, total, and remaining amounts. | 26 | 2.0.30 | 2.0.30 |
| [`system-reminder-between-range-expression.md`](../system-prompts/system-reminder-between-range-expression.md) | Expression checking whether a value falls between two bounds. | 21 | 2.0.30 | 2.0.30 |
| [`system-reminder-plugin-install-restart-notice.md`](../system-prompts/system-reminder-plugin-install-restart-notice.md) | Confirms plugins installed and requests restart to load them. | 22 | 2.0.25 | 2.0.77 |
| [`system-reminder-hook-additional-context-2.md`](../system-prompts/system-reminder-hook-additional-context-2.md) | Multiple prompts (2) | 30 | 2.0.17 | 2.0.17 |
| [`system-reminder-hook-stopped-continuation-2.md`](../system-prompts/system-reminder-hook-stopped-continuation-2.md) | Multiple prompts (2) | 30 | 2.0.17 | 2.0.17 |
| [`system-reminder-hook-success.md`](../system-prompts/system-reminder-hook-success.md) | Multiple prompts (2) | 29 | 2.0.17 | 2.0.17 |
| [`system-reminder-hook-blocking-command-error.md`](../system-prompts/system-reminder-hook-blocking-command-error.md) | Report a blocking hook error triggered by a specific command execution. | 25 | 2.0.17 | 2.0.17 |
| [`system-reminder-token-usage-remaining.md`](../system-prompts/system-reminder-token-usage-remaining.md) | Shows token usage totals and remaining token budget in a single status line. | 23 | 2.0.17 | 2.0.17 |
| [`system-reminder-hook-additional-context.md`](../system-prompts/system-reminder-hook-additional-context.md) | Attach additional context details for a specified hook invocation. | 16 | 2.0.17 | 2.0.17 |
| [`system-reminder-hook-stopped-continuation.md`](../system-prompts/system-reminder-hook-stopped-continuation.md) | State why a hook stopped the continuation of an ongoing process. | 16 | 2.0.17 | 2.0.17 |
| [`system-reminder-hook-success-message.md`](../system-prompts/system-reminder-hook-success-message.md) | Confirm a hook ran successfully and provide its resulting output. | 15 | 2.0.17 | 2.0.17 |
| [`system-reminder-months-of-year-list.md`](../system-prompts/system-reminder-months-of-year-list.md) | List of month names from January through December. | 23 | 1.0.128 | 1.0.128 |
| [`system-reminder-binary-content-placeholder.md`](../system-prompts/system-reminder-binary-content-placeholder.md) | Wraps an expression as labeled binary content within bracketed placeholder markup. | 11 | 1.0.118 | 1.0.118 |
| [`system-reminder-other-users-modified-files.md`](../system-prompts/system-reminder-other-users-modified-files.md) | Display the list of files modified by other users. | 13 | 1.0.109 | 2.0.62 |
| [`system-reminder-title-only-response.md`](../system-prompts/system-reminder-title-only-response.md) | Return only the conversation title. | 12 | 1.0.109 | 1.0.109 |
| [`system-reminder-user-modified-files.md`](../system-prompts/system-reminder-user-modified-files.md) | Display the list of files modified by the current user. | 12 | 1.0.109 | 1.0.109 |
| [`system-reminder-shutdown-on-websocket-close.md`](../system-prompts/system-reminder-shutdown-on-websocket-close.md) | Indicates the bridge is shutting down due to a closed WebSocket connection. | 11 | 1.0.94 | 1.0.94 |
| [`system-reminder-active-style-guidelines.md`](../system-prompts/system-reminder-active-style-guidelines.md) | Reminder that the active output style must be followed exactly for responses. | 21 | 1.0.78 | 1.0.78 |
| [`system-reminder-address-user-message.md`](../system-prompts/system-reminder-address-user-message.md) | Address the user’s provided message and continue ongoing tasks accordingly. | 25 | 1.0.73 | 2.0.77 |
| [`system-reminder-continued-session-warning.md`](../system-prompts/system-reminder-continued-session-warning.md) | Warns session resumed on another machine and reports updated working directory path. | 26 | 1.0.68 | 1.0.68 |
| [`system-reminder-show-existing-todo-list.md`](../system-prompts/system-reminder-show-existing-todo-list.md) | Shows the current todo list contents inside a bracketed placeholder. | 19 | 1.0.52 | 1.0.94 |
| [`system-reminder-ide-file-opened-context.md`](../system-prompts/system-reminder-ide-file-opened-context.md) | Indicates the user opened a specific IDE file that may relate to task. | 27 | 1.0.32 | 1.0.32 |
| [`system-reminder-mcp-resource-no-content.md`](../system-prompts/system-reminder-mcp-resource-no-content.md) | MCP resource tag referencing server and URI placeholders, indicating no content available. | 29 | 1.0.19 | 1.0.19 |
| [`system-reminder-full-resource-contents-header.md`](../system-prompts/system-reminder-full-resource-contents-header.md) | Introduces the full contents of a referenced resource. | 5 | 1.0.19 | 1.0.19 |
| [`system-reminder-report-new-diagnostic-issues.md`](../system-prompts/system-reminder-report-new-diagnostic-issues.md) | Announces newly detected diagnostic issues and prints the associated details block. | 27 | 1.0.18 | 1.0.94 |
| [`system-reminder-call-error-result.md`](../system-prompts/system-reminder-call-error-result.md) | Template line reporting an error result from a specified tool call. | 13 | 0.2.119 | 0.2.119 |
| [`system-reminder-empty-existing-file-warning.md`](../system-prompts/system-reminder-empty-existing-file-warning.md) | Warns that a referenced file exists but has no contents. | 22 | 0.2.115 | 1.0.53 |
| [`system-reminder-smselect-smlike-smcard-tokens.md`](../system-prompts/system-reminder-smselect-smlike-smcard-tokens.md) | Lists component token names for reference. | 7 | 0.2.108 | 0.2.108 |
| [`system-reminder-show-variable-contents.md`](../system-prompts/system-reminder-show-variable-contents.md) | Show contents of a referenced variable or expression with its resolved value. | 16 | 0.2.107 | 0.2.107 |
| [`system-reminder-call-result.md`](../system-prompts/system-reminder-call-result.md) | Report the result returned from invoking a specified tool. | 18 | 0.2.106 | 2.0.77 |

</details>
