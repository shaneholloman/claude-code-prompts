# System Prompts Index – by tokens

- Total prompt files: **276**

## Categories

- System prompts (81)
- Tool prompts (66)
- Agent prompts (3)
- System data (85)
- System reminders (41)

## System prompts (81)

_Sorted by tokens (desc)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-prompt-run-bash-commands-safely.md`](../system-prompts/system-prompt-run-bash-commands-safely.md) | Run a bash command with directory checks, quoting rules, and configurable timeout. | 2,886 | 1.0.81 | 1.0.85 |
| [`system-prompt-security-review-git-diff.md`](../system-prompts/system-prompt-security-review-git-diff.md) | Performs a high-confidence vulnerability review of branch changes using git status, logs, and diffs. | 2,808 | 1.0.69 | 1.0.69 |
| [`system-prompt-structured-coding-todo-list.md`](../system-prompts/system-prompt-structured-coding-todo-list.md) | Guide creating and updating a structured todo list for complex coding sessions. | 2,330 | 1.0.86 | 1.0.86 |
| [`system-prompt-dev-conversation-summary.md`](../system-prompts/system-prompt-dev-conversation-summary.md) | Produce a chronological, technically detailed conversation summary with structured analysis notes. | 1,263 | 1.0.14 | 1.0.87 |
| [`system-prompt-dev-conversation-summary-2.md`](../system-prompts/system-prompt-dev-conversation-summary-2.md) | Multiple prompts (2) | 1,252 | 1.0.14 | 1.0.87 |
| [`system-prompt-architect-configs-from-needs.md`](../system-prompts/system-prompt-architect-configs-from-needs.md) | Translate user requirements and project context into precise agent specifications. | 1,140 | 1.0.60 | 1.0.60 |
| [`system-prompt-learn-by-doing-human-input.md`](../system-prompts/system-prompt-learn-by-doing-human-input.md) | Request 3–5 line human code contributions for key logic, tracked via TodoList prompts. | 1,137 | 1.0.78 | 1.0.86 |
| [`system-prompt-delegate-work-to-specialists.md`](../system-prompts/system-prompt-delegate-work-to-specialists.md) | Choose correct subagent type and tools for multi-step work using routing guidelines. | 896 | 1.0.64 | 1.0.72 |
| [`system-prompt-pull-request-review-workflow.md`](../system-prompts/system-prompt-pull-request-review-workflow.md) | GitHub Actions workflow runs Claude code review on pull request open or sync. | 723 | 1.0.71 | 1.0.71 |
| [`system-prompt-bash-command-prefix-injection-detection.md`](../system-prompts/system-prompt-bash-command-prefix-injection-detection.md) | Define command prefix extraction and injection detection with illustrative shell command examples. | 693 | 1.0.23 | 1.0.34 |
| [`system-prompt-xml-decision-for-log-summary.md`](../system-prompts/system-prompt-xml-decision-for-log-summary.md) | Determine if command output is log spew and respond with XML indicating summary decision and content. | 657 | 1.0.60 | 1.0.60 |
| [`system-prompt-batch-edits-single-file.md`](../system-prompts/system-prompt-batch-edits-single-file.md) | Instructions for making multiple exact replacements in one file after reading context. | 628 | 1.0.8 | 1.0.8 |
| [`system-prompt-update-session-notes-file.md`](../system-prompts/system-prompt-update-session-notes-file.md) | Single MultiEdit updates existing session file content only, preserving headers and italic descriptions. | 498 | 1.0.87 | 1.0.87 |
| [`system-prompt-fetch-pr-comments.md`](../system-prompts/system-prompt-fetch-pr-comments.md) | Fetch PR-level and review comments via gh API, then format threads with diffs. | 444 | 0.2.9 | 0.2.9 |
| [`system-prompt-read-local-files-by-path.md`](../system-prompts/system-prompt-read-local-files-by-path.md) | Reads local filesystem files by absolute path with optional line ranges and image viewing. | 396 | 1.0.58 | 1.0.87 |
| [`system-prompt-install-github-app.md`](../system-prompts/system-prompt-install-github-app.md) | Explains adding a workflow to enable Claude Code via @claude mentions after merge. | 393 | 1.0.44 | 1.0.44 |
| [`system-prompt-create-md-guide-2.md`](../system-prompts/system-prompt-create-md-guide-2.md) | Analyze the repo and draft or improve a CLAUDE.md with commands and architecture. | 382 | 0.2.101 | 0.2.101 |
| [`system-prompt-conversation-title-writer.md`](../system-prompts/system-prompt-conversation-title-writer.md) | Generates a fixed-length title from the most recent conversation messages. | 315 | 1.0.86 | 1.0.86 |
| [`system-prompt-extract-displayed-file-paths.md`](../system-prompts/system-prompt-extract-displayed-file-paths.md) | Identify and return only explicitly shown file paths when file contents are displayed. | 289 | 1.0.8 | 1.0.8 |
| [`system-prompt-exact-string-edits-in-files.md`](../system-prompts/system-prompt-exact-string-edits-in-files.md) | Define rules for exact in-file string replacements after reading and with unique matches. | 258 | 1.0.8 | 1.0.8 |
| [`system-prompt-review-github-pull-request.md`](../system-prompts/system-prompt-review-github-pull-request.md) | Use GitHub CLI to list/view PRs, fetch diff, and deliver structured code review. | 233 | 0.2.9 | 0.2.9 |
| [`system-prompt-educational-insights-cli.md`](../system-prompts/system-prompt-educational-insights-cli.md) | CLI engineering assistant adds codebase-specific insights before and after coding in formatted blocks | 220 | 1.0.78 | 1.0.78 |
| [`system-prompt-export-aliases-filter-winpty.md`](../system-prompts/system-prompt-export-aliases-filter-winpty.md) | Writes aliases into the snapshot while filtering winpty aliases on Windows. | 218 | 1.0.65 | 1.0.65 |
| [`system-prompt-generate-github-issue-title.md`](../system-prompts/system-prompt-generate-github-issue-title.md) | Creates a concise technical GitHub issue title from a bug report. | 205 | 1.0.46 | 1.0.46 |
| [`system-prompt-snapshot-functions-base64-encode.md`](../system-prompts/system-prompt-snapshot-functions-base64-encode.md) | Captures user functions by base64 encoding definitions and writing eval restore lines. | 200 | 1.0.65 | 1.0.65 |
| [`system-prompt-coding-session-title-generator.md`](../system-prompts/system-prompt-coding-session-title-generator.md) | Generate a concise XML-wrapped title from the provided coding session description. | 198 | 1.0.68 | 1.0.76 |
| [`system-prompt-session-summary-template-sections.md`](../system-prompts/system-prompt-session-summary-template-sections.md) | Provides a structured template for summarizing task, worklog, codebase, workflow, corrections, and learnings. | 190 | 1.0.87 | 1.0.87 |
| [`system-prompt-create-shell-snapshot-file-2.md`](../system-prompts/system-prompt-create-shell-snapshot-file-2.md) | Initialize a snapshot shell file, unalias all, then append additional generated content. | 182 | 1.0.65 | 1.0.65 |
| [`system-prompt-coding-session-title-generator-2.md`](../system-prompts/system-prompt-coding-session-title-generator-2.md) | Creates a short XML-wrapped title from a coding session description. | 167 | 1.0.68 | 1.0.76 |
| [`system-prompt-write-file-with-constraints.md`](../system-prompts/system-prompt-write-file-with-constraints.md) | Defines rules for writing files, including reading before overwriting and avoiding new docs. | 145 | 1.0.7 | 1.0.7 |
| [`system-prompt-cite-with-limited-quotes.md`](../system-prompts/system-prompt-cite-with-limited-quotes.md) | Multiple prompts (2) | 140 | 0.2.40 | 1.0.87 |
| [`system-prompt-educational-insights.md`](../system-prompts/system-prompt-educational-insights.md) | Enforces brief pre/post code educational insights using a named insight banner format. | 134 | 1.0.63 | 1.0.64 |
| [`system-prompt-nested-template-functions.md`](../system-prompts/system-prompt-nested-template-functions.md) | Nested compiled template functions that concatenate output into a string buffer. | 134 | 0.2.54 | 1.0.86 |
| [`system-prompt-conversation-title-with-pattern.md`](../system-prompts/system-prompt-conversation-title-with-pattern.md) | Compose a NUM-NUM word conversation title from recent messages, matching EXPR_4 pattern. | 129 | 1.0.77 | 1.0.77 |
| [`system-prompt-file-editing-and-response-rules.md`](../system-prompts/system-prompt-file-editing-and-response-rules.md) | Guidelines to avoid creating files, prefer edits, and use absolute paths without emojis. | 129 | 1.0.59 | 1.0.59 |
| [`system-prompt-create-view-instrument-selector.md`](../system-prompts/system-prompt-create-view-instrument-selector.md) | Create a new view with specified name, optional description, and InstrumentSelector variants. | 110 | 0.2.76 | 0.2.76 |
| [`system-prompt-snapshot-functions-typeset-dump.md`](../system-prompts/system-prompt-snapshot-functions-typeset-dump.md) | Captures user function definitions via typeset and writes them directly to the snapshot. | 110 | 1.0.65 | 1.0.65 |
| [`system-prompt-default-ops-no-network.md`](../system-prompts/system-prompt-default-ops-no-network.md) | Default-allow policy denying all network except localhost proxy bind/inbound/outbound ports. | 106 | 1.0.87 | 1.0.87 |
| [`system-prompt-record-shell-options-snapshot.md`](../system-prompts/system-prompt-record-shell-options-snapshot.md) | Appends current shell options and enables expand_aliases in the snapshot. | 100 | 1.0.65 | 1.0.65 |
| [`system-prompt-redirect-detected.md`](../system-prompts/system-prompt-redirect-detected.md) | Request WebFetch rerun to retrieve content from redirected host URL with new parameters. | 97 | 1.0.52 | 1.0.74 |
| [`system-prompt-select-core-frequently-modified-files.md`](../system-prompts/system-prompt-select-core-frequently-modified-files.md) | Choose five diverse frequently modified core-logic filenames from git history stats. | 90 | 0.2.9 | 0.2.9 |
| [`system-prompt-detect-new-topic-title.md`](../system-prompts/system-prompt-detect-new-topic-title.md) | Detect whether a message starts a new topic and extract a short title. | 85 | 0.2.9 | 0.2.9 |
| [`system-prompt-check-rg-and-alias.md`](../system-prompts/system-prompt-check-rg-and-alias.md) | Append snapshot logic to check for rg command and define a fallback alias. | 82 | 1.0.65 | 1.0.65 |
| [`system-prompt-summarize-shell-command.md`](../system-prompts/system-prompt-summarize-shell-command.md) | Write a brief input-output description of a shell command in a few words. | 78 | 0.2.59 | 0.2.59 |
| [`system-prompt-git-status-session-start.md`](../system-prompts/system-prompt-git-status-session-start.md) | Record initial git status snapshot, including current branch and main branch names. | 77 | 0.2.32 | 1.0.74 |
| [`system-prompt-fix-missing-executable-name.md`](../system-prompts/system-prompt-fix-missing-executable-name.md) | Advise fixes when a specified CLI subcommand executable path is missing. | 76 | 1.0.56 | 1.0.56 |
| [`system-prompt-list-mcp-server-resources.md`](../system-prompts/system-prompt-list-mcp-server-resources.md) | Lists available resources across MCP servers with optional server filtering. | 73 | 1.0.22 | 1.0.22 |
| [`system-prompt-read-mcp-server-resource.md`](../system-prompts/system-prompt-read-mcp-server-resource.md) | Reads a resource from an MCP server by server name and URI. | 73 | 1.0.22 | 1.0.22 |
| [`system-prompt-exit-transcript-rules.md`](../system-prompts/system-prompt-exit-transcript-rules.md) | Specifies how stdout and stderr are displayed for tool call inputs and responses by exit code. | 70 | 1.0.53 | 1.0.53 |
| [`system-prompt-exit-handling.md`](../system-prompts/system-prompt-exit-handling.md) | Defines stdout and stderr visibility rules based on command exit code for tool calls. | 62 | 1.0.53 | 1.0.53 |
| [`system-prompt-replace-all-occurrences-warning.md`](../system-prompts/system-prompt-replace-all-occurrences-warning.md) | Warns about multiple replacement matches when replace_all is false, requesting unique context. | 61 | 1.0.18 | 1.0.74 |
| [`system-prompt-verify-repo-access-scope.md`](../system-prompts/system-prompt-verify-repo-access-scope.md) | Validate GitHub repository name, access permissions, and token scopes for private repos. | 61 | 1.0.25 | 1.0.25 |
| [`system-prompt-simple-conversation-title.md`](../system-prompts/system-prompt-simple-conversation-title.md) | Generate a NUM–NUM word conversation title using the last EXPR_1 of EXPR_2 messages. | 60 | 1.0.77 | 1.0.77 |
| [`system-prompt-command-exit-handling.md`](../system-prompts/system-prompt-command-exit-handling.md) | Defines JSON input expectations and exit code behaviors. | 59 | 1.0.55 | 1.0.56 |
| [`system-prompt-compaction-command-exit-codes.md`](../system-prompts/system-prompt-compaction-command-exit-codes.md) | Defines JSON input handling and exit-code behavior for compaction commands. | 55 | 1.0.53 | 1.0.53 |
| [`system-prompt-summarize-bash-output-if-needed.md`](../system-prompts/system-prompt-summarize-bash-output-if-needed.md) | Assess whether command output merits summarization, then summarize key relevant details. | 55 | 1.0.60 | 1.0.74 |
| [`system-prompt-github-permission-troubleshooting.md`](../system-prompts/system-prompt-github-permission-troubleshooting.md) | Provide quick fixes for common GitHub CLI permission and authorization issues. | 54 | 1.0.28 | 1.0.28 |
| [`system-prompt-github-repo-access-help.md`](../system-prompts/system-prompt-github-repo-access-help.md) | List common GitHub CLI repository access errors and the steps to resolve them. | 52 | 1.0.28 | 1.0.28 |
| [`system-prompt-summarize-bash-output-if-needed-2.md`](../system-prompts/system-prompt-summarize-bash-output-if-needed-2.md) | Assess whether command output merits summarization, then summarize key relevant details. | 50 | 1.0.60 | 1.0.74 |
| [`system-prompt-codebase-and-user.md`](../system-prompts/system-prompt-codebase-and-user.md) | Directive that codebase and user instructions override default behavior with settings scope labels. | 49 | 1.0.38 | 1.0.38 |
| [`system-prompt-handle-exit-codes-and-output.md`](../system-prompts/system-prompt-handle-exit-codes-and-output.md) | Routes stdout and stderr visibility based on exit code and continues execution when needed. | 49 | 1.0.53 | 1.0.53 |
| [`system-prompt-exit-output-handling.md`](../system-prompts/system-prompt-exit-output-handling.md) | Route stdout and stderr visibility based on exit codes. | 45 | 1.0.53 | 1.0.53 |
| [`system-prompt-fix-settings-json-validation.md`](../system-prompts/system-prompt-fix-settings-json-validation.md) | Analyze Claude Code settings.json validation failure using provided error text and schema, no env changes. | 45 | 1.0.82 | 1.0.82 |
| [`system-prompt-install-github-cli.md`](../system-prompts/system-prompt-install-github-cli.md) | Install GitHub CLI across macOS, Windows, and Linux. | 41 | 1.0.0 | 1.0.0 |
| [`system-prompt-show-updated-file-snippet.md`](../system-prompts/system-prompt-show-updated-file-snippet.md) | Report that a file was updated and show a numbered snippet from it. | 41 | 1.0.30 | 1.0.30 |
| [`system-prompt-cell-settings-xml-snippet.md`](../system-prompts/system-prompt-cell-settings-xml-snippet.md) | XML-like cell element embedding settings scope text and a nested path tag. | 40 | 1.0.38 | 1.0.38 |
| [`system-prompt-command-json-exit-handling.md`](../system-prompts/system-prompt-command-json-exit-handling.md) | Rules for JSON command input and exit code output handling. | 40 | 1.0.64 | 1.0.64 |
| [`system-prompt-continue-last-task.md`](../system-prompts/system-prompt-continue-last-task.md) | Continue from prior conversation state and resume the last task without questions. | 38 | 0.2.54 | 0.2.54 |
| [`system-prompt-file-updated-snippet-output.md`](../system-prompts/system-prompt-file-updated-snippet-output.md) | Notify that a file was updated and show numbered snippet output from cat -n. | 38 | 0.2.9 | 0.2.9 |
| [`system-prompt-json-command-exit-rules.md`](../system-prompts/system-prompt-json-command-exit-rules.md) | Defines JSON input and exit code handling for a command, showing stderr only on failure. | 34 | 1.0.85 | 1.0.85 |
| [`system-prompt-admin-setup-secrets-apps.md`](../system-prompts/system-prompt-admin-setup-secrets-apps.md) | Have a repository admin install apps and configure secrets when setup fails. | 33 | 1.0.0 | 1.0.0 |
| [`system-prompt-classify-bash-command-prefix.md`](../system-prompts/system-prompt-classify-bash-command-prefix.md) | Determine the appropriate prefix for bash commands requested by a coding agent. | 33 | 0.2.9 | 0.2.9 |
| [`system-prompt-summarize-coding-chat-status.md`](../system-prompts/system-prompt-summarize-coding-chat-status.md) | Condense a coding conversation into a character-limited status recap. | 33 | 0.2.91 | 0.2.91 |
| [`system-prompt-create-statusline-setup-task.md`](../system-prompts/system-prompt-create-statusline-setup-task.md) | Creates a task that invokes the statusline setup subagent. | 31 | 1.0.72 | 1.0.72 |
| [`system-prompt-malicious-files-refusal-check.md`](../system-prompts/system-prompt-malicious-files-refusal-check.md) | Checks whether listed files seem malicious and mandates refusal if suspicious. | 30 | 0.2.89 | 0.2.89 |
| [`system-prompt-use-owner-path-format.md`](../system-prompts/system-prompt-use-owner-path-format.md) | Use the owner and path or URL format for repository references. | 28 | 1.0.0 | 1.0.0 |
| [`system-prompt-applied-edits-to-settings.md`](../system-prompts/system-prompt-applied-edits-to-settings.md) | Reports that a number of edits were applied to local settings scopes. | 27 | 1.0.38 | 1.0.38 |
| [`system-prompt-authenticate-with-gh-cli.md`](../system-prompts/system-prompt-authenticate-with-gh-cli.md) | Authenticate to GitHub using gh auth login or environment-based methods. | 25 | 1.0.0 | 1.0.0 |
| [`system-prompt-hook-json-schema-validation.md`](../system-prompts/system-prompt-hook-json-schema-validation.md) | Indicates hook JSON validation failed and shows error details plus expected schema. | 24 | 1.0.38 | 1.0.38 |
| [`system-prompt-avoid-rereading-unchanged-resource.md`](../system-prompts/system-prompt-avoid-rereading-unchanged-resource.md) | Instructs to not reread a resource unless it may have changed. | 22 | 1.0.19 | 1.0.19 |
| [`system-prompt-stop-hook-feedback-links.md`](../system-prompts/system-prompt-stop-hook-feedback-links.md) | Stop hook feedback message with referenced URLs. | 18 | 1.0.38 | 1.0.38 |

## Tool prompts (66)

_Sorted by tokens (desc)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`tool-description-structured-todo-list-guidelines.md`](../system-prompts/tool-description-structured-todo-list-guidelines.md) | Criteria for starting, updating, and avoiding a structured todo tool during coding sessions | 2,335 | 1.0.86 | 1.0.86 |
| [`tool-description-collaborative-learning-cli.md`](../system-prompts/tool-description-collaborative-learning-cli.md) | Interactive CLI that blends task completion with learning by requesting meaningful human code contributions. | 1,009 | 1.0.78 | 1.0.78 |
| [`tool-description-safe-bash-command-execution.md`](../system-prompts/tool-description-safe-bash-command-execution.md) | Execute bash in persistent session with directory verification, path quoting, and timeout limits | 700 | 1.0.86 | 1.0.86 |
| [`tool-description-multi-edit-file-operations.md`](../system-prompts/tool-description-multi-edit-file-operations.md) | Explains multi-edit single-file replacement tool built on another tool, with sequencing rules. | 645 | 1.0.8 | 1.0.8 |
| [`tool-description-read-local-file-paths.md`](../system-prompts/tool-description-read-local-file-paths.md) | Reads local filesystem files by absolute path with optional line ranges and image viewing. | 396 | 1.0.58 | 1.0.87 |
| [`tool-description-fetch-and-analyze-web-content.md`](../system-prompts/tool-description-fetch-and-analyze-web-content.md) | Describes a tool that fetches a URL, converts HTML to markdown, and analyzes it with a small model. | 272 | 1.0.42 | 1.0.42 |
| [`tool-description-exact-file-string-replacement.md`](../system-prompts/tool-description-exact-file-string-replacement.md) | Describes exact in-file replacement tool rules, requiring prior read and unique old_string. | 263 | 1.0.8 | 1.0.8 |
| [`tool-description-ripgrep-search-guidelines.md`](../system-prompts/tool-description-ripgrep-search-guidelines.md) | Guidelines for using the Grep search tool with regex, filters, and output modes. | 250 | 1.0.38 | 1.0.38 |
| [`tool-description-exit-planning-when-ready.md`](../system-prompts/tool-description-exit-planning-when-ready.md) | Instructs when to trigger leaving planning mode before starting implementation. | 180 | 1.0.32 | 1.0.57 |
| [`tool-description-web-search-current-info.md`](../system-prompts/tool-description-web-search-current-info.md) | Searches the web for up-to-date information and returns formatted result blocks. | 159 | 1.0.40 | 1.0.40 |
| [`tool-description-write-file-after-reading-existing.md`](../system-prompts/tool-description-write-file-after-reading-existing.md) | Write files, reading existing contents first, and avoid unrequested new or documentation files. | 150 | 1.0.7 | 1.0.9 |
| [`tool-description-fast-glob-file-matching-2.md`](../system-prompts/tool-description-fast-glob-file-matching-2.md) | Glob-based file matcher returning paths sorted by modification time and supports batching searches. | 118 | 0.2.116 | 0.2.116 |
| [`tool-description-replace-jupyter-notebook-cell.md`](../system-prompts/tool-description-replace-jupyter-notebook-cell.md) | Replaces, inserts, or deletes a specific Jupyter notebook cell by index. | 117 | 0.2.9 | 0.2.83 |
| [`tool-description-check-background-bash-output.md`](../system-prompts/tool-description-check-background-bash-output.md) | Tool to read only new output from a running or completed background bash shell. | 97 | 1.0.72 | 1.0.72 |
| [`tool-description-educational-cli-engineering-help.md`](../system-prompts/tool-description-educational-cli-engineering-help.md) | Interactive CLI for engineering tasks with educational codebase insights under an explanatory style. | 92 | 1.0.78 | 1.0.78 |
| [`tool-description-list-configured-mcp-resources.md`](../system-prompts/tool-description-list-configured-mcp-resources.md) | Tool to list MCP resources from all or a specified server including server field. | 74 | 1.0.22 | 1.0.22 |
| [`tool-description-kill-background-bash-shell.md`](../system-prompts/tool-description-kill-background-bash-shell.md) | Terminate a running background bash shell by shell id and return status. | 65 | 1.0.60 | 1.0.68 |
| [`tool-description-list-path-with-ignore-globs.md`](../system-prompts/tool-description-list-path-with-ignore-globs.md) | Lists files and directories at an absolute path with optional ignore glob patterns. | 60 | 0.2.29 | 0.2.83 |
| [`tool-description-read-resource-by-uri.md`](../system-prompts/tool-description-read-resource-by-uri.md) | Tool to read an MCP resource by server name and resource URI. | 54 | 1.0.22 | 1.0.22 |
| [`tool-description-clear-chat-keep-summary.md`](../system-prompts/tool-description-clear-chat-keep-summary.md) | Clears conversation history while retaining a summary in context. | 24 | 0.2.54 | 0.2.57 |
| [`tool-description-show-status-details.md`](../system-prompts/tool-description-show-status-details.md) | Command to display Claude Code status, version, model, connectivity, and tools. | 18 | 1.0.4 | 1.0.4 |
| [`tool-description-bus-error-message.md`](../system-prompts/tool-description-bus-error-message.md) | Reports a bus error from misaligned or invalid memory access. | 16 | 1.0.68 | 1.0.68 |
| [`tool-description-option-enter-newline-binding.md`](../system-prompts/tool-description-option-enter-newline-binding.md) | Enable Option+Enter to insert newlines. | 12 | 0.2.80 | 0.2.83 |
| [`tool-description-paused-by-ctrl-z-or-suspend.md`](../system-prompts/tool-description-paused-by-ctrl-z-or-suspend.md) | Marks the process as stopped via job-control suspend. | 12 | 1.0.68 | 1.0.68 |
| [`tool-description-upgrade-to-max-rate-limits.md`](../system-prompts/tool-description-upgrade-to-max-rate-limits.md) | Promotes upgrading to Max to get higher rate limits and more Opus access. | 12 | 1.0.11 | 1.0.11 |
| [`tool-description-verify-setup.md`](../system-prompts/tool-description-verify-setup.md) | Diagnoses and verifies Claude Code installation and configuration settings. | 11 | 1.0.49 | 1.0.49 |
| [`tool-description-child-process-state-change.md`](../system-prompts/tool-description-child-process-state-change.md) | Multiple prompts (2) | 10 | 1.0.68 | 1.0.68 |
| [`tool-description-context-usage-grid.md`](../system-prompts/tool-description-context-usage-grid.md) | Renders current context usage as a colored grid visualization. | 10 | 1.0.86 | 1.0.86 |
| [`tool-description-set-output-style-menu.md`](../system-prompts/tool-description-set-output-style-menu.md) | Instruction to set the output style directly or via a selection menu. | 10 | 1.0.78 | 1.0.78 |
| [`tool-description-show-session-cost-and-duration.md`](../system-prompts/tool-description-show-session-cost-and-duration.md) | Displays the current session total cost and duration. | 10 | 0.2.9 | 0.2.9 |
| [`tool-description-ctrl-break-interruption.md`](../system-prompts/tool-description-ctrl-break-interruption.md) | Indicates the user interrupted execution with CTRL-BREAK. | 9 | 1.0.68 | 1.0.68 |
| [`tool-description-emulated-command-not-implemented.md`](../system-prompts/tool-description-emulated-command-not-implemented.md) | Indicates a command is expected to be emulated but has no implementation. | 9 | 1.0.68 | 1.0.68 |
| [`tool-description-export-conversation-to-file.md`](../system-prompts/tool-description-export-conversation-to-file.md) | Export the current conversation to a file or clipboard. | 9 | 1.0.44 | 1.0.44 |
| [`tool-description-migrate-npm-global-to-local.md`](../system-prompts/tool-description-migrate-npm-global-to-local.md) | Move from a global npm install to a project-local installation. | 9 | 0.2.51 | 0.2.51 |
| [`tool-description-application-specific-realtime-signal.md`](../system-prompts/tool-description-application-specific-realtime-signal.md) | Denotes receipt of an application-defined realtime signal. | 8 | 1.0.68 | 1.0.74 |
| [`tool-description-ctrl-backslash-user-interruption.md`](../system-prompts/tool-description-ctrl-backslash-user-interruption.md) | Captures a user quit signal triggered by CTRL-\ | 8 | 1.0.68 | 1.0.68 |
| [`tool-description-ctrl-c-user-interruption.md`](../system-prompts/tool-description-ctrl-c-user-interruption.md) | Captures an interactive user interrupt from CTRL-C. | 8 | 1.0.68 | 1.0.68 |
| [`tool-description-manage-ide-integrations-status.md`](../system-prompts/tool-description-manage-ide-integrations-status.md) | Manage IDE MCP integrations and display their status. | 8 | 0.2.126 | 1.0.0 |
| [`tool-description-manage-permissions.md`](../system-prompts/tool-description-manage-permissions.md) | Controls allow and deny rules for tool permissions. | 8 | 1.0.7 | 1.0.7 |
| [`tool-description-setup-github-actions.md`](../system-prompts/tool-description-setup-github-actions.md) | Sets up Claude GitHub Actions integration for a repository. | 8 | 0.2.101 | 0.2.101 |
| [`tool-description-sign-in-anthropic-account.md`](../system-prompts/tool-description-sign-in-anthropic-account.md) | Signs in using an Anthropic account. | 8 | 0.2.9 | 0.2.9 |
| [`tool-description-sign-out-anthropic-account.md`](../system-prompts/tool-description-sign-out-anthropic-account.md) | Signs out from an Anthropic account. | 8 | 0.2.9 | 0.2.9 |
| [`tool-description-socket-out-of-band-data.md`](../system-prompts/tool-description-socket-out-of-band-data.md) | Handle socket notifications for received out-of-band data. | 8 | 1.0.68 | 1.0.68 |
| [`tool-description-toggle-vim-editing-mode.md`](../system-prompts/tool-description-toggle-vim-editing-mode.md) | Switch between Vim and normal editing modes. | 8 | 0.2.54 | 0.2.54 |
| [`tool-description-background-process-terminal-output.md`](../system-prompts/tool-description-background-process-terminal-output.md) | Diagnose background process attempts to write to terminal output. | 7 | 1.0.68 | 1.0.68 |
| [`tool-description-clear-conversation-history.md`](../system-prompts/tool-description-clear-conversation-history.md) | Clears conversation history to free up context. | 7 | 0.2.9 | 0.2.9 |
| [`tool-description-manage-hook-configurations.md`](../system-prompts/tool-description-manage-hook-configurations.md) | Tool description for managing hook configurations for tool events. | 7 | 1.0.38 | 1.0.38 |
| [`tool-description-set.md`](../system-prompts/tool-description-set.md) | Set the Claude Code model selection. | 7 | 1.0.0 | 1.0.0 |
| [`tool-description-stack-empty-or-overflowed.md`](../system-prompts/tool-description-stack-empty-or-overflowed.md) | Indicates stack underflow or overflow was detected. | 7 | 1.0.68 | 1.0.68 |
| [`tool-description-background-process-terminal-read-blocked.md`](../system-prompts/tool-description-background-process-terminal-read-blocked.md) | Indicates a background job attempted to read from the controlling terminal. | 6 | 1.0.68 | 1.0.68 |
| [`tool-description-list-files-in-context.md`](../system-prompts/tool-description-list-files-in-context.md) | List all files currently available in context. | 6 | 0.2.79 | 0.2.79 |
| [`tool-description-manage-background-bash-shells.md`](../system-prompts/tool-description-manage-background-bash-shells.md) | Lists and controls background bash shell sessions. | 6 | 1.0.18 | 1.0.18 |
| [`tool-description-add-working-directory.md`](../system-prompts/tool-description-add-working-directory.md) | Add a new working directory. | 5 | 1.0.23 | 1.0.23 |
| [`tool-description-broken-pipe-or-socket.md`](../system-prompts/tool-description-broken-pipe-or-socket.md) | Occurs when writing to a closed pipe or disconnected socket. | 5 | 1.0.68 | 1.0.68 |
| [`tool-description-device-running-out-of-power.md`](../system-prompts/tool-description-device-running-out-of-power.md) | Warns that the device is running low on power. | 5 | 1.0.68 | 1.0.68 |
| [`tool-description-floating-point-arithmetic-error.md`](../system-prompts/tool-description-floating-point-arithmetic-error.md) | Signals a floating-point arithmetic exception occurred. | 5 | 1.0.68 | 1.0.68 |
| [`tool-description-install-native-build.md`](../system-prompts/tool-description-install-native-build.md) | Install the native build of Claude Code. | 5 | 1.0.31 | 1.0.31 |
| [`tool-description-show-help-and-commands.md`](../system-prompts/tool-description-show-help-and-commands.md) | Displays help text and available commands. | 5 | 0.2.9 | 0.2.9 |
| [`tool-description-submit-feedback.md`](../system-prompts/tool-description-submit-feedback.md) | Submits user feedback about Claude Code. | 5 | 0.2.9 | 0.2.9 |
| [`tool-description-application-specific-signal.md`](../system-prompts/tool-description-application-specific-signal.md) | Multiple prompts (2) | 4 | 1.0.68 | 1.0.68 |
| [`tool-description-edit-memory-files.md`](../system-prompts/tool-description-edit-memory-files.md) | Edit Claude memory files. | 4 | 0.2.54 | 0.2.54 |
| [`tool-description-manage-configurations.md`](../system-prompts/tool-description-manage-configurations.md) | Create and maintain agent configuration settings. | 4 | 1.0.60 | 1.0.60 |
| [`tool-description-request-process-information.md`](../system-prompts/tool-description-request-process-information.md) | Represents a request to report current process status information. | 4 | 1.0.68 | 1.0.68 |
| [`tool-description-terminal-window-size-changed.md`](../system-prompts/tool-description-terminal-window-size-changed.md) | React to terminal window size change events. | 4 | 1.0.68 | 1.0.68 |
| [`tool-description-invalid-machine.md`](../system-prompts/tool-description-invalid-machine.md) | Reports an invalid or unsupported CPU instruction was executed. | 3 | 1.0.68 | 1.0.68 |
| [`tool-description-resume-conversation-session.md`](../system-prompts/tool-description-resume-conversation-session.md) | Requests resuming a prior conversation. | 3 | 1.0.26 | 1.0.26 |

## Agent prompts (3)

_Sorted by tokens (desc)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`agent-prompt-configure-statusline.md`](../system-prompts/agent-prompt-configure-statusline.md) | Create or update a Claude Code statusLine by converting shell PS1 settings. | 1,055 | 1.0.81 | 1.0.81 |
| [`agent-prompt-custom-output-style-config.md`](../system-prompts/agent-prompt-custom-output-style-config.md) | Derive user preferences and generate a configuration for a custom output style. | 743 | 1.0.84 | 1.0.84 |
| [`agent-prompt-codebase-search-analysis-guide.md`](../system-prompts/agent-prompt-codebase-search-analysis-guide.md) | Guidance for searching and analyzing multiple files in a codebase without creating files. | 287 | 1.0.45 | 1.0.78 |

## System data (85)

_Sorted by tokens (desc)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-data-character-mapping-table.md`](../system-prompts/system-data-character-mapping-table.md) | Contains numeric sequences and letter markers resembling a mapping table. | 184,755 | 1.0.32 | 1.0.32 |
| [`system-data-wolfram-language-symbols-list.md`](../system-prompts/system-data-wolfram-language-symbols-list.md) | Alphabetical list of Wolfram Language built-in symbol names. | 35,789 | 0.2.9 | 0.2.9 |
| [`system-data-stan-functions-reference-list.md`](../system-prompts/system-data-stan-functions-reference-list.md) | Partial catalog of Stan math, RNG, and distribution functions. | 2,155 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-placeholder-sequence.md`](../system-prompts/system-data-numeric-placeholder-sequence.md) | Repeated numeric placeholder tokens in a long sequence. | 1,791 | 0.2.9 | 0.2.9 |
| [`system-data-truncated-numeric-placeholders.md`](../system-prompts/system-data-truncated-numeric-placeholders.md) | Truncated stream of numeric placeholders. | 1,119 | 1.0.59 | 1.0.59 |
| [`system-data-html-doctype-variants-list-2.md`](../system-prompts/system-data-html-doctype-variants-list-2.md) | Strings enumerating HTML doctype variants including strict, levels, and internet explorer. | 1,099 | 0.2.9 | 1.0.84 |
| [`system-data-html-doctype-variants-list.md`](../system-prompts/system-data-html-doctype-variants-list.md) | Strings enumerating HTML doctype variants including strict, levels, and internet explorer. | 1,063 | 0.2.9 | 1.0.84 |
| [`system-data-sql-keywords-current-array.md`](../system-prompts/system-data-sql-keywords-current-array.md) | List of SQL reserved words and functions including current and array terms. | 1,000 | 0.2.9 | 0.2.9 |
| [`system-data-pattern-and-settings-blocks.md`](../system-prompts/system-data-pattern-and-settings-blocks.md) | Defines a pattern field alongside hidden settings and numeric placeholders. | 948 | 1.0.87 | 1.0.87 |
| [`system-data-repeated-numeric-placeholders.md`](../system-prompts/system-data-repeated-numeric-placeholders.md) | Long sequence of repeated numeric placeholder tokens. | 895 | 0.2.9 | 0.2.9 |
| [`system-data-julia-base-types-list.md`](../system-prompts/system-data-julia-base-types-list.md) | List of Julia core types and standard library names. | 723 | 0.2.9 | 0.2.9 |
| [`system-data-perl-builtin-functions-list.md`](../system-prompts/system-data-perl-builtin-functions-list.md) | List of Perl keywords and built-in functions. | 682 | 0.2.9 | 0.2.9 |
| [`system-data-extended-numeric-placeholders.md`](../system-prompts/system-data-extended-numeric-placeholders.md) | Extended list of numeric placeholder values. | 678 | 1.0.59 | 1.0.59 |
| [`system-data-github-events-trigger.md`](../system-prompts/system-data-github-events-trigger.md) | GitHub Actions workflow triggers Claude Code job when @claude appears in events. | 648 | 1.0.71 | 1.0.71 |
| [`system-data-numeric-placeholder-list.md`](../system-prompts/system-data-numeric-placeholder-list.md) | Repeated numeric placeholders in a long list. | 573 | 0.2.125 | 0.2.125 |
| [`system-data-dom-exception-messages-codes.md`](../system-prompts/system-data-dom-exception-messages-codes.md) | DOM exception names with placeholder numeric codes and messages. | 532 | 0.2.33 | 0.2.33 |
| [`system-data-numeric-placeholder-block.md`](../system-prompts/system-data-numeric-placeholder-block.md) | Block of repeated numeric placeholder tokens. | 531 | 0.2.9 | 0.2.9 |
| [`system-data-http-header-field-list.md`](../system-prompts/system-data-http-header-field-list.md) | List of HTTP request and response header fields including CORS and CSP. | 501 | 0.2.125 | 0.2.125 |
| [`system-data-hidden-args-settings-data.md`](../system-prompts/system-data-hidden-args-settings-data.md) | Settings data including hidden flag and args parameters. | 482 | 1.0.86 | 1.0.86 |
| [`system-data-numeric-placeholders-sequence.md`](../system-prompts/system-data-numeric-placeholders-sequence.md) | Sequence of numeric placeholder lines. | 454 | 1.0.59 | 1.0.59 |
| [`system-data-numeric-placeholders-dump.md`](../system-prompts/system-data-numeric-placeholders-dump.md) | Multiple prompts (10) | 447 | 1.0.59 | 1.0.59 |
| [`system-data-args-and-settings-payload.md`](../system-prompts/system-data-args-and-settings-payload.md) | Large settings payload that appends an args section. | 437 | 1.0.86 | 1.0.86 |
| [`system-data-conversation-title-generator.md`](../system-prompts/system-data-conversation-title-generator.md) | Instruction to generate a short title from recent conversation messages. | 426 | 1.0.86 | 1.0.86 |
| [`system-data-ignore-caches-and-binaries.md`](../system-prompts/system-data-ignore-caches-and-binaries.md) | Ignore list for repos covering caches, media, archives, and binary data files. | 422 | 1.0.70 | 1.0.70 |
| [`system-data-hex-color-swatches-ccff.md`](../system-prompts/system-data-hex-color-swatches-ccff.md) | Sequence of hexadecimal color codes in CC/FF step combinations. | 387 | 0.2.9 | 0.2.9 |
| [`system-data-sentry-trace-settings-data.md`](../system-prompts/system-data-sentry-trace-settings-data.md) | Settings payload that includes a sentry trace identifier. | 377 | 1.0.86 | 1.0.86 |
| [`system-data-settings-placeholders-block.md`](../system-prompts/system-data-settings-placeholders-block.md) | Placeholder-filled block listing user, project, and local settings fields. | 372 | 1.0.87 | 1.0.87 |
| [`system-data-settings-scope-metadata.md`](../system-prompts/system-data-settings-scope-metadata.md) | Lists user, project, and local settings fields and related metadata. | 372 | 1.0.86 | 1.0.86 |
| [`system-data-local-settings-scope-data.md`](../system-prompts/system-data-local-settings-scope-data.md) | Local-prefixed settings data covering user, project, and local scopes. | 366 | 1.0.86 | 1.0.86 |
| [`system-data-months-weekdays-number-mapping.md`](../system-prompts/system-data-months-weekdays-number-mapping.md) | Month and weekday names paired with numeric placeholders. | 341 | 0.2.9 | 0.2.9 |
| [`system-data-settings-scope-variables.md`](../system-prompts/system-data-settings-scope-variables.md) | Placeholders and references for user, project, and local settings blocks. | 332 | 1.0.86 | 1.0.86 |
| [`system-data-sql-functions-json-regression.md`](../system-prompts/system-data-sql-functions-json-regression.md) | Catalog of SQL functions including JSON, analytics, and regression aggregates. | 297 | 0.2.9 | 0.2.9 |
| [`system-data-conversation-title-generator-2.md`](../system-prompts/system-data-conversation-title-generator-2.md) | Instruction to generate a short title from recent conversation messages. | 279 | 1.0.86 | 1.0.86 |
| [`system-data-settings-scopes-and-numbers.md`](../system-prompts/system-data-settings-scopes-and-numbers.md) | Settings scopes combined with expression fields and numeric values. | 260 | 1.0.84 | 1.0.84 |
| [`system-data-stan-distributions-list.md`](../system-prompts/system-data-stan-distributions-list.md) | Enumerates probability distributions used in modeling. | 244 | 0.2.9 | 0.2.9 |
| [`system-data-settings-scopes-data-fields.md`](../system-prompts/system-data-settings-scopes-data-fields.md) | Multiple prompts (5) | 241 | 1.0.84 | 1.0.84 |
| [`system-data-numeric-placeholders-repeated.md`](../system-prompts/system-data-numeric-placeholders-repeated.md) | Repeated numeric placeholder entries. | 237 | 0.2.9 | 0.2.9 |
| [`system-data-settings-failure-issues-report.md`](../system-prompts/system-data-settings-failure-issues-report.md) | Failure report listing issues and referencing settings scopes. | 232 | 1.0.86 | 1.0.86 |
| [`system-data-settings-urls-and-values.md`](../system-prompts/system-data-settings-urls-and-values.md) | Two URLs followed by user, project, and local settings content blocks. | 232 | 1.0.86 | 1.0.86 |
| [`system-data-css-selectors-pseudo-classes.md`](../system-prompts/system-data-css-selectors-pseudo-classes.md) | Comprehensive list of CSS pseudo-classes and pseudo-elements. | 228 | 0.2.9 | 0.2.9 |
| [`system-data-repeated-number-placeholders.md`](../system-prompts/system-data-repeated-number-placeholders.md) | Series of repeated numeric placeholder lines. | 223 | 1.0.59 | 1.0.59 |
| [`system-data-javascript-builtins-and-typed-arrays.md`](../system-prompts/system-data-javascript-builtins-and-typed-arrays.md) | Enumerates JavaScript globals, built-in objects, errors, and typed arrays. | 216 | 0.2.9 | 0.2.9 |
| [`system-data-conversation-title-generator-variables.md`](../system-prompts/system-data-conversation-title-generator-variables.md) | Compose a word title from the last messages using multiple inserted sections. | 207 | 1.0.77 | 1.0.77 |
| [`system-data-http-request-timing-milestones.md`](../system-prompts/system-data-http-request-timing-milestones.md) | Collect user/project/local settings plus HTTP request timing markers from redirect_start to response_end. | 199 | 1.0.84 | 1.0.84 |
| [`system-data-css-pseudo-class-keywords.md`](../system-prompts/system-data-css-pseudo-class-keywords.md) | List of CSS selector pseudo-classes and state keywords. | 186 | 0.2.9 | 0.2.9 |
| [`system-data-dom-exception-names-list.md`](../system-prompts/system-data-dom-exception-names-list.md) | List of DOM exception constants including security and network errors. | 184 | 0.2.33 | 0.2.33 |
| [`system-data-swift-keywords-list-3.md`](../system-prompts/system-data-swift-keywords-list-3.md) | List of Swift language keywords and declarations. | 171 | 0.2.9 | 1.0.87 |
| [`system-data-swift-keywords-list.md`](../system-prompts/system-data-swift-keywords-list.md) | List of Swift language keywords and declarations. | 166 | 0.2.9 | 1.0.87 |
| [`system-data-swift-keywords-list-2.md`](../system-prompts/system-data-swift-keywords-list-2.md) | List of Swift language keywords and declarations. | 162 | 0.2.9 | 1.0.87 |
| [`system-data-html-element-name-list.md`](../system-prompts/system-data-html-element-name-list.md) | List of common HTML element tag names. | 160 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-constants-and-paths.md`](../system-prompts/system-data-numeric-constants-and-paths.md) | Lists core constants and environment paths like Inf, NaN, missing, and LOAD_PATH. | 159 | 0.2.9 | 0.2.9 |
| [`system-data-plist-keybinding-xml-template.md`](../system-prompts/system-data-plist-keybinding-xml-template.md) | XML property-list snippet for a keybinding entry with numeric fields. | 158 | 0.2.46 | 0.2.46 |
| [`system-data-dom-media-input-events-list.md`](../system-prompts/system-data-dom-media-input-events-list.md) | List of common DOM, media, and form event names. | 153 | 0.2.33 | 0.2.33 |
| [`system-data-swift-standard-library-functions.md`](../system-prompts/system-data-swift-standard-library-functions.md) | List of Swift standard library functions and assertions utilities. | 151 | 0.2.9 | 0.2.9 |
| [`system-data-html-block-elements-list.md`](../system-prompts/system-data-html-block-elements-list.md) | List of uppercase HTML structural and block-level tag names. | 148 | 0.2.33 | 0.2.33 |
| [`system-data-patterned-conversation-title.md`](../system-prompts/system-data-patterned-conversation-title.md) | Generate a NUM–NUM word conversation title following pattern and recent message window. | 139 | 1.0.77 | 1.0.77 |
| [`system-data-generic-url-function-template.md`](../system-prompts/system-data-generic-url-function-template.md) | JavaScript function template named EXPR_1 with URL parameter and sixteen placeholder statements | 137 | 1.0.86 | 1.0.86 |
| [`system-data-underscore-template-runtime-2.md`](../system-prompts/system-data-underscore-template-runtime-2.md) | Scaffold compiled template function using escape, join, and print output buffering. | 133 | 0.2.54 | 1.0.87 |
| [`system-data-underscore-template-runtime.md`](../system-prompts/system-data-underscore-template-runtime.md) | Scaffold compiled template function using escape, join, and print output buffering. | 129 | 0.2.54 | 1.0.87 |
| [`system-data-mcp-server.md`](../system-prompts/system-data-mcp-server.md) | Lists per-server MCP tool and resource usage instructions collected from configured servers. | 128 | 1.0.86 | 1.0.86 |
| [`system-data-swift-attribute-annotations.md`](../system-prompts/system-data-swift-attribute-annotations.md) | List of Swift attribute keywords and Cocoa/Interface Builder annotations including autoclosure and objcMembers. | 127 | 0.2.9 | 0.2.25 |
| [`system-data-url-linked-settings-scopes.md`](../system-prompts/system-data-url-linked-settings-scopes.md) | Two URLs followed by user, project, local settings, then fifteen inserted expression blocks. | 127 | 1.0.84 | 1.0.84 |
| [`system-data-media-query-features-list.md`](../system-prompts/system-data-media-query-features-list.md) | List CSS media query features and prefers settings. | 124 | 0.2.9 | 0.2.9 |
| [`system-data-mongodb-collection-methods-list.md`](../system-prompts/system-data-mongodb-collection-methods-list.md) | Lists MongoDB collection operations and index methods. | 116 | 0.2.9 | 0.2.9 |
| [`system-data-session-start-hook-config.md`](../system-prompts/system-data-session-start-hook-config.md) | Session-start-hook wrapper concatenating 15 injected expressions and a trailing PATH tag. | 116 | 1.0.86 | 1.0.86 |
| [`system-data-csharp-keywords-list.md`](../system-prompts/system-data-csharp-keywords-list.md) | List of C# language keywords and modifiers. | 113 | 0.2.9 | 0.2.9 |
| [`system-data-javascript-builtins-and-typedarrays.md`](../system-prompts/system-data-javascript-builtins-and-typedarrays.md) | List of JavaScript built-ins and typed array constructors. | 111 | 0.2.9 | 0.2.9 |
| [`system-data-roman-numeral-sequence.md`](../system-prompts/system-data-roman-numeral-sequence.md) | Roman numerals listed sequentially from i through xl. | 108 | 0.2.9 | 0.2.9 |
| [`system-data-cli-user-preferences-flags.md`](../system-prompts/system-data-cli-user-preferences-flags.md) | Lists CLI configuration keys for behavior, notifications, and features. | 98 | 1.0.81 | 1.0.81 |
| [`system-data-linter-formatter-list.md`](../system-prompts/system-data-linter-formatter-list.md) | Lists common linters, formatters, and code quality tools. | 98 | 0.2.123 | 0.2.123 |
| [`system-data-allowed-shell-commands-list-2.md`](../system-prompts/system-data-allowed-shell-commands-list-2.md) | Whitelist-style list of common system, text, network, and docker commands. | 93 | 1.0.86 | 1.0.86 |
| [`system-data-cloud-throttling-exception-names.md`](../system-prompts/system-data-cloud-throttling-exception-names.md) | Collection of throttling and limit-exceeded exception identifiers. | 93 | 0.2.9 | 0.2.9 |
| [`system-data-javascript-builtins-list.md`](../system-prompts/system-data-javascript-builtins-list.md) | Enumeration of common JavaScript globals, typed arrays, collections, and utility functions. | 91 | 0.2.54 | 0.2.54 |
| [`system-data-runtime-environment-details-2.md`](../system-prompts/system-data-runtime-environment-details-2.md) | Reports runtime environment details including working directory, platform, OS version, date, and PATH. | 87 | 1.0.57 | 1.0.57 |
| [`system-data-ignore-build-artifacts.md`](../system-prompts/system-data-ignore-build-artifacts.md) | Lists common dependency, virtualenv, and build output directories to exclude. | 84 | 0.2.57 | 0.2.57 |
| [`system-data-swift-compiler-directives-list.md`](../system-prompts/system-data-swift-compiler-directives-list.md) | List of Swift compiler directives and magic literals. | 83 | 0.2.9 | 0.2.9 |
| [`system-data-csharp-query-keywords-list.md`](../system-prompts/system-data-csharp-query-keywords-list.md) | Lists query and async-related language keywords. | 81 | 0.2.9 | 0.2.9 |
| [`system-data-javascript-keyword-list.md`](../system-prompts/system-data-javascript-keyword-list.md) | List of JavaScript reserved words and control-flow keywords. | 76 | 0.2.9 | 0.2.9 |
| [`system-data-julia-keywords-list.md`](../system-prompts/system-data-julia-keywords-list.md) | List of Julia language keywords and core syntactic forms. | 69 | 0.2.9 | 0.2.9 |
| [`system-data-sql-current-context-functions.md`](../system-prompts/system-data-sql-current-context-functions.md) | Lists SQL current context and time functions. | 69 | 0.2.9 | 0.2.9 |
| [`system-data-sql-data-types-list.md`](../system-prompts/system-data-sql-data-types-list.md) | Lists SQL numeric, character, binary, and temporal types. | 64 | 0.2.9 | 0.2.9 |
| [`system-data-dart-core-types-list.md`](../system-prompts/system-data-dart-core-types-list.md) | List of Dart core types and common classes. | 61 | 0.2.9 | 0.2.9 |
| [`system-data-json-schema-constraints-list.md`](../system-prompts/system-data-json-schema-constraints-list.md) | List of common JSON Schema constraint and validation keywords. | 59 | 1.0.20 | 1.0.20 |
| [`system-data-sql-ddl-null-ordering.md`](../system-prompts/system-data-sql-ddl-null-ordering.md) | SQL DDL and query phrases including constraints and null ordering options. | 53 | 0.2.9 | 0.2.9 |
| [`system-data-post-hook-latex-verbs.md`](../system-prompts/system-data-post-hook-latex-verbs.md) | Post-tool-use hook formats verb, lstinline, mintinline, and hyperref fields with expressions. | 51 | 1.0.65 | 1.0.65 |

