# System Prompt: live-documentation-sources

- Source: inline

## Summary

File for fetching current information from sources.

# Raw Prompt Text
# Live Documentation Sources

This file contains WebFetch URLs for fetching current information from platform.claude.com and Agent SDK repositories. Use these when users need the latest data that may have changed since the cached content was last updated.

## When to Use WebFetch

- User explicitly asks for "latest" or "current" information
- Cached data seems incorrect
- User asks about features not covered in cached content
- User needs specific API details or examples

## Claude API Documentation URLs

### Models & Pricing

| Topic           | URL                                                                          | Extraction Prompt                                                               |
| --------------- | ---------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| Models Overview | `${URL}        | "Extract current model IDs, context windows, and pricing for all Claude models" |
| Pricing         | `${URL}                             | "Extract current pricing per million tokens for input and output"               |

### Core Features

| Topic             | URL                                                                          | Extraction Prompt                                                                      |
| ----------------- | ---------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| Extended Thinking | `${URL} | "Extract extended thinking parameters, budget_tokens requirements, and usage examples" |
| Adaptive Thinking | `${URL} | "Extract adaptive thinking setup, effort levels, and {{OPUS_NAME}} usage examples"         |
| Effort Parameter  | `${URL}            | "Extract effort levels, cost-quality tradeoffs, and interaction with thinking"        |
| Tool Use          | `${URL}  | "Extract tool definition schema, tool_choice options, and handling tool results"       |
| Streaming         | `${URL}         | "Extract streaming event types, SDK examples, and best practices"                      |
| Prompt Caching    | `${URL}    | "Extract cache_control usage, pricing benefits, and implementation examples"           |

### Media & Files

| Topic       | URL                                                                    | Extraction Prompt                                                 |
| ----------- | ---------------------------------------------------------------------- | ----------------------------------------------------------------- |
| Vision      | `${URL}      | "Extract supported image formats, size limits, and code examples" |
| PDF Support | `${URL} | "Extract PDF handling capabilities, limits, and examples"         |

### API Operations

| Topic            | URL                                                                         | Extraction Prompt                                                                                       |
| ---------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| Batch Processing | `${URL} | "Extract batch API endpoints, request format, and polling for results"                                  |
| Files API        | `${URL}            | "Extract file upload, download, and referencing in messages, including supported types and beta header" |
| Token Counting   | `${URL}   | "Extract token counting API usage and examples"                                                         |
| Rate Limits      | `${URL}                    | "Extract current rate limits by tier and model"                                                         |
| Errors           | `${URL}                         | "Extract HTTP error codes, meanings, and retry guidance"                                                |

### Tools

| Topic          | URL                                                                                    | Extraction Prompt                                                                        |
| -------------- | -------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| Code Execution | `${URL} | "Extract code execution tool setup, file upload, container reuse, and response handling" |
| Computer Use   | `${URL}        | "Extract computer use tool setup, capabilities, and implementation examples"             |
| Bash Tool      | `${URL}           | "Extract bash tool schema, reference implementation, and security considerations"        |
| Text Editor    | `${URL}    | "Extract text editor tool commands, schema, and reference implementation"                |
| Memory Tool    | `${URL}         | "Extract memory tool commands, directory structure, and implementation patterns"         |
| Tool Search    | `${URL}    | "Extract tool search setup, when to use, and cache interaction"                          |
| Programmatic Tool Calling | `${URL} | "Extract PTC setup, script execution model, and tool invocation from code"    |
| Skills         | `${URL}                       | "Extract skill folder structure, SKILL.md format, and loading behavior"                  |

### Advanced Features

| Topic              | URL                                                                           | Extraction Prompt                                   |
| ------------------ | ----------------------------------------------------------------------------- | --------------------------------------------------- |
| Structured Outputs | `${URL} | "Extract output_config.format usage and schema enforcement"                           |
| Compaction         | `${URL}         | "Extract compaction setup, trigger config, and streaming with compaction"             |
| Context Editing    | `${URL}    | "Extract context editing thresholds, what gets cleared, and configuration"            |
| Citations          | `${URL}          | "Extract citation format and implementation"        |
| Context Windows    | `${URL}    | "Extract context window sizes and token management" |

### Managed Agents

Use these when a managed-agents binding, behavior, or wire-level detail isn't covered in the cached `shared${PATH}*.md` concept files or in `{lang}${PATH}`.

