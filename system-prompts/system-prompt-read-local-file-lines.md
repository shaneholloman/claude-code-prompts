# System Prompt: read-local-file-lines

- Source: inline

## Summary

Reads absolute-path files with optional offset/limit, truncation, numbered lines; use EXPR_1 for notebooks.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | ReadNotebook | None |

# Raw Prompt Text
Reads a file from the local filesystem.

Usage:
- The file_path parameter must be an absolute path, not a relative path
- By default, it reads up to ${NUM} lines starting from the beginning of the file
- You can optionally specify a line offset and limit (especially handy for long files), but it's recommended to read the whole file by not providing these parameters
- Any lines longer than ${NUM} characters will be truncated
- Results are returned using cat -n format, with line numbers starting at ${NUM}
- For image files, the tool will display the image for you
For Jupyter notebooks (.ipynb files), use the ${EXPR_1: 'ReadNotebook'} instead
