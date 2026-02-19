# Claude Code CLI Surface x.y.z

## Summary

- Commands: 10
- Options: 15
- Env vars: 89
- Config keys: 51
- Tools: 0
- Skills: 0
- Models: 15
- Providers: 7

## Commands

### Names

- `add`
- `approved-tools`
- `config`
- `doctor`
- `get`
- `list`
- `mcp`
- `remove`
- `serve`
- `set`

### Specs

- `add <name> <command> [args...]`
- `approved-tools`
- `config`
- `doctor`
- `get <key>`
- `get <name>`
- `list`
- `mcp`
- `remove <key>`
- `remove <name>`
- `remove <tool>`
- `serve`
- `set <key> <value>`

## Options

### Flags

- `--cwd`
- `--dangerously-skip-permissions`
- `--debug`
- `--enable-architect`
- `--env`
- `--global`
- `--print`
- `--scope`
- `--verbose`
- `-c`
- `-d`
- `-e`
- `-g`
- `-p`
- `-s`

### Specs

- `--dangerously-skip-permissions`
- `--verbose`
- `-c, --cwd <cwd>`
- `-d, --debug`
- `-e, --env <env...>`
- `-ea, --enable-architect`
- `-g, --global`
- `-p, --print`
- `-s, --scope <scope>`

## Env Vars

- `__MINIMATCH_TESTING_PLATFORM__`
- `ALIYUN_REGION_ID`
- `ANTHROPIC_AUTH_TOKEN`
- `ANTHROPIC_MODEL`
- `API_TIMEOUT_MS`
- `APPDATA`
- `AWS_ACCESS_KEY_ID`
- `AWS_DEFAULT_REGION`
- `AWS_EXECUTION_ENV`
- `AWS_REGION`
- `AWS_SECRET_ACCESS_KEY`
- `AWS_SESSION_TOKEN`
- `CF_PAGES_COMMIT_SHA`
- `CI`
- `CLAUDE_CODE_USE_BEDROCK`
- `CLAUDE_CODE_USE_VERTEX`
- `CLAUDE_CONFIG_DIR`
- `CLOUD_ML_REGION`
- `CLOUD_RUN_JOB`
- `COMMIT_REF`
- `DEBUG`
- `DEBUG_AUTH`
- `DETECT_GCP_RETRIES`
- `DISABLE_PROMPT_CACHING`
- `DOTENV_CONFIG_DEBUG`
- `DOTENV_CONFIG_DOTENV_KEY`
- `DOTENV_CONFIG_ENCODING`
- `DOTENV_CONFIG_OVERRIDE`
- `DOTENV_CONFIG_PATH`
- `DOTENV_KEY`
- `DYNO`
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
- `GOOGLE_APPLICATION_CREDENTIALS`
- `GOOGLE_CLOUD_PROJECT`
- `GOOGLE_CLOUD_QUOTA_PROJECT`
- `HOME`
- `IBM_CLOUD_REGION`
- `K_CONFIGURATION`
- `K_SERVICE`
- `METADATA_SERVER_DETECTION`
- `NETLIFY`
- `NO_PROXY`
- `NODE_DEBUG`
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
- `SHARP_FORCE_GLOBAL_LIBVIPS`
- `SHARP_IGNORE_GLOBAL_LIBVIPS`
- `SHELL`
- `SWE_BENCH`
- `SYSTEMROOT`
- `TENCENTCLOUD_APPID`
- `TENCENTCLOUD_REGION`
- `TENCENTCLOUD_ZONE`
- `TERM_PROGRAM`
- `THINK_TOOL`
- `USE_BUILTIN_RIPGREP`
- `VERCEL`
- `VERCEL_BITBUCKET_COMMIT_SHA`
- `VERCEL_GIT_COMMIT_SHA`
- `VERCEL_GITHUB_COMMIT_SHA`
- `VERCEL_GITLAB_COMMIT_SHA`
- `VERCEL_REGION`
- `VERTEX_REGION_CLAUDE_3_5_HAIKU`
- `VERTEX_REGION_CLAUDE_3_5_SONNET`
- `VERTEX_REGION_CLAUDE_3_7_SONNET`
- `WEBSITE_SITE_NAME`
- `WS_NO_BUFFER_UTIL`
- `WS_NO_UTF_8_VALIDATE`
- `ZEIT_BITBUCKET_COMMIT_SHA`
- `ZEIT_GITHUB_COMMIT_SHA`
- `ZEIT_GITLAB_COMMIT_SHA`

## Config Keys

- `_meta`
- `api`
- `arguments`
- `code`
- `content`
- `costPriority`
- `data`
- `description`
- `error`
- `experimental`
- `hasMore`
- `hints`
- `httpMethodsToRetry`
- `id`
- `inputSchema`
- `intelligencePriority`
- `jsonrpc`
- `libvips`
- `listChanged`
- `logging`
- `message`
- `method`
- `mimeType`
- `name`
- `noResponseRetries`
- `params`
- `progress`
- `progressToken`
- `prompt`
- `prompts`
- `properties`
- `required`
- `resource`
- `resources`
- `result`
- `role`
- `roots`
- `sampling`
- `speedPriority`
- `subscribe`
- `text`
- `thought`
- `tools`
- `total`
- `trigger`
- `type`
- `uri`
- `uriTemplate`
- `value`
- `values`
- `version`

## Tools

_None detected_

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

## Providers

- `anthropic`
- `aws`
- `azure`
- `bedrock`
- `google`
- `openai`
- `vertex`
