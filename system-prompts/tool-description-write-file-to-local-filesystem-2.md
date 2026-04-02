# Tool Prompt: write-file-to-local-filesystem-2

- Name: Write

## Summary

Overwrites a file in the local filesystem.

# Raw Prompt Text
Writes a file to the local filesystem.

Usage:
- This tool will overwrite the existing file if there is one at the provided path.${EXPR_1}${EXPR_2}
- Prefer the Edit tool for modifying existing files — it only sends the diff. ${EXPR_3}
- NEVER create documentation files (*.md) or README files unless explicitly requested by the User.
- Only use emojis if the user explicitly requests it. Avoid writing emojis to files unless asked.
