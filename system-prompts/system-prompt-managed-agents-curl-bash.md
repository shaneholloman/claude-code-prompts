# System Prompt: managed-agents-curl-bash

- Source: inline

## Summary

Examples for raw HTTP requests using cURL.

# Raw Prompt Text
# Managed Agents — cURL / Raw HTTP

Use these examples when the user needs raw HTTP requests or is working without an SDK.

## Setup

```bash
export ANTHROPIC_API_KEY="your-api-key"

# Common headers
HEADERS=(
  -H "Content-Type: application${PATH}"
  -H "x-api-key: $ANTHROPIC_API_KEY"
  -H "anthropic-version: ${DATE}"
  -H "anthropic-beta: managed-agents-${DATE}"
)
```

---

## Create an Environment

```bash
curl -X POST ${URL} \
  "${EXPR_1}" \
  -d '{
    "name": "my-dev-env",
    "config": {
      "type": "cloud",
      "networking": { "type": "unrestricted" }
    }
  }'
```

### With restricted networking

```bash
curl -X POST ${URL} \
  "${EXPR_2}" \
  -d '{
    "name": "restricted-env",
    "config": {
      "type": "cloud",
      "networking": {
        "type": "package_managers_and_custom",
        "allowed_hosts": ["api.example.com"]
      }
    }
  }'
```

---

## Create an Agent (required first step)

> ⚠️ **There is no inline agent config.** Under `managed-agents-${DATE}`, `model`/`system`/`tools` are top-level fields on `POST ${PATH}`, not on the session. Always create the agent first — the session only takes `"agent": {"type": "agent", "id": "..."}`.

### Minimal

```bash
# ${NUM}. Create the agent
curl -X POST ${URL} \
  "${EXPR_3}" \
  -d '{
    "name": "Coding Assistant",
    "model": "{{OPUS_ID}}",
    "tools": [{ "type": "agent_toolset_20260401" }]
  }'
# → { "id": "agent_abc123", ... }

# ${NUM}. Start a session
curl -X POST ${URL} \
  "${EXPR_4}" \
  -d '{
    "agent": { "type": "agent", "id": "agent_abc123", "version": "${NUM}" },
    "environment_id": "env_abc123"
  }'
```

### With system prompt, custom tools, and GitHub repo

```bash
# ${NUM}. Create the agent
curl -X POST ${URL} \
  "${EXPR_5}" \
  -d '{
    "name": "Code Reviewer",
    "model": "{{OPUS_ID}}",
    "system": "You are a senior code reviewer. Be thorough and constructive.",
    "tools": [
      { "type": "agent_toolset_20260401" },
      {
        "type": "custom",
        "name": "run_linter",
        "description": "Run the project linter on a file",
        "input_schema": {
          "type": "object",
          "properties": {
            "file_path": { "type": "string", "description": "Path to lint" }
          },
          "required": ["file_path"]
        }
      }
    ]
  }'

# ${NUM}. Start a session with the repo mounted
curl -X POST ${URL} \
  "${EXPR_6}" \
  -d '{
    "agent": { "type": "agent", "id": "agent_abc123", "version": "${NUM}" },
    "environment_id": "env_abc123",
    "title": "Code review session",
    "resources": [
      {
        "type": "github_repository",
        "url": "${URL}
        "mount_path": "${PATH}",
        "authorization_token": "ghp_...",
        "branch": "feature-branch"
      }
    ]
  }'
```

---

## Send a User Message

```bash
curl -X POST ${URL} \
  "${EXPR_7}" \
  -d '{
    "events": [
      {
        "type": "user.message",
        "content": [{ "type": "text", "text": "Review the auth module for security issues" }]
      }
    ]
  }'
```

---

## Stream Events (SSE)

```bash
curl -N ${URL} \
  "${EXPR_8}"
```

Response format:

```
event: session.status_running
data: {"type":"session.status_running","id":"sevt_...","processed_at":"..."}

event: agent.message
data: {"type":"agent.message","id":"sevt_...","content":[{"type":"text","text":"I'll review..."}],"processed_at":"..."}

event: session.status_idle
data: {"type":"session.status_idle","id":"sevt_...","processed_at":"..."}
```

---

## Poll Events

```bash
# Get all events
curl ${URL} \
  "${EXPR_9}"

# Paginated — get next page of events
curl "${URL} \
  "${EXPR_10}"
```

---

## Provide Custom Tool Result

When the agent calls a custom tool, send the result back:

```bash
curl -X POST ${URL} \
  "${EXPR_11}" \
  -d '{
    "events": [
      {
        "type": "user.custom_tool_result",
        "custom_tool_use_id": "sevt_abc123",
        "content": [{ "type": "text", "text": "No linting errors found." }]
      }
    ]
  }'
```

---

## Interrupt a Running Session

```bash
curl -X POST ${URL} \
  "${EXPR_12}" \
  -d '{
    "events": [
      {
        "type": "interrupt"
      }
    ]
  }'
```

---

## Get Session Details

```bash
curl ${URL} \
  "${EXPR_13}"
```

---

## List Sessions

```bash
curl ${URL} \
  "${EXPR_14}"
```

---

## Delete a Session

```bash
curl -X DELETE ${URL} \
  "${EXPR_15}"
```

---

## Upload a File

```bash
curl -X POST ${URL} \
  -H "x-api-key: $ANTHROPIC_API_KEY" \
  -H "anthropic-version: ${DATE}" \
  -H "anthropic-beta: files-api-${DATE}" \
  -F "file=@path${PATH}" \
  -F "purpose=agent"
```

---

## List and Download Session Files

List files the agent wrote to `${PATH}` during a session, then download them.

```bash
# List files associated with a session
curl "${URL} \
  "${EXPR_16}"

# Download a specific file
curl "${URL} \
  "${EXPR_17}" \
  -o downloaded_file.txt
```

---

## List Agents

```bash
curl ${URL} \
  "${EXPR_18}"
```

---

## MCP Server Integration

```bash
# ${NUM}. Agent declares MCP server (no auth here — auth goes in a vault)
curl -X POST ${URL} \
  "${EXPR_19}" \
  -d '{
    "name": "MCP Agent",
    "model": "{{OPUS_ID}}",
    "mcp_servers": [
      { "type": "url", "name": "my-tools", "url": "${URL} }
    ],
    "tools": [
      { "type": "agent_toolset_20260401" },
      { "type": "mcp_toolset", "mcp_server_name": "my-tools" }
    ]
  }'

# ${NUM}. Session attaches vault containing credentials for that MCP server URL
curl -X POST ${URL} \
  "${EXPR_20}" \
  -d '{
    "agent": "agent_abc123",
    "environment_id": "env_abc123",
    "vault_ids": ["vlt_abc123"]
  }'
```

See `shared${PATH}` §Vaults for creating vaults and adding credentials.

---

## Tool Configuration

```bash
curl -X POST ${URL} \
  "${EXPR_21}" \
  -d '{
    "name": "Restricted Agent",
    "model": "{{OPUS_ID}}",
    "tools": [
      {
        "type": "agent_toolset_20260401",
        "default_config": { "enabled": true },
        "configs": [
          { "name": "bash", "enabled": false }
        ]
      }
    ]
  }'
```
