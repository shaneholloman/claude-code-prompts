# Tool Description: exact-replacements-with-count-check

- Name: Edit

## Summary

Exact in-file string replacement with occurrence validation and prefix handling.

# Raw Prompt Text
Performs exact string replacements in files with strict occurrence count validation.

Usage:
- When editing text from Read tool output, ensure you preserve the exact indentation (tabs${PATH}) as it appears AFTER the line number prefix. The line number prefix format is: spaces + line number + tab. Everything after that tab is the actual file content to match. Never include any part of the line number prefix in the old_string or new_string.
- ALWAYS prefer editing existing files in the codebase. NEVER write new files unless explicitly required.
