# System Prompts Index – by init

- Total prompt files: **96**

## Categories

- System prompts (25)
- Tool prompts (22)
- System data (49)

## System prompts (25)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-prompt-secure-persistent-bash-execution.md`](../system-prompts/system-prompt-secure-persistent-bash-execution.md) | Execute bash commands in persistent shell with directory checks, quoting, timeouts, and banned-command restrictions. | 2,202 | 0.2.40 | 0.2.40 |
| [`system-prompt-read-local-file-lines.md`](../system-prompts/system-prompt-read-local-file-lines.md) | Reads absolute-path files with optional offset/limit, truncation, numbered lines; use EXPR_1 for notebooks. | 158 | 0.2.40 | 0.2.40 |
| [`system-prompt-cite-with-limited-quotes.md`](../system-prompts/system-prompt-cite-with-limited-quotes.md) | Multiple prompts (2) | 140 | 0.2.40 | 0.2.40 |
| [`system-prompt-secure-cli-coding.md`](../system-prompts/system-prompt-secure-cli-coding.md) | Interactive CLI coding assistant with strict malware refusal and slash-command help workflow | 2,329 | 0.2.38 | 0.2.38 |
| [`system-prompt-continue-from-prior-session.md`](../system-prompts/system-prompt-continue-from-prior-session.md) | Continue a context-limited session using the provided prior conversation summary. | 40 | 0.2.38 | 0.2.38 |
| [`system-prompt-technical-conversation-summary-format.md`](../system-prompts/system-prompt-technical-conversation-summary-format.md) | Produces a detailed development-focused conversation summary with required sections. | 663 | 0.2.36 | 0.2.36 |
| [`system-prompt-organize-project-memories-file-2.md`](../system-prompts/system-prompt-organize-project-memories-file-2.md) | Update or add memories in CLAUDE.md, grouped by global preferences and project sections. | 340 | 0.2.36 | 0.2.36 |
| [`system-prompt-initial-git-status-snapshot-2.md`](../system-prompts/system-prompt-initial-git-status-snapshot-2.md) | Record initial git status snapshot, including current branch and main branch names. | 89 | 0.2.36 | 0.2.36 |
| [`system-prompt-bash-command-prefix-detection.md`](../system-prompts/system-prompt-bash-command-prefix-detection.md) | Define command prefix extraction and injection detection with illustrative shell command examples. | 658 | 0.2.30 | 0.2.30 |
| [`system-prompt-command-metadata-tags.md`](../system-prompts/system-prompt-command-metadata-tags.md) | Multiple prompts (2) | 52 | 0.2.30 | 0.2.30 |
| [`system-prompt-delegated-search-guidance.md`](../system-prompts/system-prompt-delegated-search-guidance.md) | Instruct when to launch a search agent versus using direct file or grep tools. | 432 | 0.2.18 | 0.2.18 |
| [`system-prompt-fetch-pr-comments.md`](../system-prompts/system-prompt-fetch-pr-comments.md) | Fetch PR-level and review comments via gh API, then format threads with diffs. | 444 | 0.2.9 | 0.2.9 |
| [`system-prompt-review-github-pull-request.md`](../system-prompts/system-prompt-review-github-pull-request.md) | Use GitHub CLI to list/view PRs, fetch diff, and deliver structured code review. | 233 | 0.2.9 | 0.2.9 |
| [`system-prompt-cli-guidelines.md`](../system-prompts/system-prompt-cli-guidelines.md) | Instruct Claude Code to reply briefly with absolute paths and relevant snippets. | 224 | 0.2.9 | 0.2.9 |
| [`system-prompt-create-md-guide.md`](../system-prompts/system-prompt-create-md-guide.md) | Generate or improve a CLAUDE.md with build commands and code style rules. | 162 | 0.2.9 | 0.2.9 |
| [`system-prompt-delphi-ui-components-list.md`](../system-prompts/system-prompt-delphi-ui-components-list.md) | Lists UI component class names and checklist states. | 148 | 0.2.9 | 0.2.9 |
| [`system-prompt-extract-command-file-paths.md`](../system-prompts/system-prompt-extract-command-file-paths.md) | Extract verbatim file paths read or modified by a command. | 143 | 0.2.9 | 0.2.9 |
| [`system-prompt-command-writer.md`](../system-prompts/system-prompt-command-writer.md) | Write a brief plain-language description of a shell command. | 95 | 0.2.9 | 0.2.9 |
| [`system-prompt-select-core-frequently-modified-files.md`](../system-prompts/system-prompt-select-core-frequently-modified-files.md) | Choose five diverse frequently modified core-logic filenames from git history stats. | 90 | 0.2.9 | 0.2.9 |
| [`system-prompt-detect-new-topic-title.md`](../system-prompts/system-prompt-detect-new-topic-title.md) | Detect whether a message starts a new topic and extract a short title. | 85 | 0.2.9 | 0.2.9 |
| [`system-prompt-command-message-xml-template.md`](../system-prompts/system-prompt-command-message-xml-template.md) | Format a command message with name, args, and contents XML-like fields. | 82 | 0.2.9 | 0.2.9 |
| [`system-prompt-fix-missing-executable-name.md`](../system-prompts/system-prompt-fix-missing-executable-name.md) | Advise fixes when a specified CLI subcommand executable path is missing. | 81 | 0.2.9 | 0.2.9 |
| [`system-prompt-feedback-issue-title.md`](../system-prompts/system-prompt-feedback-issue-title.md) | Create a concise issue title summarizing user feedback. | 56 | 0.2.9 | 0.2.9 |
| [`system-prompt-file-updated-snippet-output.md`](../system-prompts/system-prompt-file-updated-snippet-output.md) | Notify that a file was updated and show numbered snippet output from cat -n. | 38 | 0.2.9 | 0.2.9 |
| [`system-prompt-classify-bash-command-prefix.md`](../system-prompts/system-prompt-classify-bash-command-prefix.md) | Determine the appropriate prefix for bash commands requested by a coding agent. | 33 | 0.2.9 | 0.2.9 |

