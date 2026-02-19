# System Data Block: failure-report-with-tasks

- Source: inline

## Summary

Reports a failure with issues, then enumerates common follow-up coding fix tasks.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
${EXPR_1} failed due to the following issues:
@anthropic-ai${PATH}
${EXPR_2}
@anthropic-ai${PATH}
@anthropic-ai${PATH}
fix lint errors
fix typecheck errors
how does ${EXPR_3} work?
refactor ${EXPR_4}
how do I log an error?
edit ${EXPR_5} to...
write a test for ${EXPR_6}
create a util logging.py that...
