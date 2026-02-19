# System Prompts Index – by init

- Total prompt files: **207**

## Categories

- System prompts (71)
- Tool prompts (38)
- System data (61)
- System reminders (37)

## System prompts (71)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-prompt-exit-transcript-rules.md`](../system-prompts/system-prompt-exit-transcript-rules.md) | Specifies how stdout and stderr are displayed for tool call inputs and responses by exit code. | 71 | 1.0.24 | 1.0.24 |
| [`system-prompt-exit-handling.md`](../system-prompts/system-prompt-exit-handling.md) | Defines stdout and stderr visibility rules based on command exit code for tool calls. | 63 | 1.0.24 | 1.0.24 |
| [`system-prompt-run-bash-commands-safely.md`](../system-prompts/system-prompt-run-bash-commands-safely.md) | Run a bash command with directory checks, quoting rules, and configurable timeout. | 3,007 | 1.0.23 | 1.0.23 |
| [`system-prompt-bash-command-prefix-detection.md`](../system-prompts/system-prompt-bash-command-prefix-detection.md) | Define command prefix extraction and injection detection with illustrative shell command examples. | 693 | 1.0.23 | 1.0.23 |
| [`system-prompt-write-conversation-title-7.md`](../system-prompts/system-prompt-write-conversation-title-7.md) | Generate a concise NUM-NUM word title summarizing the provided conversation text. | 61 | 1.0.23 | 1.0.23 |
| [`system-prompt-list-mcp-server-resources.md`](../system-prompts/system-prompt-list-mcp-server-resources.md) | Lists available resources across MCP servers with optional server filtering. | 73 | 1.0.22 | 1.0.22 |
| [`system-prompt-read-mcp-server-resource.md`](../system-prompts/system-prompt-read-mcp-server-resource.md) | Reads a resource from an MCP server by server name and URI. | 73 | 1.0.22 | 1.0.22 |
| [`system-prompt-official-cli-cell.md`](../system-prompts/system-prompt-official-cli-cell.md) | Define a cell wrapper declaring Claude as Anthropic’s official CLI with identifiers. | 59 | 1.0.22 | 1.0.22 |
| [`system-prompt-verify-repo-access-scope.md`](../system-prompts/system-prompt-verify-repo-access-scope.md) | Verify repository name, access, and required GitHub token scopes. | 56 | 1.0.22 | 1.0.22 |
| [`system-prompt-pull-request-review.md`](../system-prompts/system-prompt-pull-request-review.md) | Pull request-triggered GitHub Actions job checks out code and runs Claude review action. | 687 | 1.0.20 | 1.0.20 |
| [`system-prompt-structured-coding-task-list.md`](../system-prompts/system-prompt-structured-coding-task-list.md) | Guide creating and updating a structured todo list for complex coding sessions. | 2,321 | 1.0.19 | 1.0.19 |
| [`system-prompt-avoid-rereading-unchanged-resource.md`](../system-prompts/system-prompt-avoid-rereading-unchanged-resource.md) | Instructs to not reread a resource unless it may have changed. | 22 | 1.0.19 | 1.0.19 |
| [`system-prompt-create-shell-snapshot-file-aliases.md`](../system-prompts/system-prompt-create-shell-snapshot-file-aliases.md) | Generates a snapshot script that unaliases, records aliases, ensures rg, and exports PATH. | 375 | 1.0.18 | 1.0.18 |
| [`system-prompt-replace-all-occurrences-warning.md`](../system-prompts/system-prompt-replace-all-occurrences-warning.md) | Warns about multiple replacement matches when replace_all is false, requesting unique context. | 61 | 1.0.18 | 1.0.18 |
| [`system-prompt-write-conversation-title-15.md`](../system-prompts/system-prompt-write-conversation-title-15.md) | Generate a …-… word title summarizing the provided conversation text. | 47 | 1.0.18 | 1.0.24 |
| [`system-prompt-delegate-uncertain-search.md`](../system-prompts/system-prompt-delegate-uncertain-search.md) | Guidelines for using an agent to search broadly, versus specific file tools. | 500 | 1.0.16 | 1.0.16 |
| [`system-prompt-dev-conversation-summary-2.md`](../system-prompts/system-prompt-dev-conversation-summary-2.md) | Produce a chronological, technically detailed conversation summary with structured analysis notes. | 1,263 | 1.0.14 | 1.0.23 |
| [`system-prompt-dev-conversation-summary.md`](../system-prompts/system-prompt-dev-conversation-summary.md) | Multiple prompts (2) | 1,252 | 1.0.14 | 1.0.23 |
| [`system-prompt-batch-edits-single-file.md`](../system-prompts/system-prompt-batch-edits-single-file.md) | Instructions for making multiple exact replacements in one file after reading context. | 628 | 1.0.8 | 1.0.8 |
| [`system-prompt-extract-displayed-file-paths.md`](../system-prompts/system-prompt-extract-displayed-file-paths.md) | Identify and return only explicitly shown file paths when file contents are displayed. | 289 | 1.0.8 | 1.0.8 |
| [`system-prompt-exact-string-edits-in-files.md`](../system-prompts/system-prompt-exact-string-edits-in-files.md) | Define rules for exact in-file string replacements after reading and with unique matches. | 258 | 1.0.8 | 1.0.8 |
| [`system-prompt-edit-files-minimal-changes.md`](../system-prompts/system-prompt-edit-files-minimal-changes.md) | Use Claude Code tools to fulfill user tasks, avoid new files, share absolute paths. | 180 | 1.0.7 | 1.0.7 |
| [`system-prompt-write-file-with-constraints.md`](../system-prompts/system-prompt-write-file-with-constraints.md) | Defines rules for writing files, including reading before overwriting and avoiding new docs. | 145 | 1.0.7 | 1.0.7 |
| [`system-prompt-applied-edits-cli-banner.md`](../system-prompts/system-prompt-applied-edits-cli-banner.md) | Announce applied local edits and state identity as Anthropic's official Claude CLI. | 64 | 1.0.7 | 1.0.7 |
| [`system-prompt-read-file-absolute-path.md`](../system-prompts/system-prompt-read-file-absolute-path.md) | Read files by absolute path with line limits, numbering, and image support. | 367 | 1.0.4 | 1.0.4 |
| [`system-prompt-install-github-cli.md`](../system-prompts/system-prompt-install-github-cli.md) | Install GitHub CLI across macOS, Windows, and Linux. | 41 | 1.0.0 | 1.0.0 |
| [`system-prompt-admin-setup-secrets-apps.md`](../system-prompts/system-prompt-admin-setup-secrets-apps.md) | Have a repository admin install apps and configure secrets when setup fails. | 33 | 1.0.0 | 1.0.0 |
| [`system-prompt-refresh-workflow-scope.md`](../system-prompts/system-prompt-refresh-workflow-scope.md) | Refresh authentication to include workflow scope for creating Actions workflows. | 31 | 1.0.0 | 1.0.0 |
| [`system-prompt-use-owner-path-format.md`](../system-prompts/system-prompt-use-owner-path-format.md) | Use the owner and path or URL format for repository references. | 28 | 1.0.0 | 1.0.0 |
| [`system-prompt-authenticate-with-gh-cli.md`](../system-prompts/system-prompt-authenticate-with-gh-cli.md) | Authenticate to GitHub using gh auth login or environment-based methods. | 25 | 1.0.0 | 1.0.0 |
| [`system-prompt-anthropic-cli-identity.md`](../system-prompts/system-prompt-anthropic-cli-identity.md) | System banner declaring the CLI identity as Anthropic’s official Claude tool. | 59 | 0.2.119 | 0.2.119 |
| [`system-prompt-install-app.md`](../system-prompts/system-prompt-install-app.md) | Explains adding a workflow to enable Claude Code via @claude mentions after merge. | 392 | 0.2.116 | 0.2.116 |
| [`system-prompt-write-conversation-title-4.md`](../system-prompts/system-prompt-write-conversation-title-4.md) | Generate a …-… word title summarizing the provided conversation text. | 42 | 0.2.113 | 1.0.24 |
| [`system-prompt-regex-content-search.md`](../system-prompts/system-prompt-regex-content-search.md) | Describes a fast regex-based file content search with guidance on match counting. | 170 | 0.2.108 | 0.2.116 |
| [`system-prompt-follow-codebase-user-2.md`](../system-prompts/system-prompt-follow-codebase-user-2.md) | Follow the provided codebase and user instructions, acting as the specified CLI persona. | 86 | 0.2.105 | 0.2.105 |
| [`system-prompt-write-conversation-title-6.md`](../system-prompts/system-prompt-write-conversation-title-6.md) | Produce a fixed-length title summarizing the provided conversation, outputting only the title. | 46 | 0.2.104 | 1.0.24 |
| [`system-prompt-cheerful-gerund-status-word-2.md`](../system-prompts/system-prompt-cheerful-gerund-status-word-2.md) | Generate one whimsical, positive gerund related to the user message with strict safety exclusions. | 198 | 0.2.103 | 0.2.103 |
| [`system-prompt-command-message-name-args.md`](../system-prompts/system-prompt-command-message-name-args.md) | XML-like command message template specifying subject, status, command name, and arguments. | 63 | 0.2.102 | 1.0.18 |
| [`system-prompt-create-md-guide-2.md`](../system-prompts/system-prompt-create-md-guide-2.md) | Analyze the repo and draft or improve a CLAUDE.md with commands and architecture. | 382 | 0.2.101 | 0.2.101 |
| [`system-prompt-write-conversation-title-10.md`](../system-prompts/system-prompt-write-conversation-title-10.md) | Generate a NUM-to-NUM word conversation title, output title only. | 87 | 0.2.101 | 1.0.24 |
| [`system-prompt-command-metadata-tags.md`](../system-prompts/system-prompt-command-metadata-tags.md) | Multiple prompts (2) | 52 | 0.2.101 | 1.0.18 |
| [`system-prompt-write-conversation-title-11.md`](../system-prompts/system-prompt-write-conversation-title-11.md) | Generate a …-… word title summarizing the provided conversation text. | 41 | 0.2.93 | 1.0.24 |
| [`system-prompt-write-conversation-title-8.md`](../system-prompts/system-prompt-write-conversation-title-8.md) | Generate a …-… word title summarizing the provided conversation text. | 41 | 0.2.93 | 1.0.24 |
| [`system-prompt-write-conversation-title-12.md`](../system-prompts/system-prompt-write-conversation-title-12.md) | Multiple prompts (4) | 42 | 0.2.92 | 1.0.24 |
| [`system-prompt-write-conversation-title-14.md`](../system-prompts/system-prompt-write-conversation-title-14.md) | Generate a …-… word title summarizing the provided conversation text. | 62 | 0.2.91 | 1.0.23 |
| [`system-prompt-generate-word-count-title.md`](../system-prompts/system-prompt-generate-word-count-title.md) | Output only a …-… word title for the given conversation. | 50 | 0.2.91 | 0.2.91 |
| [`system-prompt-write-conversation-title.md`](../system-prompts/system-prompt-write-conversation-title.md) | Generate a …-… word title summarizing the provided conversation text. | 49 | 0.2.91 | 1.0.20 |
| [`system-prompt-write-conversation-title-13.md`](../system-prompts/system-prompt-write-conversation-title-13.md) | Generate a …-… word title summarizing the provided conversation text. | 48 | 0.2.91 | 1.0.24 |
| [`system-prompt-write-conversation-title-2.md`](../system-prompts/system-prompt-write-conversation-title-2.md) | Generate a …-… word title summarizing the provided conversation text. | 48 | 0.2.91 | 1.0.24 |
| [`system-prompt-write-conversation-title-3.md`](../system-prompts/system-prompt-write-conversation-title-3.md) | Generate a …-… word title summarizing the provided conversation text. | 48 | 0.2.91 | 1.0.24 |
| [`system-prompt-write-conversation-title-9.md`](../system-prompts/system-prompt-write-conversation-title-9.md) | Generate a …-… word title summarizing the provided conversation text. | 48 | 0.2.91 | 1.0.24 |
| [`system-prompt-conversation-title-only-output.md`](../system-prompts/system-prompt-conversation-title-only-output.md) | Write a NUM-NUM word conversation title using the provided transcript only. | 47 | 0.2.91 | 0.2.91 |
| [`system-prompt-title-with-files-context.md`](../system-prompts/system-prompt-title-with-files-context.md) | Generate a …-… word title using conversation text and file context. | 46 | 0.2.91 | 0.2.91 |
| [`system-prompt-write-conversation-title-5.md`](../system-prompts/system-prompt-write-conversation-title-5.md) | Generate a …-… word title summarizing the provided conversation text. | 42 | 0.2.91 | 1.0.24 |
| [`system-prompt-summarize-coding-chat-status.md`](../system-prompts/system-prompt-summarize-coding-chat-status.md) | Condense a coding conversation into a character-limited status recap. | 33 | 0.2.91 | 0.2.91 |
| [`system-prompt-malicious-files-refusal-check.md`](../system-prompts/system-prompt-malicious-files-refusal-check.md) | Checks whether listed files seem malicious and mandates refusal if suspicious. | 30 | 0.2.89 | 0.2.89 |
| [`system-prompt-create-view-instrument-selector.md`](../system-prompts/system-prompt-create-view-instrument-selector.md) | Create a new view with specified name, optional description, and InstrumentSelector variants. | 110 | 0.2.76 | 0.2.76 |
| [`system-prompt-snapshot-zsh-functions-options.md`](../system-prompts/system-prompt-snapshot-zsh-functions-options.md) | Capture zsh functions and active options into a snapshot file. | 158 | 0.2.73 | 0.2.73 |
| [`system-prompt-summarize-shell-command.md`](../system-prompts/system-prompt-summarize-shell-command.md) | Write a brief input-output description of a shell command in a few words. | 78 | 0.2.59 | 0.2.59 |
| [`system-prompt-update-memory-file.md`](../system-prompts/system-prompt-update-memory-file.md) | Update or append memories in a file at a given path using one tool call. | 118 | 0.2.54 | 1.0.24 |
| [`system-prompt-continue-last-task.md`](../system-prompts/system-prompt-continue-last-task.md) | Continue from prior conversation state and resume the last task without questions. | 38 | 0.2.54 | 0.2.54 |
| [`system-prompt-concise-github-issue-titles.md`](../system-prompts/system-prompt-concise-github-issue-titles.md) | Create a specific technical GitHub issue title from a bug report within a character limit. | 129 | 0.2.47 | 0.2.47 |
| [`system-prompt-cite-with-limited-quotes.md`](../system-prompts/system-prompt-cite-with-limited-quotes.md) | Multiple prompts (2) | 140 | 0.2.40 | 1.0.18 |
| [`system-prompt-git-status-session-start.md`](../system-prompts/system-prompt-git-status-session-start.md) | Record initial git status snapshot, including current branch and main branch names. | 77 | 0.2.32 | 1.0.18 |
| [`system-prompt-fetch-pr-comments.md`](../system-prompts/system-prompt-fetch-pr-comments.md) | Fetch PR-level and review comments via gh API, then format threads with diffs. | 444 | 0.2.9 | 0.2.9 |
| [`system-prompt-review-github-pull-request.md`](../system-prompts/system-prompt-review-github-pull-request.md) | Use GitHub CLI to list/view PRs, fetch diff, and deliver structured code review. | 233 | 0.2.9 | 0.2.9 |
| [`system-prompt-select-core-frequently-modified-files.md`](../system-prompts/system-prompt-select-core-frequently-modified-files.md) | Choose five diverse frequently modified core-logic filenames from git history stats. | 90 | 0.2.9 | 0.2.9 |
| [`system-prompt-detect-new-topic-title.md`](../system-prompts/system-prompt-detect-new-topic-title.md) | Detect whether a message starts a new topic and extract a short title. | 85 | 0.2.9 | 0.2.9 |
| [`system-prompt-fix-missing-executable-name.md`](../system-prompts/system-prompt-fix-missing-executable-name.md) | Advise fixes when a specified CLI subcommand executable path is missing. | 81 | 0.2.9 | 1.0.23 |
| [`system-prompt-file-updated-snippet-output.md`](../system-prompts/system-prompt-file-updated-snippet-output.md) | Notify that a file was updated and show numbered snippet output from cat -n. | 38 | 0.2.9 | 0.2.9 |
| [`system-prompt-classify-bash-command-prefix.md`](../system-prompts/system-prompt-classify-bash-command-prefix.md) | Determine the appropriate prefix for bash commands requested by a coding agent. | 33 | 0.2.9 | 0.2.9 |

