# Claude Code CLI Surface x.y.z

## Summary

- Commands: 14
- Options: 17
- Env vars: 124
- Config keys: 70
- Tools: 5
- Skills: 0
- Models: 16
- Providers: 7

## Commands

### Names

- `add`
- `add-from-claude-desktop`
- `add-json`
- `config`
- `doctor`
- `get`
- `list`
- `mcp`
- `migrate-installer`
- `remove`
- `reset-project-choices`
- `serve`
- `set`
- `update`

### Specs

- `add [name] [commandOrUrl] [args...]`
- `add <key> <values...>`
- `add-from-claude-desktop`
- `add-json <name> <json>`
- `config`
- `doctor`
- `get <key>`
- `get <name>`
- `list`
- `mcp`
- `migrate-installer`
- `remove <key> [values...]`
- `remove <name>`
- `reset-project-choices`
- `serve`
- `set <key> <value>`
- `update`

## Options

### Flags

- `--allowedTools`
- `--dangerously-skip-permissions`
- `--debug`
- `--env`
- `--global`
- `--json`
- `--mcp-debug`
- `--print`
- `--scope`
- `--transport`
- `--verbose`
- `-d`
- `-e`
- `-g`
- `-p`
- `-s`
- `-t`

### Specs

- `--allowedTools <tools...>`
- `--dangerously-skip-permissions`
- `--json`
- `--mcp-debug`
- `--verbose`
- `-d, --debug`
- `-e, --env <env...>`
- `-g, --global`
- `-p, --print`
- `-s, --scope <scope>`
- `-t, --transport <transport>`

## Env Vars

- `__CFB`
- `__MINIMATCH_TESTING_PLATFORM__`
- `ALACRITTY_LOG`
- `ALIYUN_REGION_ID`
- `ANTHROPIC_API_KEY`
- `ANTHROPIC_AUTH_TOKEN`
- `ANTHROPIC_BASE_URL`
- `ANTHROPIC_CUSTOM_HEADERS`
- `ANTHROPIC_MODEL`
- `ANTHROPIC_SMALL_FAST_MODEL`
- `API_TIMEOUT_MS`
- `APPDATA`
- `AWS_ACCESS_KEY_ID`
- `AWS_DEFAULT_REGION`
- `AWS_EXECUTION_ENV`
- `AWS_REGION`
- `AWS_SECRET_ACCESS_KEY`
- `AWS_SESSION_TOKEN`
- `BUN_INSTALL`
- `C`
- `CF_PAGES_COMMIT_SHA`
- `CLAUDE_CODE_EXTRA_BODY`
- `CLAUDE_CODE_USE_BEDROCK`
- `CLAUDE_CODE_USE_VERTEX`
- `CLAUDE_CONFIG_DIR`
- `CLOUD_ML_REGION`
- `CLOUD_RUN_JOB`
- `COMMIT_REF`
- `CURSOR_TRACE_ID`
- `DEBUG`
- `DEBUG_AUTH`
- `DETECT_GCP_RETRIES`
- `DISABLE_AUTOUPDATER`
- `DISABLE_BUG_COMMAND`
- `DISABLE_COST_WARNINGS`
- `DISABLE_ERROR_REPORTING`
- `DISABLE_PROMPT_CACHING`
- `DISABLE_TELEMETRY`
- `DYNO`
- `EDITOR`
- `FLY_REGION`
- `FUNCTION_NAME`
- `FUNCTION_TARGET`
- `GAE_MODULE_NAME`
- `GAE_SERVICE`
- `GCE_METADATA_HOST`
- `GCE_METADATA_IP`
- `GCLOUD_PROJECT`
- `GCP_PROJECT`
- `GITHUB_SHA`
- `GNOME_TERMINAL_SERVICE`
- `GOOGLE_APPLICATION_CREDENTIALS`
- `GOOGLE_CLOUD_PROJECT`
- `GOOGLE_CLOUD_QUOTA_PROJECT`
- `HOME`
- `HTTP_PROXY`
- `HTTPS_PROXY`
- `IBM_CLOUD_REGION`
- `IGNORE_TEST_WIN32`
- `IS_DEMO`
- `K_CONFIGURATION`
- `K_SERVICE`
- `KITTY_WINDOW_ID`
- `KONSOLE_VERSION`
- `MAX_THINKING_TOKENS`
- `MCP_TIMEOUT`
- `MCP_TOOL_TIMEOUT`
- `METADATA_SERVER_DETECTION`
- `MSYSTEM`
- `NETLIFY`
- `NO_PROXY`
- `NODE_DEBUG`
- `NODE_OPTIONS`
- `PATH`
- `PKG_CONFIG_PATH`
- `REGION_NAME`
- `SENTRY_BAGGAGE`
- `SENTRY_DSN`
- `SENTRY_ENVIRONMENT`
- `SENTRY_NAME`
- `SENTRY_RELEASE`
- `SENTRY_TRACE`
- `SENTRY_TRACES_SAMPLE_RATE`
- `SENTRY_USE_ENVIRONMENT`
- `SESSIONNAME`
- `SHARP_FORCE_GLOBAL_LIBVIPS`
- `SHARP_IGNORE_GLOBAL_LIBVIPS`
- `SHELL`
- `SSH_CLIENT`
- `SSH_CONNECTION`
- `SSH_TTY`
- `STY`
- `SWE_BENCH`
- `SYSTEMROOT`
- `TENCENTCLOUD_APPID`
- `TENCENTCLOUD_REGION`
- `TENCENTCLOUD_ZONE`
- `TERM`
- `TERM_PROGRAM`
- `TERMINATOR_UUID`
- `TILIX_ID`
- `TMUX`
- `USE_BUILTIN_RIPGREP`
- `USERPROFILE`
- `VERCEL`
- `VERCEL_BITBUCKET_COMMIT_SHA`
- `VERCEL_GIT_COMMIT_SHA`
- `VERCEL_GITHUB_COMMIT_SHA`
- `VERCEL_GITLAB_COMMIT_SHA`
- `VERCEL_REGION`
- `VERTEX_REGION_CLAUDE_3_5_HAIKU`
- `VERTEX_REGION_CLAUDE_3_5_SONNET`
- `VERTEX_REGION_CLAUDE_3_7_SONNET`
- `VISUAL`
- `VTE_VERSION`
- `WEBSITE_SITE_NAME`
- `WS_NO_BUFFER_UTIL`
- `WS_NO_UTF_8_VALIDATE`
- `WSL_DISTRO_NAME`
- `WT_SESSION`
- `XTERM_VERSION`
- `ZEIT_BITBUCKET_COMMIT_SHA`
- `ZEIT_GITHUB_COMMIT_SHA`
- `ZEIT_GITLAB_COMMIT_SHA`