## System reminders (41)

_Sorted by tokens (desc). Showing **20** reminders with more than **30** tokens._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-reminder-cli-security-safety-guidelines.md`](../system-prompts/system-reminder-cli-security-safety-guidelines.md) | CLI assistant guidelines for safe software help, refusals, and docs lookup instructions. | 2,862 | 1.0.87 | 1.0.87 |
| [`system-reminder-architect-configs-from-needs.md`](../system-prompts/system-reminder-architect-configs-from-needs.md) | Convert user goals and project context into detailed, reliable agent specification steps. | 1,150 | 1.0.60 | 1.0.60 |
| [`system-reminder-settings-scope-2.md`](../system-prompts/system-reminder-settings-scope-2.md) | Reminder text referencing user, project, and local settings scopes. | 365 | 1.0.86 | 1.0.86 |
| [`system-reminder-settings-scope-3.md`](../system-prompts/system-reminder-settings-scope-3.md) | Reminder text referencing user, project, and local settings scopes. | 339 | 1.0.87 | 1.0.87 |
| [`system-reminder-plan-mode-no-execution.md`](../system-prompts/system-reminder-plan-mode-no-execution.md) | Answer user query, then present a confirmation plan via the EXPR_1 tool. | 155 | 1.0.69 | 1.0.69 |
| [`system-reminder-respect-intentional-file-edits.md`](../system-prompts/system-reminder-respect-intentional-file-edits.md) | Notes a file snippet was intentionally modified and should not be mentioned. | 105 | 1.0.69 | 1.0.69 |
| [`system-reminder-conversation-title-generator.md`](../system-prompts/system-reminder-conversation-title-generator.md) | Generate a NUM–NUM word conversation title from the last EXPR_6 of EXPR_7 messages. | 95 | 1.0.77 | 1.0.77 |
| [`system-reminder-session-memory-preview.md`](../system-prompts/system-reminder-session-memory-preview.md) | Previews prior session summaries and instructs reading full memory when relevant. | 74 | 1.0.87 | 1.0.87 |
| [`system-reminder-empty-todo-list.md`](../system-prompts/system-reminder-empty-todo-list.md) | Remind that the todo list is empty and must not be mentioned. | 72 | 1.0.69 | 1.0.69 |
| [`system-reminder-use-context-only-when-relevant.md`](../system-prompts/system-reminder-use-context-only-when-relevant.md) | Multiple prompts (2) | 71 | 1.0.59 | 1.0.59 |
| [`system-reminder-malicious-file-check-on-read.md`](../system-prompts/system-reminder-malicious-file-check-on-read.md) | Assess files for malicious content on read and refuse to enhance if malicious. | 67 | 1.0.31 | 1.0.31 |
| [`system-reminder-remind-to-use-todo-tracking.md`](../system-prompts/system-reminder-remind-to-use-todo-tracking.md) | Gentle reminder to use todo tracking when relevant. | 57 | 1.0.52 | 1.0.52 |
| [`system-reminder-hide-file-truncation-note.md`](../system-prompts/system-reminder-hide-file-truncation-note.md) | Warn file content is truncated and instruct using a command to read more. | 56 | 0.2.106 | 0.2.106 |
| [`system-reminder-selected-lines-context-note.md`](../system-prompts/system-reminder-selected-lines-context-note.md) | Shows user-selected line range from a file and cautions it may be unrelated. | 46 | 1.0.65 | 1.0.65 |
| [`system-reminder-todo-list-updated-silently-2.md`](../system-prompts/system-reminder-todo-list-updated-silently-2.md) | Internal notice that todo list updated; continue tasks without telling user. | 43 | 1.0.69 | 1.0.69 |
| [`system-reminder-access-prior-large-note.md`](../system-prompts/system-reminder-access-prior-large-note.md) | Reminds that … was previously read; use … tool to retrieve full contents. | 42 | 1.0.85 | 1.0.85 |
| [`system-reminder-file-offset-shorter-warning.md`](../system-prompts/system-reminder-file-offset-shorter-warning.md) | Warn that a file is shorter than the requested offset and report line count. | 42 | 1.0.53 | 1.0.53 |
| [`system-reminder-ignore-local-command-messages.md`](../system-prompts/system-reminder-ignore-local-command-messages.md) | Warns that local command output messages should be ignored unless explicitly requested. | 38 | 1.0.7 | 1.0.7 |
| [`system-reminder-invoke-requested.md`](../system-prompts/system-reminder-invoke-requested.md) | Invoke the specified agent when the user requests it, passing required context. | 32 | 1.0.62 | 1.0.62 |
| [`system-reminder-mcp-resource-no-displayable-content.md`](../system-prompts/system-reminder-mcp-resource-no-displayable-content.md) | MCP resource tag pointing to server and URI, with no displayable content. | 31 | 1.0.19 | 1.0.19 |

<details>
<summary>Show 21 low-token reminders (≤ 30 tokens)</summary>

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-reminder-mcp-resource-no-content.md`](../system-prompts/system-reminder-mcp-resource-no-content.md) | MCP resource tag referencing server and URI placeholders, indicating no content available. | 29 | 1.0.19 | 1.0.19 |
| [`system-reminder-ide-file-opened-context.md`](../system-prompts/system-reminder-ide-file-opened-context.md) | Indicates the user opened a specific IDE file that may relate to task. | 27 | 1.0.32 | 1.0.32 |
| [`system-reminder-report-new-diagnostic-issues.md`](../system-prompts/system-reminder-report-new-diagnostic-issues.md) | Announces newly detected diagnostic issues and prints the associated details block. | 27 | 1.0.18 | 1.0.74 |
| [`system-reminder-continued-session-warning.md`](../system-prompts/system-reminder-continued-session-warning.md) | Warns session resumed on another machine and reports updated working directory path. | 26 | 1.0.68 | 1.0.68 |
| [`system-reminder-address-user-message.md`](../system-prompts/system-reminder-address-user-message.md) | Address the user’s provided message and continue ongoing tasks accordingly. | 25 | 1.0.73 | 1.0.73 |
| [`system-reminder-type-alphanumeric-hyphens.md`](../system-prompts/system-reminder-type-alphanumeric-hyphens.md) | Constrain agent type strings to alphanumerics and hyphens with alphanumeric ends. | 23 | 1.0.60 | 1.0.60 |
| [`system-reminder-empty-existing-file-warning.md`](../system-prompts/system-reminder-empty-existing-file-warning.md) | Warns that a referenced file exists but has no contents. | 22 | 0.2.115 | 1.0.53 |
| [`system-reminder-active-style-guidelines.md`](../system-prompts/system-reminder-active-style-guidelines.md) | Reminder that the active output style must be followed exactly for responses. | 21 | 1.0.78 | 1.0.78 |
| [`system-reminder-call-echo-line.md`](../system-prompts/system-reminder-call-echo-line.md) | Log line noting a tool invocation and the exact input provided. | 20 | 0.2.106 | 0.2.106 |
| [`system-reminder-settings-scope.md`](../system-prompts/system-reminder-settings-scope.md) | Reminder noting userSettings, projectSettings, and localSettings locations. | 20 | 1.0.71 | 1.0.71 |
| [`system-reminder-show-existing-todo-list.md`](../system-prompts/system-reminder-show-existing-todo-list.md) | Shows the current todo list contents inside a bracketed placeholder. | 19 | 1.0.52 | 1.0.74 |
| [`system-reminder-call-result.md`](../system-prompts/system-reminder-call-result.md) | Report the result returned from invoking a specified tool. | 18 | 0.2.106 | 0.2.106 |
| [`system-reminder-check-new-bash-output.md`](../system-prompts/system-reminder-check-new-bash-output.md) | Notifies that new Bash output is available to view. | 17 | 1.0.69 | 1.0.69 |
| [`system-reminder-show-variable-contents.md`](../system-prompts/system-reminder-show-variable-contents.md) | Show contents of a referenced variable or expression with its resolved value. | 16 | 0.2.107 | 0.2.107 |
| [`system-reminder-call-error-result.md`](../system-prompts/system-reminder-call-error-result.md) | Template line reporting an error result from a specified tool call. | 13 | 0.2.119 | 0.2.119 |
| [`system-reminder-summarize-conversation.md`](../system-prompts/system-reminder-summarize-conversation.md) | Directs the assistant to summarize conversations. | 13 | 0.2.108 | 0.2.108 |
| [`system-reminder-web-search.md`](../system-prompts/system-reminder-web-search.md) | Sets the assistant to perform web search tool use. | 11 | 0.2.108 | 0.2.108 |
| [`system-reminder-exit-status.md`](../system-prompts/system-reminder-exit-status.md) | Reports the process exit code value for a completed command. | 10 | 1.0.69 | 1.0.69 |
| [`system-reminder-background-bash-run.md`](../system-prompts/system-reminder-background-bash-run.md) | Marks an identifier for a background Bash execution instance. | 9 | 1.0.69 | 1.0.69 |
| [`system-reminder-local-binary-content.md`](../system-prompts/system-reminder-local-binary-content.md) | Indicates the resource contains local binary data. | 6 | 1.0.19 | 1.0.19 |
| [`system-reminder-full-resource-contents-header.md`](../system-prompts/system-reminder-full-resource-contents-header.md) | Introduces the full contents of a referenced resource. | 5 | 1.0.19 | 1.0.19 |

</details>
