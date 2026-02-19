# System Prompt: sandbox-tmpdir-and-title

- Source: inline

## Summary

Generate a NUM–NUM word conversation title from recent messages under sandbox TMPDIR constraints.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
- Commands run in a sandbox by default with the following restrictions:
Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_1} of ${EXPR_2} messages]

${EXPR_3}

Respond with the title for the conversation and nothing else.
${EXPR_4}
  - IMPORTANT: For temporary files, use `${PATH}` as your temporary directory
    - The TMPDIR environment variable is automatically set to `${PATH}` when running in sandbox mode
    - Do NOT use `${PATH}` directly - use `${PATH}` or rely on TMPDIR instead
    - Most programs that respect TMPDIR will automatically use `${PATH}`
