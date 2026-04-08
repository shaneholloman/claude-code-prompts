# System Prompt: managed-agents-endpoint-reference

- Source: inline

## Summary

Overview of managed agents API endpoints.

# Raw Prompt Text
# Managed Agents — Endpoint Reference

All endpoints require `x-api-key` and `anthropic-version: ${DATE}` headers. Managed Agents endpoints additionally require the `anthropic-beta` header.

## Beta Headers

```
anthropic-beta: managed-agents-${DATE}
```

The SDK adds this header automatically for all `client.beta.{agents,environments,sessions,vaults}.*` calls. Skills endpoints use `skills-${DATE}`; Files endpoints use `files-api-${DATE}`.

---

## SDK Method Reference

All resources are under the `beta` namespace. Python and TypeScript share identical method names.

| Resource | Python / TypeScript (`client.beta.*`) | Go (`client.Beta.*`) |
| --- | --- | --- |
| Agents | `agents.create` / `retrieve` / `update` / `list` / `archive` | `Agents.New` / `Get` / `Update` / `List` / `Archive` |
| Agent Versions | `agents.versions.list` | `Agents.Versions.List` |
| Environments | `environments.create` / `retrieve` / `update` / `list` / `delete` / `archive` | `Environments.New` / `Get` / `Update` / `List` / `Delete` / `Archive` |
| Sessions | `sessions.create` / `retrieve` / `update` / `list` / `delete` / `archive` | `Sessions.New` / `Get` / `Update` / `List` / `Delete` / `Archive` |
| Session Events | `sessions.events.list` / `send` / `stream` | `Sessions.Events.List` / `Send` / `StreamEvents` |
| Session Resources | `sessions.resources.add` / `retrieve` / `update` / `list` / `delete` | `Sessions.Resources.Add` / `Get` / `Update` / `List` / `Delete` |
| Vaults | `vaults.create` / `retrieve` / `update` / `list` / `delete` / `archive` | `Vaults.New` / `Get` / `Update` / `List` / `Delete` / `Archive` |
| Credentials | `vaults.credentials.create` / `retrieve` / `update` / `list` / `delete` / `archive` | `Vaults.Credentials.New` / `Get` / `Update` / `List` / `Delete` / `Archive` |

**Naming quirks to watch for:**
- Agents have **no delete** — only `archive`. Other resources have both.
- Session resources use `add` (not `create`).
- Go's event stream is `StreamEvents` (not `Stream`).

**Agent shorthand:** `agent` on session create accepts either a bare string (`agent="agent_abc123"` — uses latest version) or the full reference object (`{type: "agent", id: "agent_abc123", version: ${NUM}}`).

**Model shorthand:** `model` on agent create accepts either a bare string (`model="claude-opus-${NUM}-${NUM}"` — uses `standard` speed) or the full config object (`{type: "model_config", id: "claude-opus-${NUM}-${NUM}", speed: "fast"}`).

---

## Agents

**Step one of every flow.** Sessions require a pre-created agent — there is no inline agent config under `managed-agents-${DATE}`.

| Method   | Path                                             | Operation        | Description                              |
| -------- | ------------------------------------------------ | ---------------- | ---------------------------------------- |
| `GET` | `${PATH}` | ListAgents | List agents |
| `POST` | `${PATH}` | CreateAgent | Create a saved agent configuration |
| `GET` | `${PATH}{agent_id}` | GetAgent | Get agent details |
| `POST` | `${PATH}{agent_id}` | UpdateAgent | Update agent configuration |
| `POST` | `${PATH}{agent_id}${PATH}` | ArchiveAgent | Archive an agent (no hard delete for agents) |
| `GET` | `${PATH}{agent_id}${PATH}` | ListAgentVersions | List agent versions |

## Sessions

| Method   | Path                                             | Operation        | Description                              |
| -------- | ------------------------------------------------ | ---------------- | ---------------------------------------- |
| `GET` | `${PATH}` | ListSessions | List sessions (paginated) |
| `POST` | `${PATH}` | CreateSession | Create a new session |
| `GET` | `${PATH}{session_id}` | GetSession | Get session details |
| `POST` | `${PATH}{session_id}` | UpdateSession | Update session metadata${PATH} |
| `DELETE` | `${PATH}{session_id}` | DeleteSession | Delete a session |
| `POST` | `${PATH}{session_id}${PATH}` | ArchiveSession | Archive a session |

## Events

| Method   | Path                                             | Operation        | Description                              |
| -------- | ------------------------------------------------ | ---------------- | ---------------------------------------- |
| `GET` | `${PATH}{session_id}${PATH}` | ListEvents | List events (polling, paginated) |
| `POST` | `${PATH}{session_id}${PATH}` | SendEvents | Send events (user message, tool result) |
| `GET` | `${PATH}{session_id}${PATH}` | StreamEvents | Stream events via SSE |

## Session Resources

