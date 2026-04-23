# System Prompt: live-documentation-sources

- Source: native-reference-match

## Summary

File for fetching current information from sources.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `OPUS_NAME` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |
| `EXPR_18` | None | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | None | None |
| `EXPR_22` | None | None |
| `EXPR_23` | None | None |

# Raw Prompt Text
# System Prompt: live-documentation-sources

- Source: inline

## Summary

File for fetching current information from sources.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `OPUS_NAME` | None | None |

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
| Models Overview | `${EXPR_1}        | "Extract current model IDs, context windows, and pricing for all Claude models" |
| Migration Guide | `${EXPR_2} | "Extract breaking changes, deprecated parameters, and per-model migration steps when moving to a newer Claude model" |
| Pricing         | `${EXPR_3}                             | "Extract current pricing per million tokens for input and output"               |

### Core Features

| Topic             | URL                                                                          | Extraction Prompt                                                                      |
| ----------------- | ---------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| Extended Thinking | `${EXPR_4} | "Extract extended thinking parameters, budget_tokens requirements, and usage examples" |
| Adaptive Thinking | `${EXPR_5} | "Extract adaptive thinking setup, effort levels, and {{OPUS_NAME}} usage examples"         |
| Effort Parameter  | `${EXPR_6}            | "Extract effort levels, cost-quality tradeoffs, and interaction with thinking"        |
| Tool Use          | `${EXPR_7}  | "Extract tool definition schema, tool_choice options, and handling tool results"       |
| Streaming         | `${EXPR_8}         | "Extract streaming event types, SDK examples, and best practices"                      |
| Prompt Caching    | `${EXPR_9}    | "Extract cache_control usage, pricing benefits, and implementation examples"           |

### Media & Files

| Topic       | URL                                                                    | Extraction Prompt                                                 |
| ----------- | ---------------------------------------------------------------------- | ----------------------------------------------------------------- |
| Vision      | `${EXPR_10}      | "Extract supported image formats, size limits, and code examples" |
| PDF Support | `${EXPR_11} | "Extract PDF handling capabilities, limits, and examples"         |

### API Operations

| Topic            | URL                                                                         | Extraction Prompt                                                                                       |
| ---------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| Batch Processing | `${EXPR_12} | "Extract batch API endpoints, request format, and polling for results"                                  |
| Files API        | `${EXPR_13}            | "Extract file upload, download, and referencing in messages, including supported types and beta header" |
| Token Counting   | `${EXPR_14}   | "Extract token counting API usage and examples"                                                         |
| Rate Limits      | `${EXPR_15}                    | "Extract current rate limits by tier and model"                                                         |
| Errors           | `${EXPR_16}                         | "Extract HTTP error codes, meanings, and retry guidance"                                                |

### Tools

| Topic          | URL                                                                                    | Extraction Prompt                                                                        |
| -------------- | -------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| Code Execution | `${EXPR_17} | "Extract code execution tool setup, file upload, container reuse, and response handling" |
| Computer Use   | `${EXPR_18}        | "Extract computer use tool setup, capabilities, and implementation examples"             |
| Bash Tool      | `${EXPR_19}           | "Extract bash tool schema, reference implementation, and security considerations"        |
| Text Editor    | `${EXPR_20}    | "Extract text editor tool commands, schema, and reference implementation"                |
| Memory Tool    | `${EXPR_21}         | "Extract memory tool commands, directory structure, and implementation patterns"         |
| Tool Search    | `${EXPR_22}    | "Extract tool search setup, when to use, and cache interaction"                          |
| Programmatic Tool Calling | `${EXPR_23} | "Extract PTC setup, script execution model, and tool invocation from code"    |
| Skills         | `${EXPR_24}                       | "Extract skill folder structure, SKILL.md format, and loading behavior"                  |

### Advanced Features

