# System Prompt: managed-agents-onboarding-flow

- Source: inline

## Summary

Guide for setting up a Managed Agent from scratch.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `OPUS_ID` | None | None |

# Raw Prompt Text
# Managed Agents — Onboarding Flow

> **Invoked via `${PATH} managed-agents-onboard`?** You're in the right place. Run the interview below — don't summarize it back to the user, ask the questions.

Use this when a user wants to set up a Managed Agent from scratch. Three steps: **branch on know-vs-explore → configure the template → set up the session**. End by emitting working code.

> Read `shared${PATH}` alongside this — it has full detail for each knob. This doc is the interview script, not the reference.

---

Claude Managed Agents is a hosted agent: Anthropic runs the agent loop on its orchestration layer and provisions a sandboxed container per session where the agent's tools execute. You supply the agent config and the environment config; the harness — event stream, sandbox orchestration, prompt caching, context compaction, and extended thinking — is handled for you.

**What you supply:**
- **An agent config** — tools, skills, model, system prompt. Reusable and versioned.
- **An environment config** — the sandbox your agent's tools execute in (networking, packages). Reusable across agents.

Each run of the agent is a **session**.

---

## ${NUM}. Know or explore?

Ask the user:

> Do you already know the agent you want to build, or would you like to explore some common patterns first?

### Explore path — show the patterns

Four shapes, same runtime code path (`sessions.create()` → `sessions.events.send()` → stream). Only the trigger and sink differ.

| Pattern | Trigger | Example |
|---|---|---|
| Event-triggered | Webhook | GitHub PR push → CMA (GitHub tool) → Slack | # <------ MC maybe delete?
| Scheduled | Cron | Daily brief: browser + GitHub + Jira → CMA → Slack | # <------ MC maybe delete?
| Fire-and-forget PR | Human | Slack slash-command → CMA (GitHub tool) → PR passing CI |
| Research + dashboard | Human | Topic → CMA (web search + `frontend-design` skill) → HTML dashboard |

Ask which shape fits, then continue with the Know path using it as the reference.

### Know path — configure template

Three rounds. Batch the questions in each round; don't ask them one at a time.

**Round A — Tools.** Start here; it's the most concrete part. Three types; ask which the user wants (any combination):

| Type | What it is | How to guide |
|---|---|---|
| **Prebuilt Claude Agent tools** (`agent_toolset_20260401`) | Ready-to-use: `bash`, `read`, `write`, `edit`, `glob`, `grep`, `web_fetch`, `web_search`. Enable all at once, or individually via `enabled: true${PATH}`. | Recommend enabling the full toolset. List the ${NUM} tools so the user knows what they're getting. Full detail: `shared${PATH}` → Agent Toolset. |
| **MCP tools** | Third-party integrations (GitHub, Linear, Asana, etc.) via `mcp_toolset`. Credentials live in a vault, not inline. | Ask which services. For each, walk through MCP server URL + vault credentials. Full detail: `shared${PATH}` → MCP Servers + Vaults. |
| **Custom tools** | The user's own app handles these tool calls — agent fires `agent.custom_tool_use`, the app sends a result message back. | Ask for each tool: name, description, input schema. The app code that handles the event is *their* code — don't generate it. Full detail: `shared${PATH}` → Custom Tools. |

**Round B — Skills, files, and repos.** What the agent has on hand when it starts.

*Skills* — two types; both work the same way — Claude auto-uses them when relevant. Max ${NUM} per agent.
- [ ] **Pre-built Agent Skills**: `xlsx`, `docx`, `pptx`, `pdf`. Reference by name.
- [ ] **Custom Skills**: skills uploaded to the user's org via the Skills API. Reference by `skill_id` + optional `version`. If the skill doesn't exist yet, walk the user through `POST ${PATH}` + `POST ${PATH}{id}${PATH}` (beta header `skills-${DATE}`). Full detail: `shared${PATH}` → Skills + Skills API.

