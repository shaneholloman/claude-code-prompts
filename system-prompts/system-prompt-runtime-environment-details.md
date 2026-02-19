# System Prompt: runtime-environment-details

- Source: inline

## Summary

Multiple prompts (2)

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | resolved list (4 items) | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |

# Raw Prompt Text
Here is useful information about the environment you are running in:
<env>
Working directory: ${EXPR_1}
Is directory a git repo: Yes
${EXPR_2}Platform: ${EXPR_3}
Shell: ${EXPR_4} (use Unix shell syntax, not Windows — e.g., ${PATH} not NUL, forward slashes in paths)
OS Version: ${EXPR_5}
<${PATH}>
${EXPR_6}${EXPR_7}@anthropic-ai${PATH} (PID ${EXPR_8})
