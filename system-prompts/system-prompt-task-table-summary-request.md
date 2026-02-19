# System Prompt: task-table-summary-request

- Source: inline

## Summary

Summarize coding conversation with tasks, files, issues fixed, and current status under limit.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
| ${URL} | ${URL} |
| fix lint errors | fix typecheck errors | how does ${EXPR_1} work? | refactor ${EXPR_2} | how do I log an error? | edit ${EXPR_3} to... | write a test for ${EXPR_4} | create a util logging.py that... |
Summarize this coding conversation in under ${NUM} characters.
Capture the main task, key files, problems addressed, and current status.