*GitHub repositories* — any repos the agent needs on-disk? For each:
- [ ] Repo URL (`${URL})
- [ ] `authorization_token` (PAT or GitHub App token scoped to the repo)
- [ ] Optional `mount_path` (defaults to `${PATH}<repo-name>`) and `checkout` (branch or SHA)

Emit as `resources: [{type: "github_repository", url, authorization_token, ...}]`. Full detail: `shared${PATH}` → GitHub Repositories.

> ‼️ **PR creation needs the GitHub MCP server too.** `github_repository` gives filesystem access only — to open PRs, also attach the GitHub MCP server in Round A and credential it via a vault. The workflow is: edit files in the mounted repo → push branch via `bash` → create PR via the MCP `create_pull_request` tool.

*Files* — any local files to seed the session with? For each:
- [ ] Upload via the Files API → persist `file_id`
- [ ] Choose a `mount_path` — absolute, e.g. `${PATH}` (parents auto-created; files mount read-only)

Emit as `resources: [{type: "file", file_id, mount_path}]`. Max ${NUM} file resources. Agent working directory defaults to `${PATH}`. Full detail: `shared${PATH}` → Files API.

**Round C — Environment + identity:**
- [ ] Networking: unrestricted internet from the container, or lock egress to specific hosts? (If locked, MCP server domains must be in `allowed_hosts` or tools silently fail.)
- [ ] Name?
- [ ] Job (one or two sentences — becomes the system prompt)?
- [ ] Model? (default `{{OPUS_ID}}`)

---

## ${NUM}. Set up the session

Per-run. Points at the agent + environment, attaches credentials, kicks off.

**Vault credentials** (if the agent declared MCP servers):
- [ ] Existing vault, or create one? (`client.beta.vaults.create()` + `vaults.credentials.create()`)

Credentials are write-only, matched to MCP servers by URL, auto-refreshed. See `shared${PATH}` → Vaults.

**Kickoff:**
- [ ] First message to the agent?

Session creation blocks until all resources mount. Open the event stream before sending the kickoff. Stream is SSE; break on `session.status_terminated`, or on `session.status_idle` with a terminal `stop_reason` — i.e. anything except `requires_action`, which fires transiently while the session waits on a tool confirmation or custom-tool result (see `shared${PATH}` Pattern ${NUM}). Usage lands on `span.model_request_end`. Agent-written artifacts end up in `${PATH}` — download via `files.list({scope_id: session.id, betas: ["managed-agents-${DATE}"]})`.

---

## ${NUM}. Emit the code

Go straight from the last interview answer to the code — no preamble about the setup-vs-runtime split, no "the critical thing to internalize…", no lecture about `agents.create()` being one-time. The two-block structure below already shows that; don't narrate it. Generate **two clearly-separated blocks** per language detected (Python${PATH} — see SKILL.md → Language Detection):

**Block ${NUM} — Setup (run once, store the IDs):**
${NUM}. `environments.create()` → persist `env_id`
${NUM}. `agents.create()` with everything from §Round A–C → persist `agent_id` and `agent_version`

Label: `# ONE-TIME SETUP — run once, save the IDs to config${PATH}`

**Block ${NUM} — Runtime (run on every invocation):**
${NUM}. Load `env_id` + `agent_id` from config${PATH}
${NUM}. `sessions.create(agent=AGENT_ID, environment_id=ENV_ID, resources=[...], vault_ids=[...])`
${NUM}. Open stream, `events.send()` the kickoff, loop until `session.status_terminated` or `session.status_idle && stop_reason.type !== 'requires_action'` (see `shared${PATH}` Pattern ${NUM} for the full gate — do not break on bare `session.status_idle`)

> ⚠️ **Never emit `agents.create()` and `sessions.create()` in the same unguarded block.** That teaches the user to create a new agent on every run — the #${NUM} anti-pattern. If they need a single script, wrap agent creation in `if not os.getenv("AGENT_ID"):`.

Pull exact syntax from `python${PATH}`, `typescript${PATH}`, or `curl${PATH}`. Don't invent field names.