## Tool prompts (22)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`tool-description-secure-bash-command-runner.md`](../system-prompts/tool-description-secure-bash-command-runner.md) | Run a bash command with directory verification, banned-command checks, and output truncation. | 2,179 | 0.2.40 | 0.2.40 |
| [`tool-description-fetch-url-and-summarize.md`](../system-prompts/tool-description-fetch-url-and-summarize.md) | Fetches an HTTPS URL, converts to markdown, and analyzes it with a small model using a provided prompt. | 163 | 0.2.40 | 0.2.40 |
| [`tool-description-read-local-file-lines-2.md`](../system-prompts/tool-description-read-local-file-lines-2.md) | Reads absolute-path files with optional offset/limit, truncation, numbered lines; use EXPR_1 for notebooks. | 158 | 0.2.40 | 0.2.40 |
| [`tool-description-list-allowed-capabilities.md`](../system-prompts/tool-description-list-allowed-capabilities.md) | Lists all currently allowed tools. | 5 | 0.2.40 | 0.2.40 |
| [`tool-description-change-light-theme.md`](../system-prompts/tool-description-change-light-theme.md) | Change the interface theme to light mode. | 11 | 0.2.38 | 0.2.38 |
| [`tool-description-list-path-with-ignore-globs.md`](../system-prompts/tool-description-list-path-with-ignore-globs.md) | Lists files and directories at an absolute path with optional ignore glob patterns. | 60 | 0.2.29 | 0.2.29 |
| [`tool-description-toggle-vim-emacs-modes.md`](../system-prompts/tool-description-toggle-vim-emacs-modes.md) | Switch between vim and emacs editing modes. | 8 | 0.2.19 | 0.2.19 |
| [`tool-description-edit-file-by-replacing-string.md`](../system-prompts/tool-description-edit-file-by-replacing-string.md) | Edit a file by replacing one unique old string with new text. | 687 | 0.2.9 | 0.2.9 |
| [`tool-description-fast-regex-content-search.md`](../system-prompts/tool-description-fast-regex-content-search.md) | Searches file contents with regular expressions and optional include globs. | 123 | 0.2.9 | 0.2.9 |
| [`tool-description-replace-jupyter-notebook-cell.md`](../system-prompts/tool-description-replace-jupyter-notebook-cell.md) | Replaces, inserts, or deletes a specific Jupyter notebook cell by index. | 117 | 0.2.9 | 0.2.9 |
| [`tool-description-fast-glob-file-matching.md`](../system-prompts/tool-description-fast-glob-file-matching.md) | Finds files by glob patterns and returns paths sorted by modification time. | 84 | 0.2.9 | 0.2.9 |
| [`tool-description-write-file-to-disk.md`](../system-prompts/tool-description-write-file-to-disk.md) | Writes a file to the local filesystem, overwriting if it exists. | 84 | 0.2.9 | 0.2.9 |
| [`tool-description-read-jupyter-notebook-cells.md`](../system-prompts/tool-description-read-jupyter-notebook-cells.md) | Loads an ipynb from an absolute path and returns cells with outputs. | 62 | 0.2.9 | 0.2.9 |
| [`tool-description-install-shift-enter-binding.md`](../system-prompts/tool-description-install-shift-enter-binding.md) | Installs a Shift+Enter key binding for newlines in supported terminals and editors. | 20 | 0.2.9 | 0.2.9 |
| [`tool-description-show-session-cost-and-duration.md`](../system-prompts/tool-description-show-session-cost-and-duration.md) | Displays the current session total cost and duration. | 10 | 0.2.9 | 0.2.9 |
| [`tool-description-check-health.md`](../system-prompts/tool-description-check-health.md) | Checks the health of a Claude Code installation. | 9 | 0.2.9 | 0.2.9 |
| [`tool-description-clear-history-keep-summary.md`](../system-prompts/tool-description-clear-history-keep-summary.md) | Clears conversation history while retaining a summary in context. | 9 | 0.2.9 | 0.2.9 |
| [`tool-description-sign-in-anthropic-account.md`](../system-prompts/tool-description-sign-in-anthropic-account.md) | Signs in using an Anthropic account. | 8 | 0.2.9 | 0.2.9 |
| [`tool-description-sign-out-anthropic-account.md`](../system-prompts/tool-description-sign-out-anthropic-account.md) | Signs out from an Anthropic account. | 8 | 0.2.9 | 0.2.9 |
| [`tool-description-clear-conversation-history.md`](../system-prompts/tool-description-clear-conversation-history.md) | Clears conversation history to free up context. | 7 | 0.2.9 | 0.2.9 |
| [`tool-description-show-help-and-commands.md`](../system-prompts/tool-description-show-help-and-commands.md) | Displays help text and available commands. | 5 | 0.2.9 | 0.2.9 |
| [`tool-description-submit-feedback.md`](../system-prompts/tool-description-submit-feedback.md) | Submits user feedback about Claude Code. | 5 | 0.2.9 | 0.2.9 |

