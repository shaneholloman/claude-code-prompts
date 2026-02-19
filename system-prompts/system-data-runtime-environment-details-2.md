# System Data Block: runtime-environment-details-2

- Source: inline

## Summary

Reports runtime environment details including working directory, platform, OS version, date, and PATH.

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

# Raw Prompt Text
Here is useful information about the environment you are running in:
<env>
Working directory: ${EXPR_1}
Is directory a git repo: Yes
stdio${EXPR_2}Platform: ${EXPR_3}
OS Version: ${EXPR_4}
Today's date: ${EXPR_5}-${EXPR_6}-${EXPR_7}
<${PATH}>
${EXPR_8}local