## Tool prompts (38)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`tool-description-add-working-directory.md`](../system-prompts/tool-description-add-working-directory.md) | Add a new working directory. | 5 | 1.0.23 | 1.0.23 |
| [`tool-description-run-bash-with-timeout.md`](../system-prompts/tool-description-run-bash-with-timeout.md) | Bash execution tool spec with directory verification guidance and configurable timeouts. | 641 | 1.0.22 | 1.0.22 |
| [`tool-description-list-configured-mcp-resources.md`](../system-prompts/tool-description-list-configured-mcp-resources.md) | Tool to list MCP resources from all or a specified server including server field. | 74 | 1.0.22 | 1.0.22 |
| [`tool-description-read-resource-by-uri.md`](../system-prompts/tool-description-read-resource-by-uri.md) | Tool to read an MCP resource by server name and resource URI. | 54 | 1.0.22 | 1.0.22 |
| [`tool-description-structured-todo-list-guidelines.md`](../system-prompts/tool-description-structured-todo-list-guidelines.md) | Criteria for starting, updating, and avoiding a structured todo tool during coding sessions | 2,326 | 1.0.19 | 1.0.19 |
| [`tool-description-manage-background-bash-shells.md`](../system-prompts/tool-description-manage-background-bash-shells.md) | Lists and controls background bash shell sessions. | 6 | 1.0.18 | 1.0.18 |
| [`tool-description-exit-plan-mode-confirmation.md`](../system-prompts/tool-description-exit-plan-mode-confirmation.md) | Prompts the user to exit plan mode after the plan has been presented. | 31 | 1.0.11 | 1.0.11 |
| [`tool-description-upgrade-to-max-rate-limits.md`](../system-prompts/tool-description-upgrade-to-max-rate-limits.md) | Promotes upgrading to Max to get higher rate limits and more Opus access. | 12 | 1.0.11 | 1.0.11 |
| [`tool-description-multi-edit-file-operations.md`](../system-prompts/tool-description-multi-edit-file-operations.md) | Explains multi-edit single-file replacement tool built on another tool, with sequencing rules. | 645 | 1.0.8 | 1.0.8 |
| [`tool-description-exact-file-string-replacement.md`](../system-prompts/tool-description-exact-file-string-replacement.md) | Describes exact in-file replacement tool rules, requiring prior read and unique old_string. | 263 | 1.0.8 | 1.0.8 |
| [`tool-description-write-file-after-reading-existing.md`](../system-prompts/tool-description-write-file-after-reading-existing.md) | Write files, reading existing contents first, and avoid unrequested new or documentation files. | 150 | 1.0.7 | 1.0.9 |
| [`tool-description-manage-permissions.md`](../system-prompts/tool-description-manage-permissions.md) | Controls allow and deny rules for tool permissions. | 8 | 1.0.7 | 1.0.7 |
| [`tool-description-read-local-file-paths.md`](../system-prompts/tool-description-read-local-file-paths.md) | File-reading tool spec with absolute-path requirement, line limits, and image support. | 375 | 1.0.4 | 1.0.4 |
| [`tool-description-show-status-details.md`](../system-prompts/tool-description-show-status-details.md) | Command to display Claude Code status, version, model, connectivity, and tools. | 18 | 1.0.4 | 1.0.4 |
| [`tool-description-set.md`](../system-prompts/tool-description-set.md) | Set the Claude Code model selection. | 7 | 1.0.0 | 1.0.0 |
| [`tool-description-manage-ide-integrations-status.md`](../system-prompts/tool-description-manage-ide-integrations-status.md) | Manage IDE MCP integrations and display their status. | 8 | 0.2.126 | 1.0.0 |
| [`tool-description-fast-regex-file-search.md`](../system-prompts/tool-description-fast-regex-file-search.md) | Fast regex content search across files with optional include globs for filtering. | 133 | 0.2.116 | 0.2.116 |
| [`tool-description-fast-glob-file-matching-2.md`](../system-prompts/tool-description-fast-glob-file-matching-2.md) | Glob-based file matcher returning paths sorted by modification time and supports batching searches. | 118 | 0.2.116 | 0.2.116 |
| [`tool-description-web-search-for-updates.md`](../system-prompts/tool-description-web-search-for-updates.md) | Search the web for up-to-date information and return formatted results. | 96 | 0.2.104 | 0.2.104 |
| [`tool-description-setup-github-actions.md`](../system-prompts/tool-description-setup-github-actions.md) | Sets up Claude GitHub Actions integration for a repository. | 8 | 0.2.101 | 0.2.101 |
| [`tool-description-fetch-and-analyze-url.md`](../system-prompts/tool-description-fetch-and-analyze-url.md) | Tool spec for fetching a web page converting to markdown and analyzing with a model. | 225 | 0.2.96 | 0.2.96 |
| [`tool-description-read-session-todo-list-2.md`](../system-prompts/tool-description-read-session-todo-list-2.md) | Read the current session to-do list frequently to stay aligned on pending work. | 216 | 0.2.93 | 0.2.93 |
| [`tool-description-option-enter-newline-binding.md`](../system-prompts/tool-description-option-enter-newline-binding.md) | Enable Option+Enter to insert newlines. | 12 | 0.2.80 | 0.2.83 |
| [`tool-description-list-files-in-context.md`](../system-prompts/tool-description-list-files-in-context.md) | List all files currently available in context. | 6 | 0.2.79 | 0.2.79 |
| [`tool-description-clear-chat-keep-summary.md`](../system-prompts/tool-description-clear-chat-keep-summary.md) | Clears conversation history while retaining a summary in context. | 24 | 0.2.54 | 0.2.57 |
| [`tool-description-toggle-vim-editing-mode.md`](../system-prompts/tool-description-toggle-vim-editing-mode.md) | Switch between Vim and normal editing modes. | 8 | 0.2.54 | 0.2.54 |
| [`tool-description-edit-memory-files.md`](../system-prompts/tool-description-edit-memory-files.md) | Edit Claude memory files. | 4 | 0.2.54 | 0.2.54 |
| [`tool-description-migrate-npm-global-to-local.md`](../system-prompts/tool-description-migrate-npm-global-to-local.md) | Move from a global npm install to a project-local installation. | 9 | 0.2.51 | 0.2.51 |
| [`tool-description-list-path-with-ignore-globs.md`](../system-prompts/tool-description-list-path-with-ignore-globs.md) | Lists files and directories at an absolute path with optional ignore glob patterns. | 60 | 0.2.29 | 0.2.83 |
| [`tool-description-replace-jupyter-notebook-cell.md`](../system-prompts/tool-description-replace-jupyter-notebook-cell.md) | Replaces, inserts, or deletes a specific Jupyter notebook cell by index. | 117 | 0.2.9 | 0.2.83 |
| [`tool-description-read-jupyter-notebook-cells.md`](../system-prompts/tool-description-read-jupyter-notebook-cells.md) | Loads an ipynb from an absolute path and returns cells with outputs. | 62 | 0.2.9 | 0.2.83 |
| [`tool-description-show-session-cost-and-duration.md`](../system-prompts/tool-description-show-session-cost-and-duration.md) | Displays the current session total cost and duration. | 10 | 0.2.9 | 0.2.9 |
| [`tool-description-check-health.md`](../system-prompts/tool-description-check-health.md) | Checks the health of a Claude Code installation. | 9 | 0.2.9 | 0.2.9 |
| [`tool-description-sign-in-anthropic-account.md`](../system-prompts/tool-description-sign-in-anthropic-account.md) | Signs in using an Anthropic account. | 8 | 0.2.9 | 0.2.9 |
| [`tool-description-sign-out-anthropic-account.md`](../system-prompts/tool-description-sign-out-anthropic-account.md) | Signs out from an Anthropic account. | 8 | 0.2.9 | 0.2.9 |
| [`tool-description-clear-conversation-history.md`](../system-prompts/tool-description-clear-conversation-history.md) | Clears conversation history to free up context. | 7 | 0.2.9 | 0.2.9 |
| [`tool-description-show-help-and-commands.md`](../system-prompts/tool-description-show-help-and-commands.md) | Displays help text and available commands. | 5 | 0.2.9 | 0.2.9 |
| [`tool-description-submit-feedback.md`](../system-prompts/tool-description-submit-feedback.md) | Submits user feedback about Claude Code. | 5 | 0.2.9 | 0.2.9 |

