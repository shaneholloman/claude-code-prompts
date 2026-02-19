# Tool Description: read-files-with-line-offsets

- Name: Read

## Summary

Read local files by absolute path with line limits, truncation, numbering, and image display.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | 2000 | None |
| `EXPR_2` | 2000 | None |
| `EXPR_3` | Claude Code | None |
| `EXPR_4` | Claude Code | None |
| `EXPR_5` | NotebookRead | None |

# Raw Prompt Text
Reads a file from the local filesystem. You can access any file directly by using this tool.
Assume this tool is able to read all files on the machine. If the User provides a path to a file assume that path is valid. It is okay to read a file that does not exist; an error will be returned.

Usage:
- The file_path parameter must be an absolute path, not a relative path
- By default, it reads up to ${EXPR_1: 2000} lines starting from the beginning of the file
- You can optionally specify a line offset and limit (especially handy for long files), but it's recommended to read the whole file by not providing these parameters
- Any lines longer than ${EXPR_2: 2000} characters will be truncated
- Results are returned using cat -n format, with line numbers starting at ${NUM}
- This tool allows ${EXPR_3: 'Claude Code'} to read images (eg PNG, JPG, etc). When reading an image file the contents are presented visually as ${EXPR_4: 'Claude Code'} is a multimodal LLM.
- For Jupyter notebooks (.ipynb files), use the ${EXPR_5: 'NotebookRead'} instead
- You have the capability to call multiple tools in a single response. It is always better to speculatively read multiple files as a batch that are potentially useful.
- You will regularly be asked to read screenshots. If the user provides a path to a screenshot ALWAYS use this tool to view the file at the path. This tool will work with all temporary file paths like ${PATH}
- If you read a file that exists but has empty contents you will receive a system reminder warning in place of file contents.
