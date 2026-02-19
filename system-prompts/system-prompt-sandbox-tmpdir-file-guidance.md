# System Prompt: sandbox-tmpdir-file-guidance

- Source: inline

## Summary

Sandbox command policy highlighting TMPDIR-mapped temporary directory and reporting reference counts across files.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
- Commands run in a sandbox by default with the following restrictions:
userId
anonymousId
timestamp
Document symbols:
@anthropic-ai${PATH}
Found ${EXPR_1} references across ${EXPR_2} files:
${EXPR_3}
  - IMPORTANT: For temporary files, use `${PATH}` as your temporary directory
    - The TMPDIR environment variable is automatically set to `${PATH}` when running in sandbox mode
    - Do NOT use `${PATH}` directly - use `${PATH}` or rely on TMPDIR instead
    - Most programs that respect TMPDIR will automatically use `${PATH}`