## System data (61)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-data-multiline-put-repo-update.md`](../system-prompts/system-data-multiline-put-repo-update.md) | Constructs a multiline dotall uli command to PUT updated repository file content via API. | 296 | 1.0.24 | 1.0.24 |
| [`system-data-launch-latest-cli-version.md`](../system-prompts/system-data-launch-latest-cli-version.md) | Launcher script selects latest executable CLI via symlink or newest version directory. | 383 | 1.0.22 | 1.0.22 |
| [`system-data-mention-github-action.md`](../system-prompts/system-data-mention-github-action.md) | GitHub Actions runs Claude Code when @claude appears in issues, comments, or reviews. | 596 | 1.0.20 | 1.0.20 |
| [`system-data-app-settings-keys.md`](../system-prompts/system-data-app-settings-keys.md) | Lists configuration keys for updater, theme, notifications, and editor behavior. | 80 | 1.0.4 | 1.0.4 |
| [`system-data-runtime-environment-details.md`](../system-prompts/system-data-runtime-environment-details.md) | Environment metadata: working directory, platform, OS version, date, model, and git repo status. | 74 | 1.0.4 | 1.0.4 |
| [`system-data-numeric-placeholder-list.md`](../system-prompts/system-data-numeric-placeholder-list.md) | Repeated numeric placeholders in a long list. | 573 | 0.2.125 | 0.2.125 |
| [`system-data-http-header-field-list.md`](../system-prompts/system-data-http-header-field-list.md) | List of HTTP request and response header fields including CORS and CSP. | 501 | 0.2.125 | 0.2.125 |
| [`system-data-linter-formatter-list.md`](../system-prompts/system-data-linter-formatter-list.md) | Lists common linters, formatters, and code quality tools. | 98 | 0.2.123 | 0.2.123 |
| [`system-data-shell-function-snapshot-script.md`](../system-prompts/system-data-shell-function-snapshot-script.md) | Bash snippet that snapshots functions and shell options into a file using base64-encoded eval. | 296 | 0.2.76 | 0.2.76 |
| [`system-data-ignore-build-artifacts.md`](../system-prompts/system-data-ignore-build-artifacts.md) | Lists common dependency, virtualenv, and build output directories to exclude. | 84 | 0.2.57 | 0.2.57 |
| [`system-data-underscore-template-runtime-2.md`](../system-prompts/system-data-underscore-template-runtime-2.md) | Scaffold compiled template function using escape, join, and print output buffering. | 133 | 0.2.54 | 1.0.11 |
| [`system-data-underscore-template-runtime.md`](../system-prompts/system-data-underscore-template-runtime.md) | Scaffold compiled template function using escape, join, and print output buffering. | 129 | 0.2.54 | 1.0.11 |
| [`system-data-javascript-builtins-list.md`](../system-prompts/system-data-javascript-builtins-list.md) | Enumeration of common JavaScript globals, typed arrays, collections, and utility functions. | 91 | 0.2.54 | 0.2.54 |
| [`system-data-append-memory-entry.md`](../system-prompts/system-data-append-memory-entry.md) | Insert provided memory block into an empty memory file at given path. | 37 | 0.2.54 | 0.2.54 |
| [`system-data-plist-keybinding-xml-template.md`](../system-prompts/system-data-plist-keybinding-xml-template.md) | XML property-list snippet for a keybinding entry with numeric fields. | 158 | 0.2.46 | 0.2.46 |
| [`system-data-whimsical-verb-synonyms-list.md`](../system-prompts/system-data-whimsical-verb-synonyms-list.md) | Playful list of gerund verbs describing thinking or doing. | 221 | 0.2.42 | 0.2.42 |
| [`system-data-dom-exception-messages-codes.md`](../system-prompts/system-data-dom-exception-messages-codes.md) | DOM exception names with placeholder numeric codes and messages. | 532 | 0.2.33 | 0.2.33 |
| [`system-data-dom-exception-names-list.md`](../system-prompts/system-data-dom-exception-names-list.md) | List of DOM exception constants including security and network errors. | 184 | 0.2.33 | 0.2.33 |
| [`system-data-dom-media-input-events-list.md`](../system-prompts/system-data-dom-media-input-events-list.md) | List of common DOM, media, and form event names. | 153 | 0.2.33 | 0.2.33 |
| [`system-data-html-block-elements-list.md`](../system-prompts/system-data-html-block-elements-list.md) | List of uppercase HTML structural and block-level tag names. | 148 | 0.2.33 | 0.2.33 |
| [`system-data-mapped-valid-disallowed-std.md`](../system-prompts/system-data-mapped-valid-disallowed-std.md) | Repeated tokens for mapped and valid with disallowed std markers and ignored numbers. | 211,885 | 0.2.9 | 0.2.9 |
| [`system-data-wolfram-language-symbols-list.md`](../system-prompts/system-data-wolfram-language-symbols-list.md) | Alphabetical list of Wolfram Language built-in symbol names. | 35,789 | 0.2.9 | 0.2.9 |
| [`system-data-stan-functions-reference-list.md`](../system-prompts/system-data-stan-functions-reference-list.md) | Partial catalog of Stan math, RNG, and distribution functions. | 2,155 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-placeholder-sequence.md`](../system-prompts/system-data-numeric-placeholder-sequence.md) | Repeated numeric placeholder tokens in a long sequence. | 1,791 | 0.2.9 | 0.2.9 |
| [`system-data-html-doctype-variants-list.md`](../system-prompts/system-data-html-doctype-variants-list.md) | Strings enumerating HTML doctype variants including strict, levels, and internet explorer. | 1,099 | 0.2.9 | 1.0.22 |
| [`system-data-html-doctype-variants-list-2.md`](../system-prompts/system-data-html-doctype-variants-list-2.md) | Strings enumerating HTML doctype variants including strict, levels, and internet explorer. | 1,063 | 0.2.9 | 1.0.22 |
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
| [`system-data-swift-keywords-list.md`](../system-prompts/system-data-swift-keywords-list.md) | List of Swift language keywords and declarations. | 171 | 0.2.9 | 1.0.22 |
| [`system-data-swift-keywords-list-2.md`](../system-prompts/system-data-swift-keywords-list-2.md) | List of Swift language keywords and declarations. | 166 | 0.2.9 | 1.0.23 |
| [`system-data-swift-keywords-list-3.md`](../system-prompts/system-data-swift-keywords-list-3.md) | List of Swift language keywords and declarations. | 162 | 0.2.9 | 1.0.23 |
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
| [`system-data-http-request-timing-events.md`](../system-prompts/system-data-http-request-timing-events.md) | Provide HTTP request timing event markers from redirect start through response end. | 92 | 0.2.9 | 1.0.1 |
| [`system-data-swift-compiler-directives-list.md`](../system-prompts/system-data-swift-compiler-directives-list.md) | List of Swift compiler directives and magic literals. | 83 | 0.2.9 | 0.2.9 |
| [`system-data-csharp-query-keywords-list.md`](../system-prompts/system-data-csharp-query-keywords-list.md) | Lists query and async-related language keywords. | 81 | 0.2.9 | 0.2.9 |
| [`system-data-javascript-keyword-list.md`](../system-prompts/system-data-javascript-keyword-list.md) | List of JavaScript reserved words and control-flow keywords. | 76 | 0.2.9 | 0.2.9 |
| [`system-data-julia-keywords-list.md`](../system-prompts/system-data-julia-keywords-list.md) | List of Julia language keywords and core syntactic forms. | 69 | 0.2.9 | 0.2.9 |
| [`system-data-sql-current-context-functions.md`](../system-prompts/system-data-sql-current-context-functions.md) | Lists SQL current context and time functions. | 69 | 0.2.9 | 0.2.9 |
| [`system-data-sql-data-types-list.md`](../system-prompts/system-data-sql-data-types-list.md) | Lists SQL numeric, character, binary, and temporal types. | 64 | 0.2.9 | 0.2.9 |
| [`system-data-dart-core-types-list.md`](../system-prompts/system-data-dart-core-types-list.md) | List of Dart core types and common classes. | 61 | 0.2.9 | 0.2.9 |
| [`system-data-sql-ddl-null-ordering.md`](../system-prompts/system-data-sql-ddl-null-ordering.md) | SQL DDL and query phrases including constraints and null ordering options. | 53 | 0.2.9 | 0.2.9 |

## System reminders (37)

_Sorted by init (newest first). Showing **16** reminders with more than **30** tokens._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-reminder-cli-safety-guidelines.md`](../system-prompts/system-reminder-cli-safety-guidelines.md) | Interactive CLI system rules for safe assistance, refusing malicious requests, and help/feedback guidance. | 3,047 | 1.0.20 | 1.0.20 |
| [`system-reminder-multi-expression-placeholder-block.md`](../system-prompts/system-reminder-multi-expression-placeholder-block.md) | System reminder template concatenating seven ordered expression blocks separated by blank lines | 48 | 1.0.19 | 1.0.19 |
| [`system-reminder-mcp-resource-no-displayable-content.md`](../system-prompts/system-reminder-mcp-resource-no-displayable-content.md) | MCP resource tag pointing to server and URI, with no displayable content. | 31 | 1.0.19 | 1.0.19 |
| [`system-reminder-plan-mode-no-changes-2.md`](../system-prompts/system-reminder-plan-mode-no-changes-2.md) | Multiple prompts (2) | 163 | 1.0.16 | 1.0.16 |
| [`system-reminder-relative-date-shortcuts-list.md`](../system-prompts/system-reminder-relative-date-shortcuts-list.md) | List of relative date shortcut commands. | 38 | 1.0.8 | 1.0.8 |
| [`system-reminder-ignore-local-command-messages.md`](../system-prompts/system-reminder-ignore-local-command-messages.md) | Warns that local command output messages should be ignored unless explicitly requested. | 38 | 1.0.7 | 1.0.7 |
| [`system-reminder-respect-intentional-file-edits.md`](../system-prompts/system-reminder-respect-intentional-file-edits.md) | Multiple prompts (2) | 104 | 0.2.118 | 0.2.118 |
| [`system-reminder-todo-list-updated-2.md`](../system-prompts/system-reminder-todo-list-updated-2.md) | Multiple prompts (2) | 85 | 0.2.118 | 0.2.118 |
| [`system-reminder-optional-context.md`](../system-prompts/system-reminder-optional-context.md) | Multiple prompts (2) | 88 | 0.2.106 | 0.2.106 |
| [`system-reminder-empty-todo-list.md`](../system-prompts/system-reminder-empty-todo-list.md) | Multiple prompts (2) | 83 | 0.2.106 | 0.2.106 |
| [`system-reminder-template-function-wrapper.md`](../system-prompts/system-reminder-template-function-wrapper.md) | Underscore-style template wrapper using object scope, escaping, print join, and output buffer. | 78 | 0.2.106 | 0.2.106 |
| [`system-reminder-underscore-template-function-wrapper.md`](../system-prompts/system-reminder-underscore-template-function-wrapper.md) | Compiled Underscore template function skeleton that escapes values and accumulates output. | 70 | 0.2.106 | 0.2.106 |
| [`system-reminder-hide-file-truncation-note.md`](../system-prompts/system-reminder-hide-file-truncation-note.md) | Warn file content is truncated and instruct using a command to read more. | 56 | 0.2.106 | 0.2.106 |
| [`system-reminder-synthesize-multi-findings.md`](../system-prompts/system-reminder-synthesize-multi-findings.md) | Synthesize multiple agents’ analyses into one unified, contradiction-resolved response for the original task | 159 | 0.2.72 | 1.0.14 |
| [`system-reminder-nested-underscore-template-functions.md`](../system-prompts/system-reminder-nested-underscore-template-functions.md) | Nested compiled template functions that concatenate output into a string buffer. | 134 | 0.2.54 | 1.0.4 |
| [`system-reminder-update-memory-file.md`](../system-prompts/system-reminder-update-memory-file.md) | Update or append memories in a file at a given path using one tool call. | 118 | 0.2.54 | 1.0.24 |

