# Tool Description: write-file-to-local-filesystem-3

- Source: native-reference-match

## Summary

Tool Description: write-file-to-local-filesystem-… - Source: native-reference-match Summary Tool Description: write-file-to-local-filesystem-… - Name: Write…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# Tool Description: write-file-to-local-filesystem-${NUM}

- Source: native-reference-match

## Summary

Tool Description: write-file-to-local-filesystem-… - Name: Write Summary Overwrites an existing file in the local filesystem.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
# Tool Description: write-file-to-local-filesystem-${EXPR_1}

- Name: Write

## Summary

Overwrites an existing file in the local filesystem.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Writes a file to the local filesystem.

Usage:
- This tool will overwrite the existing file if there is one at the provided path.${EXPR_2}
- Prefer the Edit tool for modifying existing files — it only sends the diff. Only use this tool to create new files or for complete rewrites.
- NEVER create documentation files (*.md) or README files unless explicitly requested by the User.
- Only use emojis if the user explicitly requests it. Avoid writing emojis to files unless asked.
