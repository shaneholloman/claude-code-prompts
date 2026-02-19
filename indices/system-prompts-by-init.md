# System Prompts Index – by init

- Total prompt files: **301**

## Categories

- System prompts (81)
- Tool prompts (69)
- Agent prompts (3)
- System data (86)
- System reminders (62)

## System prompts (81)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-prompt-safe-bash-command-execution-2.md`](../system-prompts/system-prompt-safe-bash-command-execution-2.md) | Run bash commands in persistent shell with directory checks, quoting rules, and timeouts | 2,450 | 2.0.0 | 2.0.0 |
| [`system-prompt-dev-conversation-summary.md`](../system-prompts/system-prompt-dev-conversation-summary.md) | Create a chronological, technically detailed conversation summary with analysis notes. | 1,268 | 2.0.0 | 2.0.0 |
| [`system-prompt-delegate-work-to-specialists.md`](../system-prompts/system-prompt-delegate-work-to-specialists.md) | Delegate multi-step tasks to specialized subagents and prefer direct search tools when appropriate. | 979 | 2.0.0 | 2.0.0 |
| [`system-prompt-update-session-notes-file.md`](../system-prompts/system-prompt-update-session-notes-file.md) | Single MultiEdit updates existing session file content only, preserving headers and italic descriptions. | 495 | 2.0.0 | 2.0.0 |
| [`system-prompt-constants-and-argument-tokens.md`](../system-prompts/system-prompt-constants-and-argument-tokens.md) | Provides a dense list of constants, group names, language codes, and argument tokens. | 291 | 2.0.0 | 2.0.0 |
| [`system-prompt-create-shell-snapshot-file-3.md`](../system-prompts/system-prompt-create-shell-snapshot-file-3.md) | Writes a snapshot script file, clears aliases, injects dynamic sections, and verifies output exists | 246 | 2.0.0 | 2.0.0 |
| [`system-prompt-tmux-terminal-shortcut-setup.md`](../system-prompts/system-prompt-tmux-terminal-shortcut-setup.md) | Sets Shift+Enter multiline shortcut by running terminal command outside tmux, persisting settings. | 141 | 2.0.0 | 2.0.0 |
| [`system-prompt-anthropic-path-snippets.md`](../system-prompts/system-prompt-anthropic-path-snippets.md) | Lists repeated @anthropic-ai PATH entries with additional-count placeholders EXPR_1 to EXPR_5. | 105 | 2.0.0 | 2.0.0 |
| [`system-prompt-absolute-paths-output-rules.md`](../system-prompts/system-prompt-absolute-paths-output-rules.md) | Use absolute paths, include filenames and code snippets, avoid emojis in final reply. | 100 | 2.0.0 | 2.0.0 |
| [`system-prompt-create-view-instrumentselector-local.md`](../system-prompts/system-prompt-create-view-instrumentselector-local.md) | Create a new view with specified name/description and InstrumentSelector set to local. | 97 | 2.0.0 | 2.0.0 |
| [`system-prompt-git-status-session-start.md`](../system-prompts/system-prompt-git-status-session-start.md) | Record starting git status snapshot, including current branch and recent commits. | 72 | 2.0.0 | 2.0.0 |
| [`system-prompt-file-updated-snippet.md`](../system-prompts/system-prompt-file-updated-snippet.md) | Announces … updated and shows numbered `cat -n` snippet output …. | 42 | 2.0.0 | 2.0.0 |
| [`system-prompt-continue-last-task.md`](../system-prompts/system-prompt-continue-last-task.md) | Resume from the previous point and proceed with the most recent task without asking questions. | 33 | 2.0.0 | 2.0.0 |
| [`system-prompt-cli-identity-2.md`](../system-prompts/system-prompt-cli-identity-2.md) | Defines Claude Code as Anthropic's official CLI running in the agent SDK. | 21 | 1.0.128 | 1.0.128 |
| [`system-prompt-stream-json-flag-argument-parsing.md`](../system-prompts/system-prompt-stream-json-flag-argument-parsing.md) | Conditional logic for selecting stream-json flag based on argument types. | 226 | 1.0.122 | 1.0.122 |
| [`system-prompt-frustration-and-pr-detection.md`](../system-prompts/system-prompt-frustration-and-pr-detection.md) | Analyze conversation to output frustration and explicit GitHub pull request send intent flags. | 220 | 1.0.122 | 1.0.122 |
| [`system-prompt-conversation-title-generator-2.md`](../system-prompts/system-prompt-conversation-title-generator-2.md) | Requests a fixed-length title derived from recent conversation messages. | 190 | 1.0.118 | 1.0.120 |
| [`system-prompt-conversation-title-generator-3.md`](../system-prompts/system-prompt-conversation-title-generator-3.md) | Requests a fixed-length title derived from recent conversation messages. | 148 | 1.0.118 | 1.0.120 |
| [`system-prompt-exit-transcript-rules.md`](../system-prompts/system-prompt-exit-transcript-rules.md) | Specifies how stdout and stderr are displayed for tool call inputs and responses by exit code. | 70 | 1.0.113 | 1.0.113 |
| [`system-prompt-constants-env-path-args.md`](../system-prompts/system-prompt-constants-env-path-args.md) | Multiple prompts (2) | 845 | 1.0.112 | 1.0.112 |
| [`system-prompt-create-md-guide-2.md`](../system-prompts/system-prompt-create-md-guide-2.md) | Analyze the repo and draft or improve a CLAUDE.md with commands and architecture. | 381 | 1.0.112 | 1.0.112 |
| [`system-prompt-command-purpose-in-words.md`](../system-prompts/system-prompt-command-purpose-in-words.md) | Guidelines to describe a shell command’s function in a fixed word range with examples. | 80 | 1.0.102 | 1.0.102 |
| [`system-prompt-background-task-monitoring.md`](../system-prompts/system-prompt-background-task-monitoring.md) | Announces task moved to background; provides monitoring link and teleport resume command. | 58 | 1.0.102 | 1.0.122 |
| [`system-prompt-read-local-files-by-path.md`](../system-prompts/system-prompt-read-local-files-by-path.md) | Reads local filesystem files by absolute path with optional line ranges and image viewing. | 423 | 1.0.98 | 1.0.98 |
| [`system-prompt-socat-tcp-to-unix-bridge.md`](../system-prompts/system-prompt-socat-tcp-to-unix-bridge.md) | Launches socat TCP listener to Unix socket, traps cleanup, then evals command | 112 | 1.0.93 | 1.0.93 |
| [`system-prompt-structured-coding-todo-list.md`](../system-prompts/system-prompt-structured-coding-todo-list.md) | Guide creating and updating a structured todo list for complex coding sessions. | 2,433 | 1.0.89 | 1.0.89 |
| [`system-prompt-github-issue-title-generator.md`](../system-prompts/system-prompt-github-issue-title-generator.md) | Generates a concise technical GitHub issue title from a bug report. | 254 | 1.0.89 | 1.0.89 |
| [`system-prompt-session-summary-template-sections.md`](../system-prompts/system-prompt-session-summary-template-sections.md) | Provides a structured template for summarizing task, worklog, codebase, workflow, corrections, and learnings. | 190 | 1.0.87 | 1.0.87 |
| [`system-prompt-json-command-exit-rules.md`](../system-prompts/system-prompt-json-command-exit-rules.md) | Defines JSON input and exit code handling for a command, showing stderr only on failure. | 34 | 1.0.85 | 1.0.85 |
| [`system-prompt-fix-settings-json-validation.md`](../system-prompts/system-prompt-fix-settings-json-validation.md) | Analyze Claude Code settings.json validation failure using provided error text and schema, no env changes. | 45 | 1.0.82 | 1.0.82 |
| [`system-prompt-learn-by-doing-human-input.md`](../system-prompts/system-prompt-learn-by-doing-human-input.md) | Request 3–5 line human code contributions for key logic, tracked via TodoList prompts. | 1,137 | 1.0.78 | 1.0.86 |
| [`system-prompt-educational-insights-cli.md`](../system-prompts/system-prompt-educational-insights-cli.md) | CLI engineering assistant adds codebase-specific insights before and after coding in formatted blocks | 220 | 1.0.78 | 1.0.78 |
| [`system-prompt-simple-conversation-title.md`](../system-prompts/system-prompt-simple-conversation-title.md) | Generate a NUM–NUM word conversation title using the last EXPR_1 of EXPR_2 messages. | 60 | 1.0.77 | 1.0.122 |
| [`system-prompt-create-statusline-setup-task.md`](../system-prompts/system-prompt-create-statusline-setup-task.md) | Creates a task that invokes the statusline setup subagent. | 31 | 1.0.72 | 1.0.72 |
| [`system-prompt-pull-request-review-workflow.md`](../system-prompts/system-prompt-pull-request-review-workflow.md) | GitHub Actions workflow runs Claude code review on pull request open or sync. | 723 | 1.0.71 | 1.0.71 |
| [`system-prompt-security-review-git-diff.md`](../system-prompts/system-prompt-security-review-git-diff.md) | Performs a high-confidence vulnerability review of branch changes using git status, logs, and diffs. | 2,808 | 1.0.69 | 1.0.69 |
| [`system-prompt-coding-session-title-generator.md`](../system-prompts/system-prompt-coding-session-title-generator.md) | Generate a concise XML-wrapped title from the provided coding session description. | 198 | 1.0.68 | 1.0.93 |
| [`system-prompt-coding-session-title-generator-2.md`](../system-prompts/system-prompt-coding-session-title-generator-2.md) | Creates a short XML-wrapped title from a coding session description. | 167 | 1.0.68 | 1.0.93 |
| [`system-prompt-export-aliases-filter-winpty.md`](../system-prompts/system-prompt-export-aliases-filter-winpty.md) | Writes aliases into the snapshot while filtering winpty aliases on Windows. | 218 | 1.0.65 | 1.0.65 |
| [`system-prompt-snapshot-functions-base64-encode.md`](../system-prompts/system-prompt-snapshot-functions-base64-encode.md) | Captures user functions by base64 encoding definitions and writing eval restore lines. | 200 | 1.0.65 | 1.0.65 |
| [`system-prompt-snapshot-functions-typeset-dump.md`](../system-prompts/system-prompt-snapshot-functions-typeset-dump.md) | Captures user function definitions via typeset and writes them directly to the snapshot. | 110 | 1.0.65 | 1.0.65 |
| [`system-prompt-record-shell-options-snapshot.md`](../system-prompts/system-prompt-record-shell-options-snapshot.md) | Appends current shell options and enables expand_aliases in the snapshot. | 100 | 1.0.65 | 1.0.65 |
| [`system-prompt-check-rg-and-alias.md`](../system-prompts/system-prompt-check-rg-and-alias.md) | Append snapshot logic to check for rg command and define a fallback alias. | 82 | 1.0.65 | 1.0.65 |
| [`system-prompt-command-json-exit-handling.md`](../system-prompts/system-prompt-command-json-exit-handling.md) | Rules for JSON command input and exit code output handling. | 40 | 1.0.64 | 1.0.64 |
| [`system-prompt-educational-insights.md`](../system-prompts/system-prompt-educational-insights.md) | Enforces brief pre/post code educational insights using a named insight banner format. | 134 | 1.0.63 | 1.0.64 |
| [`system-prompt-architect-configs-from-needs.md`](../system-prompts/system-prompt-architect-configs-from-needs.md) | Translate user requirements and project context into precise agent specifications. | 1,140 | 1.0.60 | 1.0.60 |
| [`system-prompt-summarize-bash-output-if-needed.md`](../system-prompts/system-prompt-summarize-bash-output-if-needed.md) | Assess whether command output merits summarization, then summarize key relevant details. | 55 | 1.0.60 | 2.0.0 |
| [`system-prompt-command-exit-handling.md`](../system-prompts/system-prompt-command-exit-handling.md) | Defines JSON input expectations and exit code behaviors. | 59 | 1.0.55 | 1.0.56 |
| [`system-prompt-exit-handling.md`](../system-prompts/system-prompt-exit-handling.md) | Defines stdout and stderr visibility rules based on command exit code for tool calls. | 62 | 1.0.53 | 1.0.53 |
| [`system-prompt-compaction-command-exit-codes.md`](../system-prompts/system-prompt-compaction-command-exit-codes.md) | Defines JSON input handling and exit-code behavior for compaction commands. | 55 | 1.0.53 | 1.0.53 |
| [`system-prompt-handle-exit-codes-and-output.md`](../system-prompts/system-prompt-handle-exit-codes-and-output.md) | Routes stdout and stderr visibility based on exit code and continues execution when needed. | 49 | 1.0.53 | 1.0.53 |
| [`system-prompt-exit-output-handling.md`](../system-prompts/system-prompt-exit-output-handling.md) | Route stdout and stderr visibility based on exit codes. | 45 | 1.0.53 | 1.0.53 |
| [`system-prompt-redirect-detected.md`](../system-prompts/system-prompt-redirect-detected.md) | Request WebFetch rerun to retrieve content from redirected host URL with new parameters. | 97 | 1.0.52 | 1.0.124 |
| [`system-prompt-install-github-app.md`](../system-prompts/system-prompt-install-github-app.md) | Explains adding a workflow to enable Claude Code via @claude mentions after merge. | 393 | 1.0.44 | 1.0.44 |
| [`system-prompt-hook-json-schema-validation.md`](../system-prompts/system-prompt-hook-json-schema-validation.md) | Indicates hook JSON validation failed and shows error details plus expected schema. | 24 | 1.0.38 | 1.0.38 |
| [`system-prompt-stop-hook-feedback-links.md`](../system-prompts/system-prompt-stop-hook-feedback-links.md) | Stop hook feedback message with referenced URLs. | 18 | 1.0.38 | 1.0.38 |
| [`system-prompt-github-permission-troubleshooting.md`](../system-prompts/system-prompt-github-permission-troubleshooting.md) | Provide quick fixes for common GitHub CLI permission and authorization issues. | 54 | 1.0.28 | 1.0.28 |
| [`system-prompt-github-repo-access-help.md`](../system-prompts/system-prompt-github-repo-access-help.md) | List common GitHub CLI repository access errors and the steps to resolve them. | 52 | 1.0.28 | 1.0.28 |
| [`system-prompt-verify-repo-access-scope.md`](../system-prompts/system-prompt-verify-repo-access-scope.md) | Validate GitHub repository name, access permissions, and token scopes for private repos. | 61 | 1.0.25 | 1.0.25 |
| [`system-prompt-bash-command-prefix-injection-detection.md`](../system-prompts/system-prompt-bash-command-prefix-injection-detection.md) | Define command prefix extraction and injection detection with illustrative shell command examples. | 693 | 1.0.23 | 1.0.34 |
| [`system-prompt-list-mcp-server-resources.md`](../system-prompts/system-prompt-list-mcp-server-resources.md) | Lists available resources across MCP servers with optional server filtering. | 73 | 1.0.22 | 1.0.22 |
| [`system-prompt-read-mcp-server-resource.md`](../system-prompts/system-prompt-read-mcp-server-resource.md) | Reads a resource from an MCP server by server name and URI. | 73 | 1.0.22 | 1.0.22 |
| [`system-prompt-avoid-rereading-unchanged-resource.md`](../system-prompts/system-prompt-avoid-rereading-unchanged-resource.md) | Instructs to not reread a resource unless it may have changed. | 22 | 1.0.19 | 1.0.19 |
| [`system-prompt-replace-all-occurrences-warning.md`](../system-prompts/system-prompt-replace-all-occurrences-warning.md) | Warns about multiple replacement matches when replace_all is false, requesting unique context. | 61 | 1.0.18 | 1.0.94 |
| [`system-prompt-extract-displayed-file-paths.md`](../system-prompts/system-prompt-extract-displayed-file-paths.md) | Identify and return only explicitly shown file paths when file contents are displayed. | 289 | 1.0.8 | 1.0.8 |
| [`system-prompt-exact-string-edits-in-files.md`](../system-prompts/system-prompt-exact-string-edits-in-files.md) | Define rules for exact in-file string replacements after reading and with unique matches. | 258 | 1.0.8 | 1.0.8 |
| [`system-prompt-write-file-with-constraints.md`](../system-prompts/system-prompt-write-file-with-constraints.md) | Defines rules for writing files, including reading before overwriting and avoiding new docs. | 145 | 1.0.7 | 1.0.7 |
| [`system-prompt-install-github-cli.md`](../system-prompts/system-prompt-install-github-cli.md) | Install GitHub CLI across macOS, Windows, and Linux. | 41 | 1.0.0 | 1.0.0 |
| [`system-prompt-admin-setup-secrets-apps.md`](../system-prompts/system-prompt-admin-setup-secrets-apps.md) | Have a repository admin install apps and configure secrets when setup fails. | 33 | 1.0.0 | 1.0.0 |
| [`system-prompt-use-owner-path-format.md`](../system-prompts/system-prompt-use-owner-path-format.md) | Use the owner and path or URL format for repository references. | 28 | 1.0.0 | 1.0.0 |
| [`system-prompt-authenticate-with-gh-cli.md`](../system-prompts/system-prompt-authenticate-with-gh-cli.md) | Authenticate to GitHub using gh auth login or environment-based methods. | 25 | 1.0.0 | 1.0.0 |
| [`system-prompt-summarize-coding-chat-status.md`](../system-prompts/system-prompt-summarize-coding-chat-status.md) | Condense a coding conversation into a character-limited status recap. | 33 | 0.2.91 | 0.2.91 |
| [`system-prompt-nested-template-functions.md`](../system-prompts/system-prompt-nested-template-functions.md) | Nested compiled template functions that concatenate output into a string buffer. | 134 | 0.2.54 | 1.0.86 |
| [`system-prompt-cite-with-limited-quotes.md`](../system-prompts/system-prompt-cite-with-limited-quotes.md) | Multiple prompts (2) | 140 | 0.2.40 | 2.0.0 |
| [`system-prompt-fetch-pr-comments.md`](../system-prompts/system-prompt-fetch-pr-comments.md) | Fetch PR-level and review comments via gh API, then format threads with diffs. | 444 | 0.2.9 | 0.2.9 |
| [`system-prompt-review-github-pull-request.md`](../system-prompts/system-prompt-review-github-pull-request.md) | Use GitHub CLI to list/view PRs, fetch diff, and deliver structured code review. | 233 | 0.2.9 | 0.2.9 |
| [`system-prompt-select-core-frequently-modified-files.md`](../system-prompts/system-prompt-select-core-frequently-modified-files.md) | Choose five diverse frequently modified core-logic filenames from git history stats. | 90 | 0.2.9 | 0.2.9 |
| [`system-prompt-detect-new-topic-title.md`](../system-prompts/system-prompt-detect-new-topic-title.md) | Detect whether a message starts a new topic and extract a short title. | 85 | 0.2.9 | 0.2.9 |
| [`system-prompt-fix-missing-executable-name.md`](../system-prompts/system-prompt-fix-missing-executable-name.md) | Advise fixes when a specified CLI subcommand executable path is missing. | 81 | 0.2.9 | 1.0.30 |
| [`system-prompt-file-updated-snippet-output.md`](../system-prompts/system-prompt-file-updated-snippet-output.md) | Notify that a file was updated and show numbered snippet output from cat -n. | 38 | 0.2.9 | 0.2.9 |
| [`system-prompt-classify-bash-command-prefix.md`](../system-prompts/system-prompt-classify-bash-command-prefix.md) | Determine the appropriate prefix for bash commands requested by a coding agent. | 33 | 0.2.9 | 0.2.9 |

