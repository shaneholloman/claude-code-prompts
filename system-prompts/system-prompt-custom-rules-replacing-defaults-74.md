# System Data Block: environment-info-custom-defaults

- Source: inline

## Summary

Information on custom rules in the environment.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |

# Raw Prompt Text
Here is useful information about the environment you are running in:
<env>
Working directory: ${EXPR_1}
Is directory a git repo: Yes
stablePlatform: ${EXPR_2}
Shell: ${EXPR_3} (use Unix shell syntax, not Windows — e.g., ${PATH} not NUL, forward slashes in paths)
OS Version: ${EXPR_4}
<${PATH}>
${EXPR_5}## allow (custom rules replacing defaults)
Custom:
${EXPR_6}

Defaults being replaced:
${EXPR_7}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_8}

Defaults being replaced:
${EXPR_9}

## environment (custom rules replacing defaults)
Custom:
${EXPR_10}

Defaults being replaced:
${EXPR_11}