| Topic                 | URL                                                                              | Extraction Prompt                                                                               |
| --------------------- | -------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| Overview              | `${URL}                 | "Extract the high-level architecture and how agents${PATH} fit together" |
| Quickstart            | `${URL}               | "Extract the minimal end-to-end agent → environment → session → stream code path"              |
| Agent Setup           | `${URL}              | "Extract agent create${PATH} lifecycle and parameters"                   |
| Define Outcomes       | `${URL}          | "Extract outcome definitions, evaluation hooks, and success criteria configuration"             |
| Sessions              | `${URL}                 | "Extract session lifecycle, status transitions, idle${PATH} semantics, and resume rules"    |
| Environments          | `${URL}             | "Extract environment config (cloud${PATH}), management endpoints, and reuse model"          |
| Events and Streaming  | `${URL}     | "Extract event stream types, stream-first ordering, reconnect${PATH}, and steering patterns"    |
| Tools                 | `${URL}                    | "Extract built-in toolset, custom tool definitions, and tool result wire format"                |
| Files                 | `${URL}                    | "Extract file upload, mount paths, session resources, and listing${PATH} session outputs"  |
| Permission Policies   | `${URL}      | "Extract permission policy types (allow${PATH}) and per-tool config"                     |
| Multi-Agent           | `${URL}              | "Extract multi-agent composition patterns, sub-agent invocation, and result handoff"            |
| Observability         | `${URL}            | "Extract logging, tracing, and usage telemetry exposed by managed agents"                       |
| GitHub                | `${URL}                   | "Extract github_repository resource shape, multi-repo mounting, and token rotation"             |
| MCP Connector         | `${URL}            | "Extract MCP server declaration on agents and vault-based credential injection at session"     |
| Vaults                | `${URL}                   | "Extract vault create, credential add${PATH}, OAuth refresh shape, and archive"                 |
| Skills                | `${URL}                   | "Extract skill packaging and loading model for managed agents"                                  |
| Memory                | `${URL}                   | "Extract memory resource shape, scoping, and lifecycle"                                         |
| Onboarding            | `${URL}               | "Extract first-run setup, prerequisites, and account${PATH} requirements"                      |
| Cloud Containers      | `${URL}         | "Extract cloud container runtime, image config, and network${PATH} knobs"                     |
| Migration             | `${URL}                | "Extract migration paths from earlier APIs${PATH} shapes to GA managed agents"                 |

### Anthropic CLI

The `ant` CLI provides terminal access to the Claude API. Every API resource is exposed as a subcommand. It is one convenient way to create agents, environments, sessions, and other resources from version-controlled YAML, and to inspect responses interactively.

| Topic         | URL                                                     | Extraction Prompt                                                                                  |
| ------------- | ------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| Anthropic CLI | `${URL}   | "Extract CLI install, authentication, command structure, and the beta:agents${PATH} commands" |

---

## Claude API SDK Repositories

WebFetch these when a binding (class, method, namespace, field) isn't covered in the cached `{lang}/` skill files or in the managed-agents docs above. The SDKs include beta managed-agents support for `${PATH}`, `${PATH}`, `${PATH}`, and related resources — search the repo for `BetaManagedAgents`, `beta.agents`, `beta.sessions`, or the equivalent namespace for that language.

| SDK        | URL                                                      | Extraction Prompt                                                                                                       |
| ---------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| Python     | `${URL}     | "Extract beta managed-agents namespaces, classes, and method signatures (`client.beta.agents`, `client.beta.sessions`)" |
| TypeScript | `${URL} | "Extract beta managed-agents namespaces, classes, and method signatures (`client.beta.agents`, `client.beta.sessions`)" |
| Java       | `${URL}       | "Extract beta managed-agents classes, builders, and method signatures (`client.beta().agents()`, `BetaManagedAgents*`)" |
| Go         | `${URL}         | "Extract beta managed-agents types and method signatures (`client.Beta.Agents`, `BetaManagedAgents*` event types)"      |
| Ruby       | `${URL}       | "Extract beta managed-agents methods and parameter shapes (`client.beta.agents`, `client.beta.sessions`)"               |
| C#         | `${URL}     | "Extract beta managed-agents classes and method signatures (NuGet package, `BetaManagedAgents*` types)"                 |
| PHP        | `${URL}        | "Extract beta managed-agents classes and method signatures (`$client->beta->agents`, `BetaManagedAgents*` params)"      |

---

## Fallback Strategy

If WebFetch fails (network issues, URL changed):

${NUM}. Use cached content from the language-specific files (note the cache date)
${NUM}. Inform user the data may be outdated
${NUM}. Suggest they check platform.claude.com or the GitHub repos directly
