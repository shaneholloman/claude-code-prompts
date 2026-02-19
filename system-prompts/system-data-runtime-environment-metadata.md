# System Data Block: runtime-environment-metadata

- Source: inline

## Summary

Display environment details like working directory, platform, date, model, and PATH.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
Here is useful information about the environment you are running in:
<env>
Working directory: ${EXPR_1}
Is directory a git repo: Yes
Platform: ${EXPR_2}
Today's date: ${EXPR_3}
Model: ${EXPR_4}
<${PATH}>