## Tool prompts (69)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`tool-description-run-bash-commands-safely.md`](../system-prompts/tool-description-run-bash-commands-safely.md) | Run bash commands in persistent shell, verifying directories and quoting paths safely. | 926 | 2.0.0 | 2.0.0 |
| [`tool-description-show-plan-usage-limits.md`](../system-prompts/tool-description-show-plan-usage-limits.md) | Display plan usage and limits. | 4 | 2.0.0 | 2.0.0 |
| [`tool-description-restore-previous-conversation.md`](../system-prompts/tool-description-restore-previous-conversation.md) | Restores the conversation state to an earlier point. | 8 | 1.0.128 | 1.0.128 |
| [`tool-description-execute-slash-command-guide.md`](../system-prompts/tool-description-execute-slash-command-guide.md) | Execute validated slash command with arguments; on failure list up to … alternatives. | 160 | 1.0.122 | 1.0.122 |
| [`tool-description-read-local-file-paths.md`](../system-prompts/tool-description-read-local-file-paths.md) | File-reading tool spec with absolute-path requirement, line limits, and image support. | 427 | 1.0.98 | 1.0.98 |
| [`tool-description-view-update-privacy-settings.md`](../system-prompts/tool-description-view-update-privacy-settings.md) | View and update privacy settings. | 6 | 1.0.96 | 1.0.96 |
| [`tool-description-list-todo-items.md`](../system-prompts/tool-description-list-todo-items.md) | Requests listing the current todo items. | 4 | 1.0.94 | 1.0.94 |
| [`tool-description-structured-todo-list-usage-guidelines.md`](../system-prompts/tool-description-structured-todo-list-usage-guidelines.md) | Criteria for starting, updating, and avoiding a structured todo tool during coding sessions | 2,438 | 1.0.89 | 1.0.113 |
| [`tool-description-context-usage-grid.md`](../system-prompts/tool-description-context-usage-grid.md) | Renders current context usage as a colored grid visualization. | 10 | 1.0.86 | 1.0.86 |
| [`tool-description-collaborative-learning-cli.md`](../system-prompts/tool-description-collaborative-learning-cli.md) | Interactive CLI that blends task completion with learning by requesting meaningful human code contributions. | 1,009 | 1.0.78 | 1.0.78 |
| [`tool-description-educational-cli-engineering-help.md`](../system-prompts/tool-description-educational-cli-engineering-help.md) | Interactive CLI for engineering tasks with educational codebase insights under an explanatory style. | 92 | 1.0.78 | 1.0.78 |
| [`tool-description-set-output-style-menu.md`](../system-prompts/tool-description-set-output-style-menu.md) | Instruction to set the output style directly or via a selection menu. | 10 | 1.0.78 | 1.0.78 |
| [`tool-description-check-background-bash-output.md`](../system-prompts/tool-description-check-background-bash-output.md) | Tool to read only new output from a running or completed background bash shell. | 97 | 1.0.72 | 1.0.72 |
| [`tool-description-bus-error-message.md`](../system-prompts/tool-description-bus-error-message.md) | Reports a bus error from misaligned or invalid memory access. | 16 | 1.0.68 | 1.0.68 |
| [`tool-description-paused-by-ctrl-z-or-suspend.md`](../system-prompts/tool-description-paused-by-ctrl-z-or-suspend.md) | Marks the process as stopped via job-control suspend. | 12 | 1.0.68 | 1.0.68 |
| [`tool-description-child-process-state-change.md`](../system-prompts/tool-description-child-process-state-change.md) | Multiple prompts (2) | 10 | 1.0.68 | 1.0.68 |
| [`tool-description-ctrl-break-interruption.md`](../system-prompts/tool-description-ctrl-break-interruption.md) | Indicates the user interrupted execution with CTRL-BREAK. | 9 | 1.0.68 | 1.0.68 |
| [`tool-description-emulated-command-not-implemented.md`](../system-prompts/tool-description-emulated-command-not-implemented.md) | Indicates a command is expected to be emulated but has no implementation. | 9 | 1.0.68 | 1.0.68 |
| [`tool-description-application-specific-realtime-signal.md`](../system-prompts/tool-description-application-specific-realtime-signal.md) | Denotes receipt of an application-defined realtime signal. | 8 | 1.0.68 | 1.0.94 |
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
| [`tool-description-fetch-and-analyze-web-content.md`](../system-prompts/tool-description-fetch-and-analyze-web-content.md) | Describes a tool that fetches a URL, converts HTML to markdown, and analyzes it with a small model. | 272 | 1.0.42 | 1.0.42 |
| [`tool-description-web-search-current-info.md`](../system-prompts/tool-description-web-search-current-info.md) | Searches the web for up-to-date information and returns formatted result blocks. | 159 | 1.0.40 | 1.0.40 |
| [`tool-description-ripgrep-search-guidelines.md`](../system-prompts/tool-description-ripgrep-search-guidelines.md) | Guidelines for using the Grep search tool with regex, filters, and output modes. | 250 | 1.0.38 | 1.0.38 |
| [`tool-description-manage-hook-configurations.md`](../system-prompts/tool-description-manage-hook-configurations.md) | Tool description for managing hook configurations for tool events. | 7 | 1.0.38 | 1.0.38 |
| [`tool-description-exit-planning-when-ready.md`](../system-prompts/tool-description-exit-planning-when-ready.md) | Instructs when to trigger leaving planning mode before starting implementation. | 180 | 1.0.32 | 1.0.57 |
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
| [`tool-description-list-manage-background-tasks.md`](../system-prompts/tool-description-list-manage-background-tasks.md) | List and manage background tasks. | 5 | 0.2.117 | 1.0.102 |
| [`tool-description-fast-glob-file-matching-2.md`](../system-prompts/tool-description-fast-glob-file-matching-2.md) | Glob-based file matcher returning paths sorted by modification time and supports batching searches. | 118 | 0.2.116 | 0.2.116 |
| [`tool-description-setup-github-actions.md`](../system-prompts/tool-description-setup-github-actions.md) | Sets up Claude GitHub Actions integration for a repository. | 8 | 0.2.101 | 0.2.101 |
| [`tool-description-option-enter-newline-binding.md`](../system-prompts/tool-description-option-enter-newline-binding.md) | Enable Option+Enter to insert newlines. | 12 | 0.2.80 | 0.2.83 |
| [`tool-description-list-files-in-context.md`](../system-prompts/tool-description-list-files-in-context.md) | List all files currently available in context. | 6 | 0.2.79 | 0.2.79 |
| [`tool-description-clear-chat-keep-summary.md`](../system-prompts/tool-description-clear-chat-keep-summary.md) | Clears conversation history while retaining a summary in context. | 24 | 0.2.54 | 0.2.57 |
| [`tool-description-toggle-vim-editing-mode.md`](../system-prompts/tool-description-toggle-vim-editing-mode.md) | Switch between Vim and normal editing modes. | 8 | 0.2.54 | 0.2.54 |
| [`tool-description-edit-memory-files.md`](../system-prompts/tool-description-edit-memory-files.md) | Edit Claude memory files. | 4 | 0.2.54 | 0.2.54 |
| [`tool-description-migrate-npm-global-to-local.md`](../system-prompts/tool-description-migrate-npm-global-to-local.md) | Move from a global npm install to a project-local installation. | 9 | 0.2.51 | 0.2.51 |
| [`tool-description-replace-jupyter-notebook-cell.md`](../system-prompts/tool-description-replace-jupyter-notebook-cell.md) | Replaces, inserts, or deletes a specific Jupyter notebook cell by index. | 117 | 0.2.9 | 0.2.83 |
| [`tool-description-show-session-cost-and-duration.md`](../system-prompts/tool-description-show-session-cost-and-duration.md) | Displays the current session total cost and duration. | 10 | 0.2.9 | 0.2.9 |
| [`tool-description-sign-in-anthropic-account.md`](../system-prompts/tool-description-sign-in-anthropic-account.md) | Signs in using an Anthropic account. | 8 | 0.2.9 | 0.2.9 |
| [`tool-description-sign-out-anthropic-account.md`](../system-prompts/tool-description-sign-out-anthropic-account.md) | Signs out from an Anthropic account. | 8 | 0.2.9 | 0.2.9 |
| [`tool-description-clear-conversation-history.md`](../system-prompts/tool-description-clear-conversation-history.md) | Clears conversation history to free up context. | 7 | 0.2.9 | 0.2.9 |
| [`tool-description-show-help-and-commands.md`](../system-prompts/tool-description-show-help-and-commands.md) | Displays help text and available commands. | 5 | 0.2.9 | 0.2.9 |
| [`tool-description-submit-feedback.md`](../system-prompts/tool-description-submit-feedback.md) | Submits user feedback about Claude Code. | 5 | 0.2.9 | 1.0.102 |

