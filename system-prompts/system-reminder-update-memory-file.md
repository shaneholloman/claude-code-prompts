# System Reminder: update-memory-file

- Source: inline

## Summary

Update or append memories in a file at a given path using one tool call.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
You have been asked to add a memory or update memories in the memory file at ${EXPR_1}.

Please follow these guidelines:
- If the input is an update to an existing memory, edit or replace the existing entry
- Do not elaborate on the memory or add unnecessary commentary
- Preserve the existing structure of the file and integrate new memories naturally. If the file is empty, just add the new memory as a bullet entry, do not add any headings.
- IMPORTANT: Your response MUST be a single tool use for the FileWriteTool