## System data (49)

_Sorted by init (newest first)._

| File | Summary | Tokens | Init | Last edit |
| --- | --- | ---: | --- | --- |
| [`system-data-path-list-template.md`](../system-prompts/system-data-path-list-template.md) | Multiple prompts (2) | 111 | 0.2.40 | 0.2.40 |
| [`system-data-dom-exception-messages-codes.md`](../system-prompts/system-data-dom-exception-messages-codes.md) | DOM exception names with placeholder numeric codes and messages. | 532 | 0.2.33 | 0.2.33 |
| [`system-data-dom-exception-names-list.md`](../system-prompts/system-data-dom-exception-names-list.md) | List of DOM exception constants including security and network errors. | 184 | 0.2.33 | 0.2.33 |
| [`system-data-dom-media-input-events-list.md`](../system-prompts/system-data-dom-media-input-events-list.md) | List of common DOM, media, and form event names. | 153 | 0.2.33 | 0.2.33 |
| [`system-data-html-block-elements-list.md`](../system-prompts/system-data-html-block-elements-list.md) | List of uppercase HTML structural and block-level tag names. | 148 | 0.2.33 | 0.2.33 |
| [`system-data-swift-attribute-annotations.md`](../system-prompts/system-data-swift-attribute-annotations.md) | List of Swift attribute keywords and Cocoa/Interface Builder annotations including autoclosure and objcMembers. | 235 | 0.2.30 | 0.2.30 |
| [`system-data-mapped-valid-disallowed-std.md`](../system-prompts/system-data-mapped-valid-disallowed-std.md) | Repeated tokens for mapped and valid with disallowed std markers and ignored numbers. | 211,885 | 0.2.9 | 0.2.9 |
| [`system-data-wolfram-language-symbols-list.md`](../system-prompts/system-data-wolfram-language-symbols-list.md) | Alphabetical list of Wolfram Language built-in symbol names. | 35,789 | 0.2.9 | 0.2.9 |
| [`system-data-stan-functions-reference-list.md`](../system-prompts/system-data-stan-functions-reference-list.md) | Partial catalog of Stan math, RNG, and distribution functions. | 2,155 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-placeholder-sequence.md`](../system-prompts/system-data-numeric-placeholder-sequence.md) | Repeated numeric placeholder tokens in a long sequence. | 1,791 | 0.2.9 | 0.2.9 |
| [`system-data-html-doctype-variants-list.md`](../system-prompts/system-data-html-doctype-variants-list.md) | Strings enumerating HTML doctype variants including strict, levels, and internet explorer. | 1,099 | 0.2.9 | 0.2.40 |
| [`system-data-html-doctype-variants-list-2.md`](../system-prompts/system-data-html-doctype-variants-list-2.md) | Strings enumerating HTML doctype variants including strict, levels, and internet explorer. | 1,063 | 0.2.9 | 0.2.40 |
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
| [`system-data-whimsical-verb-synonyms-list.md`](../system-prompts/system-data-whimsical-verb-synonyms-list.md) | Playful list of gerund verbs describing thinking or doing. | 217 | 0.2.9 | 0.2.9 |
| [`system-data-javascript-builtins-and-typed-arrays.md`](../system-prompts/system-data-javascript-builtins-and-typed-arrays.md) | Enumerates JavaScript globals, built-in objects, errors, and typed arrays. | 216 | 0.2.9 | 0.2.9 |
| [`system-data-css-pseudo-class-keywords.md`](../system-prompts/system-data-css-pseudo-class-keywords.md) | List of CSS selector pseudo-classes and state keywords. | 186 | 0.2.9 | 0.2.9 |
| [`system-data-swift-keywords-list.md`](../system-prompts/system-data-swift-keywords-list.md) | List of Swift language keywords and declarations. | 171 | 0.2.9 | 0.2.40 |
| [`system-data-swift-keywords-list-3.md`](../system-prompts/system-data-swift-keywords-list-3.md) | List of Swift language keywords and declarations. | 166 | 0.2.9 | 0.2.38 |
| [`system-data-swift-keywords-list-2.md`](../system-prompts/system-data-swift-keywords-list-2.md) | List of Swift language keywords and declarations. | 162 | 0.2.9 | 0.2.40 |
| [`system-data-html-element-name-list.md`](../system-prompts/system-data-html-element-name-list.md) | List of common HTML element tag names. | 160 | 0.2.9 | 0.2.9 |
| [`system-data-numeric-constants-and-paths.md`](../system-prompts/system-data-numeric-constants-and-paths.md) | Lists core constants and environment paths like Inf, NaN, missing, and LOAD_PATH. | 159 | 0.2.9 | 0.2.9 |
| [`system-data-plist-keybinding-xml-template.md`](../system-prompts/system-data-plist-keybinding-xml-template.md) | XML property-list snippet for a keybinding entry with numeric fields. | 158 | 0.2.9 | 0.2.9 |
| [`system-data-swift-standard-library-functions.md`](../system-prompts/system-data-swift-standard-library-functions.md) | List of Swift standard library functions and assertions utilities. | 151 | 0.2.9 | 0.2.9 |
| [`system-data-media-query-features-list.md`](../system-prompts/system-data-media-query-features-list.md) | List CSS media query features and prefers settings. | 124 | 0.2.9 | 0.2.9 |
| [`system-data-mongodb-collection-methods-list.md`](../system-prompts/system-data-mongodb-collection-methods-list.md) | Lists MongoDB collection operations and index methods. | 116 | 0.2.9 | 0.2.9 |
| [`system-data-csharp-keywords-list.md`](../system-prompts/system-data-csharp-keywords-list.md) | List of C# language keywords and modifiers. | 113 | 0.2.9 | 0.2.9 |
| [`system-data-javascript-builtins-and-typedarrays.md`](../system-prompts/system-data-javascript-builtins-and-typedarrays.md) | List of JavaScript built-ins and typed array constructors. | 111 | 0.2.9 | 0.2.9 |
| [`system-data-roman-numeral-sequence.md`](../system-prompts/system-data-roman-numeral-sequence.md) | Roman numerals listed sequentially from i through xl. | 108 | 0.2.9 | 0.2.9 |
| [`system-data-cloud-throttling-exception-names.md`](../system-prompts/system-data-cloud-throttling-exception-names.md) | Collection of throttling and limit-exceeded exception identifiers. | 93 | 0.2.9 | 0.2.9 |
| [`system-data-http-request-timing-events.md`](../system-prompts/system-data-http-request-timing-events.md) | Provide HTTP request timing event markers from redirect start through response end. | 92 | 0.2.9 | 0.2.9 |
| [`system-data-swift-compiler-directives-list.md`](../system-prompts/system-data-swift-compiler-directives-list.md) | List of Swift compiler directives and magic literals. | 83 | 0.2.9 | 0.2.9 |
| [`system-data-csharp-query-keywords-list.md`](../system-prompts/system-data-csharp-query-keywords-list.md) | Lists query and async-related language keywords. | 81 | 0.2.9 | 0.2.9 |
| [`system-data-javascript-keyword-list.md`](../system-prompts/system-data-javascript-keyword-list.md) | List of JavaScript reserved words and control-flow keywords. | 76 | 0.2.9 | 0.2.9 |
| [`system-data-runtime-environment-metadata.md`](../system-prompts/system-data-runtime-environment-metadata.md) | Display environment details like working directory, platform, date, model, and PATH. | 71 | 0.2.9 | 0.2.9 |
| [`system-data-julia-keywords-list.md`](../system-prompts/system-data-julia-keywords-list.md) | List of Julia language keywords and core syntactic forms. | 69 | 0.2.9 | 0.2.9 |
| [`system-data-sql-current-context-functions.md`](../system-prompts/system-data-sql-current-context-functions.md) | Lists SQL current context and time functions. | 69 | 0.2.9 | 0.2.9 |
| [`system-data-sql-data-types-list.md`](../system-prompts/system-data-sql-data-types-list.md) | Lists SQL numeric, character, binary, and temporal types. | 64 | 0.2.9 | 0.2.9 |
| [`system-data-dart-core-types-list.md`](../system-prompts/system-data-dart-core-types-list.md) | List of Dart core types and common classes. | 61 | 0.2.9 | 0.2.9 |
| [`system-data-sql-ddl-null-ordering.md`](../system-prompts/system-data-sql-ddl-null-ordering.md) | SQL DDL and query phrases including constraints and null ordering options. | 53 | 0.2.9 | 0.2.9 |