| Method   | Path                                                    | Operation        | Description                              |
| -------- | ------------------------------------------------------- | ---------------- | ---------------------------------------- |
| `GET` | `${PATH}{session_id}${PATH}` | ListResources | List resources attached to session |
| `POST` | `${PATH}{session_id}${PATH}` | AddResource | Attach file or github_repository mount (SDK method: `add`, not `create`) |
| `GET` | `${PATH}{session_id}${PATH}{resource_id}` | GetResource | Get a single resource |
| `POST` | `${PATH}{session_id}${PATH}{resource_id}` | UpdateResource | Update resource |
| `DELETE` | `${PATH}{session_id}${PATH}{resource_id}` | DeleteResource | Remove resource from session |

## Environments

| Method   | Path                                                             | Operation            | Description                         |
| -------- | ---------------------------------------------------------------- | -------------------- | ----------------------------------- |
| `POST`   | `${PATH}`                                     | CreateEnvironment    | Create environment                  |
| `GET`    | `${PATH}`                                     | ListEnvironments     | List environments                   |
| `GET`    | `${PATH}{environment_id}`                    | GetEnvironment       | Get environment details             |
| `POST`   | `${PATH}{environment_id}`                    | UpdateEnvironment    | Update environment                  |
| `DELETE` | `${PATH}{environment_id}`                    | DeleteEnvironment    | Delete environment. Returns ${NUM}. |
| `POST`   | `${PATH}{environment_id}${PATH}`            | ArchiveEnvironment   | Archive environment (read-only; existing sessions continue) |

## Vaults

Vaults store MCP credentials that Anthropic manages on your behalf — OAuth credentials with auto-refresh, or static bearer tokens. Attach to sessions via `vault_ids`. See `managed-agents-tools.md` §Vaults for the conceptual guide and credential shapes.

| Method   | Path                                             | Operation        | Description                              |
| -------- | ------------------------------------------------ | ---------------- | ---------------------------------------- |
| `POST`   | `${PATH}`                                     | CreateVault      | Create a vault                           |
| `GET`    | `${PATH}`                                     | ListVaults       | List vaults                              |
| `GET`    | `${PATH}{vault_id}`                          | GetVault         | Get vault details                        |
| `POST`   | `${PATH}{vault_id}`                          | UpdateVault      | Update vault                             |
| `DELETE` | `${PATH}{vault_id}`                          | DeleteVault      | Delete vault                             |
| `POST`   | `${PATH}{vault_id}${PATH}`                  | ArchiveVault     | Archive vault                            |

## Credentials

Credentials are individual secrets stored inside a vault.

| Method   | Path                                                              | Operation          | Description                  |
| -------- | ----------------------------------------------------------------- | ------------------ | ---------------------------- |
| `POST`   | `${PATH}{vault_id}${PATH}`                               | CreateCredential   | Create a credential          |
| `GET`    | `${PATH}{vault_id}${PATH}`                               | ListCredentials    | List credentials in vault    |
| `GET`    | `${PATH}{vault_id}${PATH}{credential_id}`               | GetCredential      | Get credential metadata      |
| `POST`   | `${PATH}{vault_id}${PATH}{credential_id}`               | UpdateCredential   | Update credential            |
| `DELETE` | `${PATH}{vault_id}${PATH}{credential_id}`               | DeleteCredential   | Delete credential            |
| `POST`   | `${PATH}{vault_id}${PATH}{credential_id}${PATH}`       | ArchiveCredential  | Archive credential           |

## Files

| Method   | Path                                             | Operation        | Description                              |
| -------- | ------------------------------------------------ | ---------------- | ---------------------------------------- |
| `POST`   | `${PATH}`                            | UploadFile       | Upload a file                            |
| `GET`    | `${PATH}`                            | ListFiles        | List files                               |
| `GET`    | `${PATH}{file_id}`                  | GetFile          | Get file metadata (SDK method: `retrieve_metadata`) |
| `GET`    | `${PATH}{file_id}${PATH}`          | DownloadFile     | Download file content                    |
| `DELETE` | `${PATH}{file_id}`                  | DeleteFile       | Delete a file                            |

## Skills

| Method   | Path                                                            | Operation          | Description                  |
| -------- | --------------------------------------------------------------- | ------------------ | ---------------------------- |
| `POST`   | `${PATH}`                                          | CreateSkill        | Create a skill               |
| `GET`    | `${PATH}`                                          | ListSkills         | List skills                  |
| `GET`    | `${PATH}{skill_id}`                               | GetSkill           | Get skill details            |
| `DELETE` | `${PATH}{skill_id}`                               | DeleteSkill        | Delete a skill               |
| `POST`   | `${PATH}{skill_id}${PATH}`                      | CreateVersion      | Create skill version         |
| `GET`    | `${PATH}{skill_id}${PATH}`                      | ListVersions       | List skill versions          |
| `GET`    | `${PATH}{skill_id}${PATH}{version}`            | GetVersion         | Get skill version            |
| `DELETE` | `${PATH}{skill_id}${PATH}{version}`            | DeleteVersion      | Delete skill version         |

---

## Request${PATH} Schema Quick Reference

### CreateAgent Request Body

**Always start here.** `model`, `system`, `tools`, `mcp_servers`, `skills` are top-level fields on this object — they do NOT go on the session.

