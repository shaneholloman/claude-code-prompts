# System Prompt: write-file-to-local-filesystem-2

- Source: inline

## Summary

Writes a file to the local filesystem with checks.

# Raw Prompt Text
Writes a file to the local filesystem.

Usage:
- This tool will overwrite the existing file if there is one at the provided path.
- If this is an existing file, you MUST use the Read tool first to read the file's contents. This tool will fail if you did not read the file first.${EXPR_1}
- Prefer the Edit tool for modifying existing files — it only sends the diff. ${EXPR_2}
- NEVER create documentation files (*.md) or README files unless explicitly requested by the User.
- Only use emojis if the user explicitly requests it. Avoid writing emojis to files unless asked.