## Agent prompts (3)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`agent-prompt-custom-output-style-config.md`](../system-prompts/agent-prompt-custom-output-style-config.md) | Derive user preferences and generate a configuration for a custom output style. | 743 | 1.0.84 | 1.0.98 |
| [`agent-prompt-configure-statusline.md`](../system-prompts/agent-prompt-configure-statusline.md) | Create or update a Claude Code statusLine by converting shell PS1 settings. | 1,055 | 1.0.81 | 1.0.81 |
| [`agent-prompt-codebase-search-analysis-guide.md`](../system-prompts/agent-prompt-codebase-search-analysis-guide.md) | Guidance for searching and analyzing multiple files in a codebase without creating files. | 287 | 1.0.45 | 1.0.78 |

## System data (86)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-data-macos-sandbox-policy-rules.md`](../system-prompts/system-data-macos-sandbox-policy-rules.md) | Sandbox profile allowing specific process permissions and Mach service lookups. | 1,769 | 2.0.0 | 2.0.0 |
| [`system-data-conversation-title-generator-3.md`](../system-prompts/system-data-conversation-title-generator-3.md) | Instructs generating a fixed-length title from the last conversation messages. | 219 | 2.0.0 | 2.0.0 |
| [`system-data-conversation-title.md`](../system-prompts/system-data-conversation-title.md) | Repeats title-generation directions with appended anthropic-ai path context. | 219 | 2.0.0 | 2.0.0 |
| [`system-data-write-conversation-title-4.md`](../system-prompts/system-data-write-conversation-title-4.md) | Instruction to generate a short title for a conversation. | 170 | 2.0.0 | 2.0.0 |
| [`system-data-force-uninstall-function-template.md`](../system-prompts/system-data-force-uninstall-function-template.md) | Defines a function running forced global uninstall with additional arguments and pattern string. | 104 | 2.0.0 | 2.0.0 |
| [`system-data-uninstall-command-arguments.md`](../system-prompts/system-data-uninstall-command-arguments.md) | Uninstall @anthropic-ai package globally with force flag and configurable pattern expression options. | 100 | 2.0.0 | 2.0.0 |
| [`system-data-mcp-server-2.md`](../system-prompts/system-data-mcp-server-2.md) | MCP uninstall tool usage flags and force options with pattern and extra expressions. | 98 | 2.0.0 | 2.0.0 |
| [`system-data-local-environment-metadata.md`](../system-prompts/system-data-local-environment-metadata.md) | Multiple prompts (2) | 91 | 2.0.0 | 2.0.0 |
| [`system-data-session-start-uninstall.md`](../system-prompts/system-data-session-start-uninstall.md) | Session-start hook runs forced global uninstall targeting a specified pattern and extra flags. | 87 | 2.0.0 | 2.0.0 |
| [`system-data-uninstall-command-block.md`](../system-prompts/system-data-uninstall-command-block.md) | Forced global uninstall command with pattern filter and multiple optional argument expressions. | 86 | 2.0.0 | 2.0.0 |
| [`system-data-pattern-metadata-record.md`](../system-prompts/system-data-pattern-metadata-record.md) | Pattern record listing multiple expression fields, numeric counters, filesystem paths, and trailing notes | 71 | 2.0.0 | 2.0.0 |
| [`system-data-api-put-update-file-branch.md`](../system-prompts/system-data-api-put-update-file-branch.md) | Runs background bash then issues an API PUT to update repo content on a branch. | 298 | 1.0.128 | 1.0.128 |
| [`system-data-pattern-with-background-bash-status-2.md`](../system-prompts/system-data-pattern-with-background-bash-status-2.md) | Template combining a pattern field with background bash command and status. | 236 | 1.0.128 | 2.0.0 |
| [`system-data-pattern-with-background-bash-status.md`](../system-prompts/system-data-pattern-with-background-bash-status.md) | Template combining a pattern field with background bash command and status. | 185 | 1.0.128 | 2.0.0 |
| [`system-data-api-put-with-context-and-stream.md`](../system-prompts/system-data-api-put-with-context-and-stream.md) | API PUT update sequence with user/project/local context and stream-json fields. | 178 | 1.0.128 | 1.0.128 |
| [`system-data-api-put-repo-update.md`](../system-prompts/system-data-api-put-repo-update.md) | Specifies an API PUT request to update repository content with message and branch. | 160 | 1.0.128 | 1.0.128 |
| [`system-data-background-bash-status.md`](../system-prompts/system-data-background-bash-status.md) | Captures background bash commands along with their execution status outputs. | 150 | 1.0.128 | 1.0.128 |
| [`system-data-patterned-conversation-title.md`](../system-prompts/system-data-patterned-conversation-title.md) | Generate a NUM–NUM word conversation title following pattern and recent message window. | 146 | 1.0.128 | 1.0.128 |
| [`system-data-codebase-user.md`](../system-prompts/system-data-codebase-user.md) | Mandates strict adherence to overriding codebase and user instructions, injecting eight templated blocks. | 98 | 1.0.128 | 1.0.128 |
| [`system-data-cell-pattern-xml-template.md`](../system-prompts/system-data-cell-pattern-xml-template.md) | XML cell tag with dynamic id, pattern string, and nested path element id | 80 | 1.0.128 | 1.0.128 |
| [`system-data-http-request-timing-events.md`](../system-prompts/system-data-http-request-timing-events.md) | Lists HTTP request lifecycle timing event markers. | 97 | 1.0.127 | 1.0.127 |
| [`system-data-github-pr-review.md`](../system-prompts/system-data-github-pr-review.md) | GitHub Actions pull_request workflow checks out code and runs Claude review on a PR. | 534 | 1.0.124 | 1.0.124 |
| [`system-data-write-conversation-title-2.md`](../system-prompts/system-data-write-conversation-title-2.md) | Requests a fixed-length title for a conversation using recent message context. | 160 | 1.0.118 | 1.0.118 |
| [`system-data-common-shell-and-docker-commands.md`](../system-prompts/system-data-common-shell-and-docker-commands.md) | List of common Unix utilities plus Docker ps/images and basic system info commands. | 81 | 1.0.109 | 1.0.109 |
| [`system-data-conversation-title-generator-variables-2.md`](../system-prompts/system-data-conversation-title-generator-variables-2.md) | Compose a word title from the last messages using multiple inserted sections. | 109 | 1.0.93 | 1.0.120 |
| [`system-data-conversation-title-generator-variables.md`](../system-prompts/system-data-conversation-title-generator-variables.md) | Compose a word title from the last messages using multiple inserted sections. | 109 | 1.0.93 | 1.0.128 |
| [`system-data-mention-triggered-github-workflow.md`](../system-prompts/system-data-mention-triggered-github-workflow.md) | Runs Claude Code action on issues or comments mentioning @claude, using Anthropic API key. | 520 | 1.0.91 | 1.0.91 |
| [`system-data-github-events-trigger.md`](../system-prompts/system-data-github-events-trigger.md) | GitHub Actions workflow triggers Claude Code job when @claude appears in events. | 648 | 1.0.71 | 1.0.71 |
| [`system-data-ignore-caches-and-binaries.md`](../system-prompts/system-data-ignore-caches-and-binaries.md) | Ignore list for repos covering caches, media, archives, and binary data files. | 422 | 1.0.70 | 1.0.70 |
| [`system-data-truncated-numeric-placeholders.md`](../system-prompts/system-data-truncated-numeric-placeholders.md) | Truncated stream of numeric placeholders. | 1,119 | 1.0.59 | 1.0.59 |
| [`system-data-extended-numeric-placeholders.md`](../system-prompts/system-data-extended-numeric-placeholders.md) | Extended list of numeric placeholder values. | 678 | 1.0.59 | 1.0.59 |
| [`system-data-numeric-placeholders-sequence.md`](../system-prompts/system-data-numeric-placeholders-sequence.md) | Sequence of numeric placeholder lines. | 454 | 1.0.59 | 1.0.59 |
| [`system-data-numeric-placeholders-dump.md`](../system-prompts/system-data-numeric-placeholders-dump.md) | Multiple prompts (10) | 447 | 1.0.59 | 1.0.59 |
| [`system-data-repeated-number-placeholders.md`](../system-prompts/system-data-repeated-number-placeholders.md) | Series of repeated numeric placeholder lines. | 223 | 1.0.59 | 1.0.59 |
| [`system-data-character-mapping-table.md`](../system-prompts/system-data-character-mapping-table.md) | Contains numeric sequences and letter markers resembling a mapping table. | 184,755 | 1.0.32 | 1.0.32 |
| [`system-data-json-schema-constraints-list.md`](../system-prompts/system-data-json-schema-constraints-list.md) | List of common JSON Schema constraint and validation keywords. | 59 | 1.0.20 | 1.0.20 |
| [`system-data-numeric-placeholder-list.md`](../system-prompts/system-data-numeric-placeholder-list.md) | Repeated numeric placeholders in a long list. | 573 | 0.2.125 | 0.2.125 |
| [`system-data-http-header-field-list.md`](../system-prompts/system-data-http-header-field-list.md) | List of HTTP request and response header fields including CORS and CSP. | 501 | 0.2.125 | 0.2.125 |
| [`system-data-linter-formatter-list.md`](../system-prompts/system-data-linter-formatter-list.md) | Lists common linters, formatters, and code quality tools. | 98 | 0.2.123 | 0.2.123 |
| [`system-data-underscore-template-runtime.md`](../system-prompts/system-data-underscore-template-runtime.md) | Scaffold compiled template function using escape, join, and print output buffering. | 133 | 0.2.54 | 2.0.0 |
| [`system-data-underscore-template-runtime-2.md`](../system-prompts/system-data-underscore-template-runtime-2.md) | Scaffold compiled template function using escape, join, and print output buffering. | 129 | 0.2.54 | 2.0.0 |
| [`system-data-javascript-builtins-list.md`](../system-prompts/system-data-javascript-builtins-list.md) | Enumeration of common JavaScript globals, typed arrays, collections, and utility functions. | 91 | 0.2.54 | 0.2.54 |
| [`system-data-plist-keybinding-xml-template.md`](../system-prompts/system-data-plist-keybinding-xml-template.md) | XML property-list snippet for a keybinding entry with numeric fields. | 158 | 0.2.46 | 0.2.46 |
| [`system-data-dom-exception-messages-codes.md`](../system-prompts/system-data-dom-exception-messages-codes.md) | DOM exception names with placeholder numeric codes and messages. | 532 | 0.2.33 | 0.2.33 |
| [`system-data-dom-exception-names-list.md`](../system-prompts/system-data-dom-exception-names-list.md) | List of DOM exception constants including security and network errors. | 184 | 0.2.33 | 0.2.33 |
| [`system-data-dom-media-input-events-list.md`](../system-prompts/system-data-dom-media-input-events-list.md) | List of common DOM, media, and form event names. | 153 | 0.2.33 | 0.2.33 |
| [`system-data-html-block-elements-list.md`](../system-prompts/system-data-html-block-elements-list.md) | List of uppercase HTML structural and block-level tag names. | 148 | 0.2.33 | 0.2.33 |
| [`system-data-wolfram-language-symbols-list.md`](../system-prompts/system-data-wolfram-language-symbols-list.md) | Alphabetical list of Wolfram Language built-in symbol names. | 35,789 | 0.2.9 | 0.2.9 |
| [`system-data-stan-functions-reference-list.md`](../system-prompts/system-data-stan-functions-reference-list.md) | Partial catalog of Stan math, RNG, and distribution functions. | 2,155 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-placeholder-sequence.md`](../system-prompts/system-data-numeric-placeholder-sequence.md) | Repeated numeric placeholder tokens in a long sequence. | 1,791 | 0.2.9 | 0.2.9 |
| [`system-data-html-doctype-variants-list.md`](../system-prompts/system-data-html-doctype-variants-list.md) | Strings enumerating HTML doctype variants including strict, levels, and internet explorer. | 1,099 | 0.2.9 | 1.0.128 |
| [`system-data-html-doctype-variants-list-2.md`](../system-prompts/system-data-html-doctype-variants-list-2.md) | Strings enumerating HTML doctype variants including strict, levels, and internet explorer. | 1,063 | 0.2.9 | 1.0.128 |
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
| [`system-data-swift-keywords-list.md`](../system-prompts/system-data-swift-keywords-list.md) | List of Swift language keywords and declarations. | 171 | 0.2.9 | 2.0.0 |
| [`system-data-swift-keywords-list-3.md`](../system-prompts/system-data-swift-keywords-list-3.md) | List of Swift language keywords and declarations. | 166 | 0.2.9 | 1.0.127 |
| [`system-data-swift-keywords-list-2.md`](../system-prompts/system-data-swift-keywords-list-2.md) | List of Swift language keywords and declarations. | 162 | 0.2.9 | 2.0.0 |
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

## System reminders (62)

_Sorted by init (newest first). Showing **31** reminders with more than **30** tokens._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-reminder-defensive-security-cli-guidelines-2.md`](../system-prompts/system-reminder-defensive-security-cli-guidelines-2.md) | Defines CLI behavior with strict defensive-security limits and URL caution. | 2,848 | 2.0.0 | 2.0.0 |
| [`system-reminder-background-bash-status.md`](../system-prompts/system-reminder-background-bash-status.md) | Format background Bash job report with command, status, and optional output sections. | 99 | 2.0.0 | 2.0.0 |
| [`system-reminder-uninstall.md`](../system-prompts/system-reminder-uninstall.md) | Forced global uninstall command template with pattern filter and optional extra arguments. | 77 | 2.0.0 | 2.0.0 |
| [`system-reminder-force-uninstall-pattern.md`](../system-prompts/system-reminder-force-uninstall-pattern.md) | Force global uninstall command using target, quoted pattern filter, and additional trailing flags. | 63 | 2.0.0 | 2.0.0 |
| [`system-reminder-task-with-prior-context.md`](../system-prompts/system-reminder-task-with-prior-context.md) | System reminder framing a task with optional local prior conversation context summary. | 63 | 2.0.0 | 2.0.0 |
| [`system-reminder-post-hook-feedback.md`](../system-prompts/system-reminder-post-hook-feedback.md) | Acknowledge post-tool-use hook feedback at given path and continue tasks. | 45 | 2.0.0 | 2.0.0 |
| [`system-reminder-user-selected-lines-2.md`](../system-prompts/system-reminder-user-selected-lines-2.md) | Reference user-selected line range from a local file, possibly unrelated to task. | 41 | 2.0.0 | 2.0.0 |
| [`system-reminder-token-usage-warning.md`](../system-prompts/system-reminder-token-usage-warning.md) | System warning displays tokens used out of limit and remaining balance. | 35 | 2.0.0 | 2.0.0 |
| [`system-reminder-conversation-title-generator-3.md`](../system-prompts/system-reminder-conversation-title-generator-3.md) | Write a NUM–NUM word conversation title using last EXPR_1 of EXPR_2 messages | 78 | 1.0.127 | 1.0.127 |
| [`system-reminder-preserve-intentional-file-changes.md`](../system-prompts/system-reminder-preserve-intentional-file-changes.md) | Honor intentional modifications to EXPR_1; consider listed diffs without mentioning them to user. | 84 | 1.0.114 | 1.0.114 |
| [`system-reminder-remote-session-task-status.md`](../system-prompts/system-reminder-remote-session-task-status.md) | Renders background remote session status block with task id, title, status, and delta summary | 55 | 1.0.111 | 1.0.111 |
| [`system-reminder-session-title.md`](../system-prompts/system-reminder-session-title.md) | Generate a session title based on the provided session description text. | 37 | 1.0.109 | 1.0.109 |
| [`system-reminder-fixed-length-conversation-title.md`](../system-prompts/system-reminder-fixed-length-conversation-title.md) | Write a title of the requested word count summarizing the given conversation. | 35 | 1.0.109 | 1.0.109 |
| [`system-reminder-conversation-development-summary.md`](../system-prompts/system-reminder-conversation-development-summary.md) | Produce a chronological, technically detailed conversation summary with analysis wrapped in tags. | 1,273 | 1.0.103 | 1.0.128 |
| [`system-reminder-nudge-todo-tracking.md`](../system-prompts/system-reminder-nudge-todo-tracking.md) | Suggests using and cleaning up the todo list when it would help track progress. | 79 | 1.0.94 | 1.0.94 |
| [`system-reminder-session-memory-preview-guidance.md`](../system-prompts/system-reminder-session-memory-preview-guidance.md) | Notes that past session summaries may be unrelated and require reading full memory when needed. | 99 | 1.0.91 | 1.0.94 |
| [`system-reminder-access-prior-large-note.md`](../system-prompts/system-reminder-access-prior-large-note.md) | Reminds that … was previously read; use … tool to retrieve full contents. | 42 | 1.0.85 | 1.0.85 |
| [`system-reminder-plan-mode-no-execution.md`](../system-prompts/system-reminder-plan-mode-no-execution.md) | Answer user query, then present a confirmation plan via the EXPR_1 tool. | 155 | 1.0.69 | 1.0.69 |
| [`system-reminder-empty-todo-list.md`](../system-prompts/system-reminder-empty-todo-list.md) | Remind that the todo list is empty and must not be mentioned. | 72 | 1.0.69 | 1.0.69 |
| [`system-reminder-todo-list-updated-silently-2.md`](../system-prompts/system-reminder-todo-list-updated-silently-2.md) | Internal notice that todo list updated; continue tasks without telling user. | 43 | 1.0.69 | 1.0.69 |
| [`system-reminder-invoke-requested.md`](../system-prompts/system-reminder-invoke-requested.md) | Invoke the specified agent when the user requests it, passing required context. | 32 | 1.0.62 | 1.0.62 |
| [`system-reminder-architect-configs-from-needs.md`](../system-prompts/system-reminder-architect-configs-from-needs.md) | Convert user goals and project context into detailed, reliable agent specification steps. | 1,150 | 1.0.60 | 1.0.60 |
| [`system-reminder-xml-bash-output-summarizer.md`](../system-prompts/system-reminder-xml-bash-output-summarizer.md) | Determine if command output is log spew and respond with XML indicating summary decision and content. | 657 | 1.0.60 | 1.0.109 |
| [`system-reminder-summarize-bash-output.md`](../system-prompts/system-reminder-summarize-bash-output.md) | Assess whether command output merits summarization, then summarize key relevant details. | 55 | 1.0.60 | 2.0.0 |
| [`system-reminder-use-context-only-when-relevant.md`](../system-prompts/system-reminder-use-context-only-when-relevant.md) | Multiple prompts (2) | 71 | 1.0.59 | 1.0.59 |
| [`system-reminder-file-offset-shorter-warning.md`](../system-prompts/system-reminder-file-offset-shorter-warning.md) | Warn that a file is shorter than the requested offset and report line count. | 42 | 1.0.53 | 1.0.53 |
| [`system-reminder-malicious-file-check-on-read.md`](../system-prompts/system-reminder-malicious-file-check-on-read.md) | Assess files for malicious content on read and refuse to enhance if malicious. | 67 | 1.0.31 | 1.0.31 |
| [`system-reminder-mcp-resource-no-displayable-content.md`](../system-prompts/system-reminder-mcp-resource-no-displayable-content.md) | MCP resource tag pointing to server and URI, with no displayable content. | 31 | 1.0.19 | 1.0.19 |
| [`system-reminder-ignore-local-command-messages.md`](../system-prompts/system-reminder-ignore-local-command-messages.md) | Warns that local command output messages should be ignored unless explicitly requested. | 38 | 1.0.7 | 1.0.7 |
| [`system-reminder-hide-file-truncation-note.md`](../system-prompts/system-reminder-hide-file-truncation-note.md) | Warn file content is truncated and instruct using a command to read more. | 56 | 0.2.106 | 0.2.106 |
| [`system-reminder-quote-limited-web-response.md`](../system-prompts/system-reminder-quote-limited-web-response.md) | Multiple prompts (2) | 140 | 0.2.40 | 2.0.0 |

