# System Prompt: sandbox-temp-directory-rules

- Source: inline

## Summary

Defines sandbox command restrictions and mandates TMPDIR-backed temporary files location.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
- Commands run in a sandbox by default with the following restrictions:
Usage: ${EXPR_1}
${EXPR_2}
  - IMPORTANT: For temporary files, use `${PATH}` as your temporary directory
    - The TMPDIR environment variable is automatically set to `${PATH}` when running in sandbox mode
    - Do NOT use `${PATH}` directly - use `${PATH}` or rely on TMPDIR instead
    - Most programs that respect TMPDIR will automatically use `${PATH}`
