# Tool Description: edit-files-string-replace

- Name: Edit

## Summary

Describes a string-replacement file edit tool and references a notebook tool alternative.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | Bash | None |
| `EXPR_2` | Write | None |
| `EXPR_3` | NotebookEdit | None |
| `EXPR_4` | Read | None |
| `EXPR_5` | LS | None |
| `EXPR_6` | Read | None |

# Raw Prompt Text
This is a tool for editing files. For moving or renaming files, you should generally use the ${EXPR_1: 'Bash'} tool with the 'mv' command instead. For larger edits, use the ${EXPR_2: 'Write'} tool to overwrite files. For Jupyter notebooks (.ipynb files), use the ${EXPR_3: 'NotebookEdit'} instead.

Before using this tool:

${NUM}. Use the ${EXPR_4: 'Read'} tool to understand the file's contents and context

${NUM}. Verify the directory path is correct (only applicable when creating new files):
   - Use the ${EXPR_5: 'LS'} tool to verify the parent directory exists and is the correct location

To make a file edit, provide the following:
${NUM}. file_path: The absolute path to the file to modify (must be absolute, not relative)
${NUM}. old_string: The text to replace (must match the file contents exactly, including all whitespace and indentation)
${NUM}. new_string: The edited text to replace the old_string (must be different from old_string)
${NUM}. expected_replacements: The number of replacements you expect to make. Defaults to ${NUM} if not specified.

By default, the tool will replace ONE occurrence of old_string with new_string in the specified file. If you want to replace multiple occurrences, provide the expected_replacements parameter with the exact number of occurrences you expect.

CRITICAL REQUIREMENTS FOR USING THIS TOOL:

${NUM}. UNIQUENESS (when expected_replacements is not specified): The old_string MUST uniquely identify the specific instance you want to change. This means:
   - Include AT LEAST ${NUM}-${NUM} lines of context BEFORE the change point
   - Include AT LEAST ${NUM}-${NUM} lines of context AFTER the change point
   - Include all whitespace, indentation, and surrounding code exactly as it appears in the file

${NUM}. EXPECTED MATCHES: If you want to replace multiple instances:
   - Use the expected_replacements parameter with the exact number of occurrences you expect to replace
   - This will replace ALL occurrences of the old_string with the new_string
   - If the actual number of matches doesn't equal expected_replacements, the edit will fail
   - This is a safety feature to prevent unintended replacements

${NUM}. VERIFICATION: Before using this tool:
   - Check how many instances of the target text exist in the file
   - If multiple instances exist, either:
     a) Gather enough context to uniquely identify each one and make separate calls, OR
     b) Use expected_replacements parameter with the exact count of instances you expect to replace

WARNING:
- The tool will fail if old_string matches multiple locations and expected_replacements isn't specified
- The tool will fail if the number of matches doesn't equal expected_replacements when it's specified
- The tool will fail if old_string doesn't match the file contents exactly (including whitespace)
- The tool will fail if old_string and new_string are the same
- The tool will fail if you did not read the file using the ${EXPR_6: 'Read'} tool first, before using this tool

When making edits:
   - Ensure the edit results in idiomatic, correct code
   - Do not add trailing whitespace to lines (a newline at the end of a file is fine)
   - Do not leave the code in a broken state
   - Always use absolute file paths (starting with /)

If you want to create a new file, use:
   - A new file path, including dir name if needed
   - An empty old_string
   - The new file's contents as new_string