<details>
<summary>Show 31 low-token reminders (≤ 30 tokens)</summary>

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-reminder-terminal-color-codes.md`](../system-prompts/system-reminder-terminal-color-codes.md) | List of terminal color label constants. | 30 | 2.0.0 | 2.0.0 |
| [`system-reminder-smselect-smlike-smcard-tokens.md`](../system-prompts/system-reminder-smselect-smlike-smcard-tokens.md) | Lists component token names for reference. | 13 | 2.0.0 | 2.0.0 |
| [`system-reminder-hourly-limit-reset-notice.md`](../system-prompts/system-reminder-hourly-limit-reset-notice.md) | Notice that an hourly limit resets and extra usage continues. | 24 | 1.0.128 | 1.0.128 |
| [`system-reminder-months-of-year-list.md`](../system-prompts/system-reminder-months-of-year-list.md) | List of month names from January through December. | 23 | 1.0.128 | 1.0.128 |
| [`system-reminder-opus-limit-reset-notice.md`](../system-prompts/system-reminder-opus-limit-reset-notice.md) | Notice that the Opus limit resets and extra usage continues. | 19 | 1.0.128 | 1.0.128 |
| [`system-reminder-ssm-ui-components-list.md`](../system-prompts/system-reminder-ssm-ui-components-list.md) | List of SSM browse and select component names. | 19 | 1.0.128 | 1.0.128 |
| [`system-reminder-weekly-limit-reset-notice.md`](../system-prompts/system-reminder-weekly-limit-reset-notice.md) | Notice that a weekly limit resets and extra usage continues. | 18 | 1.0.128 | 1.0.128 |
| [`system-reminder-extra-usage-active-notice.md`](../system-prompts/system-reminder-extra-usage-active-notice.md) | Indicator that extra usage is now being used. | 4 | 1.0.128 | 1.0.128 |
| [`system-reminder-detect-conversation-features.md`](../system-prompts/system-reminder-detect-conversation-features.md) | Instruction to analyze user messages to detect interaction features. | 16 | 1.0.122 | 1.0.122 |
| [`system-reminder-binary-content-placeholder.md`](../system-prompts/system-reminder-binary-content-placeholder.md) | Wraps an expression as labeled binary content within bracketed placeholder markup. | 11 | 1.0.118 | 1.0.118 |
| [`system-reminder-other-users-modified-files.md`](../system-prompts/system-reminder-other-users-modified-files.md) | Display the list of files modified by other users. | 13 | 1.0.109 | 1.0.109 |
| [`system-reminder-user-modified-files.md`](../system-prompts/system-reminder-user-modified-files.md) | Display the list of files modified by the current user. | 12 | 1.0.109 | 1.0.109 |
| [`system-reminder-active-style-guidelines.md`](../system-prompts/system-reminder-active-style-guidelines.md) | Reminder that the active output style must be followed exactly for responses. | 21 | 1.0.78 | 1.0.78 |
| [`system-reminder-address-user-message.md`](../system-prompts/system-reminder-address-user-message.md) | Address the user’s provided message and continue ongoing tasks accordingly. | 25 | 1.0.73 | 1.0.73 |
| [`system-reminder-combine-two-expressions.md`](../system-prompts/system-reminder-combine-two-expressions.md) | Comma-separated coordination of two expression placeholders with “and” in a single phrase. | 13 | 1.0.70 | 1.0.70 |
| [`system-reminder-check-new-bash-output.md`](../system-prompts/system-reminder-check-new-bash-output.md) | Notifies that new Bash output is available to view. | 17 | 1.0.69 | 1.0.69 |
| [`system-reminder-exit-status.md`](../system-prompts/system-reminder-exit-status.md) | Reports the process exit code value for a completed command. | 10 | 1.0.69 | 1.0.69 |
| [`system-reminder-background-bash-run.md`](../system-prompts/system-reminder-background-bash-run.md) | Marks an identifier for a background Bash execution instance. | 9 | 1.0.69 | 1.0.69 |
| [`system-reminder-continued-session-warning.md`](../system-prompts/system-reminder-continued-session-warning.md) | Warns session resumed on another machine and reports updated working directory path. | 26 | 1.0.68 | 1.0.68 |
| [`system-reminder-show-existing-todo-list.md`](../system-prompts/system-reminder-show-existing-todo-list.md) | Shows the current todo list contents inside a bracketed placeholder. | 19 | 1.0.52 | 1.0.94 |
| [`system-reminder-ide-file-opened-context.md`](../system-prompts/system-reminder-ide-file-opened-context.md) | Indicates the user opened a specific IDE file that may relate to task. | 27 | 1.0.32 | 1.0.32 |
| [`system-reminder-mcp-resource-no-content.md`](../system-prompts/system-reminder-mcp-resource-no-content.md) | MCP resource tag referencing server and URI placeholders, indicating no content available. | 29 | 1.0.19 | 1.0.19 |
| [`system-reminder-full-resource-contents-header.md`](../system-prompts/system-reminder-full-resource-contents-header.md) | Introduces the full contents of a referenced resource. | 5 | 1.0.19 | 1.0.19 |
| [`system-reminder-report-new-diagnostic-issues.md`](../system-prompts/system-reminder-report-new-diagnostic-issues.md) | Announces newly detected diagnostic issues and prints the associated details block. | 27 | 1.0.18 | 1.0.94 |
| [`system-reminder-call-error-result.md`](../system-prompts/system-reminder-call-error-result.md) | Template line reporting an error result from a specified tool call. | 13 | 0.2.119 | 0.2.119 |
| [`system-reminder-empty-existing-file-warning.md`](../system-prompts/system-reminder-empty-existing-file-warning.md) | Warns that a referenced file exists but has no contents. | 22 | 0.2.115 | 1.0.53 |
| [`system-reminder-summarize-conversation.md`](../system-prompts/system-reminder-summarize-conversation.md) | Directs the assistant to summarize conversations. | 13 | 0.2.108 | 0.2.108 |
| [`system-reminder-web-search.md`](../system-prompts/system-reminder-web-search.md) | Sets the assistant to perform web search tool use. | 11 | 0.2.108 | 0.2.108 |
| [`system-reminder-show-variable-contents.md`](../system-prompts/system-reminder-show-variable-contents.md) | Show contents of a referenced variable or expression with its resolved value. | 16 | 0.2.107 | 0.2.107 |
| [`system-reminder-call-echo-line.md`](../system-prompts/system-reminder-call-echo-line.md) | Log line noting a tool invocation and the exact input provided. | 20 | 0.2.106 | 0.2.106 |
| [`system-reminder-call-result.md`](../system-prompts/system-reminder-call-result.md) | Report the result returned from invoking a specified tool. | 18 | 0.2.106 | 0.2.106 |

</details>