<details>
<summary>Show 21 low-token reminders (≤ 30 tokens)</summary>

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-reminder-mcp-resource-no-content.md`](../system-prompts/system-reminder-mcp-resource-no-content.md) | MCP resource tag referencing server and URI placeholders, indicating no content available. | 29 | 1.0.19 | 1.0.19 |
| [`system-reminder-local-binary-content.md`](../system-prompts/system-reminder-local-binary-content.md) | Indicates the resource contains local binary data. | 6 | 1.0.19 | 1.0.19 |
| [`system-reminder-full-resource-contents-header.md`](../system-prompts/system-reminder-full-resource-contents-header.md) | Introduces the full contents of a referenced resource. | 5 | 1.0.19 | 1.0.19 |
| [`system-reminder-report-new-diagnostic-issues.md`](../system-prompts/system-reminder-report-new-diagnostic-issues.md) | Announces newly detected diagnostic issues and prints the associated details block. | 27 | 1.0.18 | 1.0.18 |
| [`system-reminder-call-error-result.md`](../system-prompts/system-reminder-call-error-result.md) | Template line reporting an error result from a specified tool call. | 13 | 0.2.119 | 0.2.119 |
| [`system-reminder-empty-existing-file-warning.md`](../system-prompts/system-reminder-empty-existing-file-warning.md) | Warns that a referenced file exists but has no contents. | 22 | 0.2.115 | 1.0.20 |
| [`system-reminder-relay-user-message-content.md`](../system-prompts/system-reminder-relay-user-message-content.md) | Introduces and includes the user’s message content verbatim. | 13 | 0.2.108 | 0.2.108 |
| [`system-reminder-summarize-conversation.md`](../system-prompts/system-reminder-summarize-conversation.md) | Directs the assistant to summarize conversations. | 13 | 0.2.108 | 0.2.108 |
| [`system-reminder-web-search.md`](../system-prompts/system-reminder-web-search.md) | Sets the assistant to perform web search tool use. | 11 | 0.2.108 | 0.2.108 |
| [`system-reminder-smselect-smlike-smcard-tokens.md`](../system-prompts/system-reminder-smselect-smlike-smcard-tokens.md) | Lists component token names for reference. | 7 | 0.2.108 | 0.2.108 |
| [`system-reminder-show-variable-contents.md`](../system-prompts/system-reminder-show-variable-contents.md) | Show contents of a referenced variable or expression with its resolved value. | 16 | 0.2.107 | 0.2.107 |
| [`system-reminder-null-safe-interpolation.md`](../system-prompts/system-reminder-null-safe-interpolation.md) | Render an expression with null treated as an empty string. | 26 | 0.2.106 | 0.2.106 |
| [`system-reminder-user-selected-lines.md`](../system-prompts/system-reminder-user-selected-lines.md) | Present the specific lines the user selected from a given file. | 21 | 0.2.106 | 0.2.106 |
| [`system-reminder-call-echo-line.md`](../system-prompts/system-reminder-call-echo-line.md) | Log line noting a tool invocation and the exact input provided. | 20 | 0.2.106 | 0.2.106 |
| [`system-reminder-call-result.md`](../system-prompts/system-reminder-call-result.md) | Report the result returned from invoking a specified tool. | 18 | 0.2.106 | 0.2.106 |
| [`system-reminder-console-log-level-words.md`](../system-prompts/system-reminder-console-log-level-words.md) | Lists console logging level labels such as error, info, and warn. | 15 | 0.2.106 | 0.2.106 |
| [`system-reminder-escape-interpolated-expression.md`](../system-prompts/system-reminder-escape-interpolated-expression.md) | Escape and output an interpolated template expression safely. | 15 | 0.2.106 | 0.2.106 |
| [`system-reminder-user-opened-file-ide.md`](../system-prompts/system-reminder-user-opened-file-ide.md) | Notify that the user opened a specified file in the IDE. | 15 | 0.2.106 | 0.2.106 |
| [`system-reminder-new-uid-generated.md`](../system-prompts/system-reminder-new-uid-generated.md) | Indicates that a new unique identifier was generated. | 5 | 0.2.106 | 0.2.106 |
| [`system-reminder-simulated-unmount-behavior.md`](../system-prompts/system-reminder-simulated-unmount-behavior.md) | Notes that unmount behavior is simulated. | 5 | 0.2.106 | 0.2.106 |
| [`system-reminder-schedule-after-delay.md`](../system-prompts/system-reminder-schedule-after-delay.md) | Indicates scheduling an action after a delay. | 3 | 0.2.106 | 0.2.106 |

</details>
