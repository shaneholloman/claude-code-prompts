# Tool Description: filesystem-file-reader

- Name: View

## Summary

Read a local file by absolute path with line limits, truncation, and image support.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | 2000 | None |
| `EXPR_2` | 2000 | None |
| `EXPR_3` | Claude Code | None |
| `EXPR_4` | Claude Code | None |
| `EXPR_5` | ReadNotebook | None |

# Raw Prompt Text
Reads a file from the local filesystem. You can access any file directly by using this tool.
Assume this tool is able to read all files on the machine. If the User provides a path to a file assume that path is valid. It is okay to read a file that does not exist; an error will be returned.

Usage:
- The file_path parameter must be an absolute path, not a relative path
- By default, it reads up to ${EXPR_1: 2000} lines starting from the beginning of the file
- You can optionally specify a line offset and limit (especially handy for long files), but it's recommended to read the whole file by not providing these parameters
- Any lines longer than ${EXPR_2: 2000} characters will be truncated
- Results are returned using cat -n format, with line numbers starting at ${NUM}
- This tool allows ${EXPR_3: 'Claude Code'} to VIEW images (eg PNG, JPG, etc). When reading an image file the contents are presented visually as ${EXPR_4: 'Claude Code'} is a multimodal LLM.
For Jupyter notebooks (.ipynb files), use the ${EXPR_5: 'ReadNotebook'} instead
