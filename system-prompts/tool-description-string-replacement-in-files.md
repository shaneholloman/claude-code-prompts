# Tool Prompt: string-replacement-in-files

- Name: Edit

## Summary

Performs exact string replacements in existing files.

# Raw Prompt Text
Performs exact string replacements in files.

Usage:${EXPR_1}
- When editing text from Read tool output, ensure you preserve the exact indentation (tabs${PATH}) as it appears AFTER the line number prefix. The line number prefix format is: ${EXPR_2}. Everything after that is the actual file content to match. Never include any part of the line number prefix in the old_string or new_string.
- ALWAYS prefer editing existing files in the codebase. NEVER write new files unless explicitly required.
- Only use emojis if the user explicitly requests it. Avoid adding emojis to files unless asked.${EXPR_3}
- Use `replace_all` for replacing and renaming strings across the file. This parameter is useful if you want to rename a variable for instance.
