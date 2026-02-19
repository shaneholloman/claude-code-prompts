# Claude Code 0.2.9 – Flags

| Flag | Type | Category | Summary | Notes | Confidence | Occurrences |
| --- | --- | --- | --- | --- | --- | ---: |
| `tengu_sticker_easter_egg` | gate | tools | toggles availability of a sticker request tool/form in the CLI | Only seen gating isEnabled for StickerRequest tool. | medium | 1 |
| `tengu_think_tool` | gate | tools | Enables a Think tool that logs user-provided thoughts for internal use. | Gated by env var and runtime check; appears to log thoughts. | high | 1 |
