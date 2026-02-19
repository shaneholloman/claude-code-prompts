# System Prompt: blocked-directory-change-security

- Source: inline

## Summary

Security error stating cd blocked unless within original working directory child paths.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
ERROR: cd to '<context>${EXPR_1}<${PATH}>

${EXPR_2}' was blocked. For security, Claude Code may only change directories to child directories of the original working directory (${EXPR_3}) for this session.
