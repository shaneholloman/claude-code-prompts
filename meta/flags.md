# Claude Code 0.2.92 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `contents_identical` | gate | other | Detects identical message contents to avoid further comparison or resolution. | Exact effect of W() and return value semantics unclear. | medium | 2 |
| `force_local_installation_migration` | gate | tools | Forces CLI migration from global npm install to local installation with restart prompt | Triggered only when additional runtime checks pass. | high | 1 |
| `missing_text_or_edit` | gate | telemetry | Detects invalid message edit when required text or tool call is missing | Appears to log/track edit validation failures via nu2(). | high | 1 |
| `tengu_motd` | config | ui | Fetches and renders a message-of-the-day UI element with theming | Config includes message and optional color mapped by theme. | high | 1 |
| `tengu_version_config` | config | ui | Checks minimum required CLI version and instructs user to update if outdated. | Used for runtime version gating and update messaging. | high | 1 |
| `tool_use_invalid` | gate | tools | Detects invalid tool call content during message comparison and aborts | Based on tool_use validation logic in CLI diff/compare flow. | high | 1 |
