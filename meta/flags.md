# Claude Code 0.2.29 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `contents_identical` | gate | other | Detects identical message contents to avoid further comparison or resolution. | Exact effect of W() and return value semantics unclear. | medium | 2 |
| `tengu_motd` | config | ui | Fetches and renders a message-of-the-day UI element with theming | Config includes message and optional color mapped by theme. | high | 1 |
| `tengu_sticker_easter_egg` | gate | tools | toggles availability of a sticker request tool/form in the CLI | Only seen gating isEnabled for StickerRequest tool. | medium | 1 |
| `tengu_think_tool` | gate | tools | Enables a Think tool that logs user-provided thoughts for internal use. | Gated by env var and runtime check; appears to log thoughts. | high | 1 |
| `tengu_version_config` | config | ui | Checks minimum required CLI version and instructs user to update if outdated. | Used for runtime version gating and update messaging. | high | 1 |
| `tool_use_invalid` | gate | tools | Detects invalid tool call content during message comparison and aborts | Based on tool_use validation logic in CLI diff/compare flow. | high | 1 |