```json
{
  "name": "string (required, ${NUM}-${NUM} chars)",
  "model": "{{OPUS_ID}} (required — bare string, or {id, speed} object)",
  "description": "string (optional, up to ${NUM} chars)",
  "system": "string (optional, up to ${NUM},${NUM} chars)",
  "tools": [
    { "type": "agent_toolset_20260401" }
  ],
  "skills": [
    { "type": "anthropic", "skill_id": "xlsx" },
    { "type": "custom", "skill_id": "skill_abc123", "version": "${NUM}" }
  ],
  "mcp_servers": [
    {
      "type": "url",
      "name": "github",
      "url": "${URL}
    }
  ],
  "metadata": {
    "key": "value (max ${NUM} pairs, keys ≤${NUM} chars, values ≤${NUM} chars)"
  }
}
```

> Limits: `tools` max ${NUM}, `skills` max ${NUM}, `mcp_servers` max ${NUM} (unique names).

### CreateSession Request Body

```json
{
  "agent": "agent_abc123 (required — string shorthand for latest version, or {type: \"agent\", id, version} object)",
  "environment_id": "env_abc123 (required)",
  "title": "string (optional)",
  "resources": [
    {
      "type": "github_repository",
      "url": "${URL} (required)",
      "authorization_token": "ghp_... (required)",
      "mount_path": "${PATH} (optional — defaults to ${PATH}<repo-name>)",
      "checkout": { "type": "branch", "name": "main" }
    }
  ],
  "vault_ids": ["vlt_abc123 (optional — MCP credentials with auto-refresh)"],
  "metadata": {
    "key": "value"
  }
}
```

> The `agent` field accepts only a string ID or `{type: "agent", id, version}` — `model`/`system`/`tools` live on the agent, not here.
>
> **`checkout`** accepts `{type: "branch", name: "..."}` or `{type: "commit", sha: "..."}`. Omit for the repo's default branch.

### CreateEnvironment Request Body

```json
{
  "name": "string (required)",
  "description": "string (optional)",
  "config": {
    "type": "cloud",
    "networking": {
      "type": "unrestricted | limited (union — see SDK types)"
    },
    "packages": { }
  },
  "metadata": { "key": "value" }
}
```

### SendEvents Request Body

```json
{
  "events": [
    {
      "type": "user.message",
      "content": [
        {
          "type": "text",
          "text": "Hello"
        }
      ]
    }
  ]
}
```

### Tool Result Event

```json
{
  "type": "user.custom_tool_result",
  "custom_tool_use_id": "sevt_abc123",
  "content": [{ "type": "text", "text": "Result data" }],
  "is_error": false
}
```

---

## Error Handling

Managed Agents endpoints use the standard Anthropic API error format. Errors are returned with an HTTP status code and a JSON body containing `type`, `error`, and `request_id`:

```json
{
  "type": "error",
  "error": {
    "type": "invalid_request_error",
    "message": "Description of what went wrong"
  },
  "request_id": "req_011CRv1W3XQ8XpFikNYG7RnE"
}
```

Include the `request_id` when reporting issues to Anthropic — it lets us trace the request end-to-end. The inner `error.type` is one of the following:

| Status | Error type | Description |
|---|---|---|
| ${NUM} | `invalid_request_error` | The request was malformed or missing required parameters |
| ${NUM} | `authentication_error` | Invalid or missing API key |
| ${NUM} | `permission_error` | The API key doesn't have permission for this operation |
| ${NUM} | `not_found_error` | The requested resource doesn't exist |
| ${NUM} | `invalid_request_error` | The request conflicts with the resource's current state (e.g., sending to an archived session) |
| ${NUM} | `request_too_large` | The request body exceeds the maximum allowed size |
| ${NUM} | `rate_limit_error` | Too many requests — check rate limit headers for retry timing |
| ${NUM} | `api_error` | An internal server error occurred |
| ${NUM} | `overloaded_error` | The service is temporarily overloaded — retry with backoff |

Note that `${NUM} Conflict` carries `error.type: "invalid_request_error"` (there is no separate `conflict_error` type); inspect both the HTTP status and the `message` to distinguish conflicts from other invalid requests.

---

## Rate Limits

Managed Agents endpoints have per-organization request-per-minute (RPM) limits, separate from your [Messages API token limits](${URL}). Model inference inside a session still draws from your organization's standard ITPM${PATH} limits.

| Endpoint group | Scope | RPM | Max concurrent |
|---|---|---|---|
| Create operations (Agents, Sessions, Vaults) | organization | ${NUM} | — |
| All other operations (Agents, Sessions, Vaults) | organization | ${NUM} | — |
| All operations (Environments) | organization | ${NUM} | ${NUM} |

Files and Skills endpoints use the standard tier-based [rate limits](${URL}).

When a limit is exceeded the API returns `${NUM}` with a `rate_limit_error` (see [Error Handling](#error-handling) for the response envelope) and a `retry-after` header indicating how many seconds to wait before retrying. The Anthropic SDK reads this header and retries automatically.
