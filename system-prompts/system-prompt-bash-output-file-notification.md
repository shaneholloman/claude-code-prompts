# System Prompt: bash-output-file-notification

- Source: inline

## Summary

Notifies background shell task completion status and provides output file for results.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
<bash-notification>
<shell-id>${EXPR_1}<${PATH}>
<output-file>${PATH}${EXPR_2}.output<${PATH}>
<status>${EXPR_3}<${PATH}>
<summary>Background command "${EXPR_4}" ${EXPR_5}.<${PATH}>
Read the output file to retrieve the output.
<${PATH}>