## Config Keys

- `_meta`
- `allow`
- `api`
- `args`
- `arguments`
- `character`
- `charset`
- `code`
- `command`
- `compressible`
- `content`
- `costPriority`
- `data`
- `description`
- `end`
- `env`
- `error`
- `experimental`
- `extensions`
- `filePath`
- `hasMore`
- `hints`
- `httpMethodsToRetry`
- `id`
- `input`
- `inputSchema`
- `intelligencePriority`
- `jsonrpc`
- `libvips`
- `line`
- `listChanged`
- `logging`
- `mcpServers`
- `message`
- `method`
- `mimeType`
- `name`
- `noResponseRetries`
- `params`
- `permissions`
- `progress`
- `progressToken`
- `prompt`
- `prompts`
- `properties`
- `reason`
- `required`
- `resource`
- `resources`
- `result`
- `role`
- `roots`
- `sampling`
- `selection`
- `server`
- `source`
- `speedPriority`
- `start`
- `subscribe`
- `text`
- `tool_name`
- `tools`
- `total`
- `type`
- `uri`
- `uriTemplate`
- `url`
- `value`
- `values`
- `version`

## Tools

- `⚒`
- `⚔`
- `⚗`
- `⚙`
- `⛏`

## Skills

_None detected_

## Models

- `claude-1.3`
- `claude-1.3-100k`
- `claude-2.0`
- `claude-2.1`
- `claude-3-5-haiku`
- `claude-3-5-haiku-20241022`
- `claude-3-5-sonnet`
- `claude-3-7-sonnet`
- `claude-3-7-sonnet-20250219`
- `claude-3-sonnet-20240229`
- `claude-cli`
- `claude-code-20250219`
- `claude-instant-1.1`
- `claude-instant-1.1-100k`
- `claude-instant-1.2`
- `claude-local`

## Providers

- `anthropic`
- `aws`
- `azure`
- `bedrock`
- `google`
- `openai`
- `vertex`
