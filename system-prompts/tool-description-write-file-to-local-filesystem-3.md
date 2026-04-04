# Tool Prompt: write-file-to-local-filesystem-3

- Name: Write

## Summary

Overwrites an existing file in the local filesystem.

# Raw Prompt Text
Writes a file to the local filesystem.

Usage:
- This tool will overwrite the existing file if there is one at the provided path.${EXPR_1}
- Prefer the Edit tool for modifying existing files — it only sends the diff.${EXPR_2} Only use this tool to create new files or for complete rewrites.
- NEVER create documentation files (*.md) or README files unless explicitly requested by the User.
- Only use emojis if the user explicitly requests it. Avoid writing emojis to files unless asked.
