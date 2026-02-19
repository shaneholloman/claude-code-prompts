# Tool Description: edit-file-by-replacing-string

- Name: Edit

## Summary

Edit a file by replacing one unique old string with new text.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | NotebookEditCell | None |

# Raw Prompt Text
This is a tool for editing files. For moving or renaming files, you should generally use the Bash tool with the 'mv' command instead. For larger edits, use the Write tool to overwrite files. For Jupyter notebooks (.ipynb files), use the ${EXPR_1: 'NotebookEditCell'} instead.

Before using this tool:

${NUM}. Use the View tool to understand the file's contents and context

${NUM}. Verify the directory path is correct (only applicable when creating new files):
   - Use the LS tool to verify the parent directory exists and is the correct location

To make a file edit, provide the following:
${NUM}. file_path: The absolute path to the file to modify (must be absolute, not relative)
${NUM}. old_string: The text to replace (must be unique within the file, and must match the file contents exactly, including all whitespace and indentation)
${NUM}. new_string: The edited text to replace the old_string

The tool will replace ONE occurrence of old_string with new_string in the specified file.

CRITICAL REQUIREMENTS FOR USING THIS TOOL:

${NUM}. UNIQUENESS: The old_string MUST uniquely identify the specific instance you want to change. This means:
   - Include AT LEAST ${NUM}-${NUM} lines of context BEFORE the change point
   - Include AT LEAST ${NUM}-${NUM} lines of context AFTER the change point
   - Include all whitespace, indentation, and surrounding code exactly as it appears in the file

${NUM}. SINGLE INSTANCE: This tool can only change ONE instance at a time. If you need to change multiple instances:
   - Make separate calls to this tool for each instance
   - Each call must uniquely identify its specific instance using extensive context

${NUM}. VERIFICATION: Before using this tool:
   - Check how many instances of the target text exist in the file
   - If multiple instances exist, gather enough context to uniquely identify each one
   - Plan separate tool calls for each instance

WARNING: If you do not follow these requirements:
   - The tool will fail if old_string matches multiple locations
   - The tool will fail if old_string doesn't match exactly (including whitespace)
   - You may change the wrong instance if you don't include enough context

When making edits:
   - Ensure the edit results in idiomatic, correct code
   - Do not leave the code in a broken state
   - Always use absolute file paths (starting with /)

If you want to create a new file, use:
   - A new file path, including dir name if needed
   - An empty old_string
   - The new file's contents as new_string

Remember: when making multiple file edits in a row to the same file, you should prefer to send all edits in a single message with multiple calls to this tool, rather than multiple messages with a single call each.
