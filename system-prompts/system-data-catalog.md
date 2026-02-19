# System Data Block: catalog

- Source: inline

## Summary

Authoritative list of valid Claude model IDs, aliases, and statuses.

# Raw Prompt Text
# Claude Model Catalog

**Only use exact model IDs listed in this file.** Never guess or construct model IDs — incorrect IDs will cause API errors. Use aliases wherever available. For the latest information, WebFetch the Models Overview URL in `shared${PATH}`.

## Current Models (recommended)

| Friendly Name     | Alias (use this)    | Full ID                       | Context | Status |
|-------------------|---------------------|-------------------------------|---------|--------|
| Claude Opus ${NUM}   | `claude-opus-${NUM}-${NUM}`   | —                             | 200K    | Active |
| Claude Sonnet ${NUM} | `claude-sonnet-${NUM}-${NUM}` | -                             | 200K    | Active |
| Claude Haiku ${NUM}  | `claude-haiku-${NUM}-${NUM}`  | `claude-haiku-${NUM}-${NUM}-${NUM}`   | 200K    | Active |

## Legacy Models (still active)

| Friendly Name     | Alias (use this)    | Full ID                       | Status |
|-------------------|---------------------|-------------------------------|--------|
| Claude Opus ${NUM}   | `claude-opus-${NUM}-${NUM}`   | `claude-opus-${NUM}-${NUM}-${NUM}`    | Active |
| Claude Opus ${NUM}   | `claude-opus-${NUM}-${NUM}`   | `claude-opus-${NUM}-${NUM}-${NUM}`    | Active |
| Claude Sonnet ${NUM} | `claude-sonnet-${NUM}-${NUM}` | `claude-sonnet-${NUM}-${NUM}-${NUM}`  | Active |
| Claude Sonnet ${NUM}   | `claude-sonnet-${NUM}-${NUM}` | `claude-sonnet-${NUM}-${NUM}`    | Active |
| Claude Opus ${NUM}     | `claude-opus-${NUM}-${NUM}`   | `claude-opus-${NUM}-${NUM}`      | Active |
| Claude Haiku ${NUM}    | —                   | `claude-${NUM}-haiku-${NUM}`     | Active |

## Deprecated Models (retiring soon)

| Friendly Name     | Full ID                       | Retirement Date  |
|-------------------|-------------------------------|------------------|
| Claude Sonnet ${NUM} | `claude-${NUM}-${NUM}-sonnet-${NUM}`  | Feb ${NUM}, ${NUM}     |
| Claude Haiku ${NUM}  | `claude-${NUM}-${NUM}-haiku-${NUM}`   | Feb ${NUM}, ${NUM}     |

## Retired Models (no longer available)

| Friendly Name     | Full ID                       | Retired     |
|-------------------|-------------------------------|-------------|
| Claude Opus ${NUM}     | `claude-${NUM}-opus-${NUM}`      | Jan ${NUM}, ${NUM} |
| Claude Sonnet ${NUM} | `claude-${NUM}-${NUM}-sonnet-${NUM}`  | Oct ${NUM}, ${NUM} |
| Claude Sonnet ${NUM} | `claude-${NUM}-${NUM}-sonnet-${NUM}`  | Oct ${NUM}, ${NUM} |
| Claude Sonnet ${NUM}   | `claude-${NUM}-sonnet-${NUM}`    | Jul ${NUM}, ${NUM} |
| Claude ${NUM}        | `claude-${NUM}`                  | Jul ${NUM}, ${NUM} |
| Claude ${NUM}        | `claude-${NUM}`                  | Jul ${NUM}, ${NUM} |

## Resolving User Requests

When a user asks for a model by name, use this table to find the correct model ID:

| User says...                              | Use this model ID              |
|-------------------------------------------|--------------------------------|
| "opus", "most powerful"                   | `claude-opus-${NUM}-${NUM}`              |
| "opus ${NUM}"                                | `claude-opus-${NUM}-${NUM}`              |
| "opus ${NUM}"                                | `claude-opus-${NUM}-${NUM}`              |
| "opus ${NUM}"                                | `claude-opus-${NUM}-${NUM}`              |
| "opus ${NUM}", "opus ${NUM}"                      | `claude-opus-${NUM}-${NUM}`              |
| "sonnet", "balanced"                      | `claude-sonnet-${NUM}-${NUM}`            |
| "sonnet ${NUM}"                              | `claude-sonnet-${NUM}-${NUM}`            |
| "sonnet ${NUM}"                              | `claude-sonnet-${NUM}-${NUM}`            |
| "sonnet ${NUM}", "sonnet ${NUM}"                  | `claude-sonnet-${NUM}-${NUM}`            |
| "sonnet ${NUM}"                              | `claude-${NUM}-${NUM}-sonnet-${NUM}` (deprecated) |
| "sonnet ${NUM}"                              | Retired — suggest `claude-sonnet-${NUM}-${NUM}` |
| "haiku", "fast", "cheap"                  | `claude-haiku-${NUM}-${NUM}`             |
| "haiku ${NUM}"                               | `claude-haiku-${NUM}-${NUM}`             |
| "haiku ${NUM}"                               | `claude-${NUM}-${NUM}-haiku-${NUM}` (deprecated) |
| "haiku ${NUM}"                                 | `claude-${NUM}-haiku-${NUM}`      |