| Topic              | URL                                                                           | Extraction Prompt                                   |
| ------------------ | ----------------------------------------------------------------------------- | --------------------------------------------------- |
| Structured Outputs | `${EXPR_25} | "Extract output_config.format usage and schema enforcement"                           |
| Compaction         | `${EXPR_26}         | "Extract compaction setup, trigger config, and streaming with compaction"             |
| Context Editing    | `${EXPR_27}    | "Extract context editing thresholds, what gets cleared, and configuration"            |
| Citations          | `${EXPR_28}          | "Extract citation format and implementation"        |
| Context Windows    | `${EXPR_29}    | "Extract context window sizes and token management" |

### Managed Agents

Use these when a managed-agents binding, behavior, or wire-level detail isn't covered in the cached `shared${EXPR_30}*.md` concept files or in `{lang}${EXPR_31}`.

| Topic                 | URL                                                                              | Extraction Prompt                                                                               |
| --------------------- | -------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| Overview              | `${EXPR_32}                 | "Extract the high-level architecture and how agents${EXPR_33} fit together" |
| Quickstart            | `${EXPR_34}               | "Extract the minimal end-to-end agent → environment → session → stream code path"              |
| Agent Setup           | `${EXPR_35}              | "Extract agent create${EXPR_36} lifecycle and parameters"                   |
| Define Outcomes       | `${EXPR_37}          | "Extract outcome definitions, evaluation hooks, and success criteria configuration"             |
| Sessions              | `${EXPR_38}                 | "Extract session lifecycle, status transitions, idle${EXPR_39} semantics, and resume rules"    |
| Environments          | `${EXPR_40}             | "Extract environment config (cloud${EXPR_41}), management endpoints, and reuse model"          |
| Events and Streaming  | `${EXPR_42}     | "Extract event stream types, stream-first ordering, reconnect${EXPR_43}, and steering patterns"    |
| Tools                 | `${EXPR_44}                    | "Extract built-in toolset, custom tool definitions, and tool result wire format"                |
| Files                 | `${EXPR_45}                    | "Extract file upload, mount paths, session resources, and listing${EXPR_46} session outputs"  |
| Permission Policies   | `${EXPR_47}      | "Extract permission policy types (allow${EXPR_48}) and per-tool config"                     |
| Multi-Agent           | `${EXPR_49}              | "Extract multi-agent composition patterns, sub-agent invocation, and result handoff"            |
| Observability         | `${EXPR_50}            | "Extract logging, tracing, and usage telemetry exposed by managed agents"                       |
| GitHub                | `${EXPR_51}                   | "Extract github_repository resource shape, multi-repo mounting, and token rotation"             |
| MCP Connector         | `${EXPR_52}            | "Extract MCP server declaration on agents and vault-based credential injection at session"     |
| Vaults                | `${EXPR_53}                   | "Extract vault create, credential add${EXPR_54}, OAuth refresh shape, and archive"                 |
| Skills                | `${EXPR_55}                   | "Extract skill packaging and loading model for managed agents"                                  |
| Memory                | `${EXPR_56}                   | "Extract memory resource shape, scoping, and lifecycle"                                         |
| Onboarding            | `${EXPR_57}               | "Extract first-run setup, prerequisites, and account${EXPR_58} requirements"                      |
| Cloud Containers      | `${EXPR_59}         | "Extract cloud container runtime, image config, and network${EXPR_60} knobs"                     |
| Migration             | `${EXPR_61}                | "Extract migration paths from earlier APIs${EXPR_62} shapes to GA managed agents"                 |

### Anthropic CLI

The `ant` CLI provides terminal access to the Claude API. Every API resource is exposed as a subcommand. It is one convenient way to create agents, environments, sessions, and other resources from version-controlled YAML, and to inspect responses interactively.

| Topic         | URL                                                     | Extraction Prompt                                                                                  |
| ------------- | ------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| Anthropic CLI | `${EXPR_63}   | "Extract CLI install, authentication, command structure, and the beta:agents${EXPR_64} commands" |

---

## Claude API SDK Repositories

WebFetch these when a binding (class, method, namespace, field) isn't covered in the cached `{lang}/` skill files or in the managed-agents docs above. The SDKs include beta managed-agents support for `${EXPR_65}`, `${EXPR_66}`, `${EXPR_67}`, and related resources — search the repo for `BetaManagedAgents`, `beta.agents`, `beta.sessions`, or the equivalent namespace for that language.

| SDK        | URL                                                      | Extraction Prompt                                                                                                       |
| ---------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| Python     | `${EXPR_68}     | "Extract beta managed-agents namespaces, classes, and method signatures (`client.beta.agents`, `client.beta.sessions`)" |
| TypeScript | `${EXPR_69} | "Extract beta managed-agents namespaces, classes, and method signatures (`client.beta.agents`, `client.beta.sessions`)" |
| Java       | `${EXPR_70}       | "Extract beta managed-agents classes, builders, and method signatures (`client.beta().agents()`, `BetaManagedAgents*`)" |
| Go         | `${EXPR_71}         | "Extract beta managed-agents types and method signatures (`client.Beta.Agents`, `BetaManagedAgents*` event types)"      |
| Ruby       | `${EXPR_72}       | "Extract beta managed-agents methods and parameter shapes (`client.beta.agents`, `client.beta.sessions`)"               |
| C#         | `${EXPR_73}     | "Extract beta managed-agents classes and method signatures (NuGet package, `BetaManagedAgents*` types)"                 |
| PHP        | `${EXPR_74}        | "Extract beta managed-agents classes and method signatures (`$client->beta->agents`, `BetaManagedAgents*` params)"      |

---

## Fallback Strategy

If WebFetch fails (network issues, URL changed):

${EXPR_75}. Use cached content from the language-specific files (note the cache date)
${EXPR_76}. Inform user the data may be outdated
${EXPR_77}. Suggest they check platform.claude.com or the GitHub repos directly
