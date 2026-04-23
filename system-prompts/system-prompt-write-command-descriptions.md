# System Prompt: write-command-descriptions

- Source: native-reference-match

## Summary

System Prompt: write-command-descriptions - Source: inline Summary Rules for generating clear active-voice descriptions of shell commands.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
# System Prompt: write-command-descriptions

- Source: inline

## Summary

Rules for generating clear active-voice descriptions of shell commands.

# Raw Prompt Text
Clear, concise description of what this command does in active voice. Never use words like "complex" or "risk" in the description - just describe what it does.

For simple commands (git, npm, standard CLI tools), keep it brief (${EXPR_1}-${EXPR_2} words):
- ls → "List files in current directory"
- git status → "Show working tree status"
- npm install → "Install package dependencies"

For commands that are harder to parse at a glance (piped commands, obscure flags, etc.), add enough context to clarify what it does:
- find . -name "*.tmp" -exec rm {} \; → "Find and delete all .tmp files recursively"
- git reset --hard origin${EXPR_3} → "Discard all local changes and match remote main"
- curl -s url | jq '.data[]' → "Fetch JSON from URL and extract data array elements"
