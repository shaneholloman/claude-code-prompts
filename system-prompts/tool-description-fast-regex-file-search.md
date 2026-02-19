# Tool Description: fast-regex-file-search

- Name: Grep

## Summary

Fast regex content search across files with optional include globs for filtering.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
- Fast content search tool that works with any codebase size
- Searches file contents using regular expressions
- Supports full regex syntax (eg. "log.*Error", "function\s+\w+", etc.)
- Filter files by pattern with the include parameter (eg. "*.js", "*.{ts,tsx}")
- Returns file paths with at least one match sorted by modification time
- Use this tool when you need to find files containing specific patterns${EXPR_1}
- When you are doing an open ended search that may require multiple rounds of globbing and grepping, use the Agent tool instead
