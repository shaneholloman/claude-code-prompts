# System Data Block: background-bash-status-log-3

- Source: inline

## Summary

Structured log template for background Bash commands, statuses, and chained entries.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | Task | None |
| `EXPR_5` | Bash | None |
| `EXPR_6` | Glob | None |
| `EXPR_7` | Grep | None |
| `EXPR_8` | ExitPlanMode | None |
| `EXPR_9` | Read | None |
| `EXPR_10` | Edit | None |
| `EXPR_11` | MultiEdit | None |
| `EXPR_12` | Write | None |
| `EXPR_13` | NotebookEdit | None |
| `EXPR_14` | WebFetch | None |
| `EXPR_15` | WebSearch | None |
| `EXPR_16` | BashOutput | None |
| `EXPR_17` | KillShell | None |
| `EXPR_18` | None | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | Task | None |
| `EXPR_22` | Bash | None |
| `EXPR_23` | Glob | None |
| `EXPR_24` | Grep | None |

# Raw Prompt Text
${EXPR_1}
${EXPR_2}
${EXPR_3}
${EXPR_4: 'Task'}
${EXPR_5: 'Bash'}
${EXPR_6: 'Glob'}
${EXPR_7: 'Grep'}
${EXPR_8: 'ExitPlanMode'}
${EXPR_9: 'Read'}
${EXPR_10: 'Edit'}
${EXPR_11: 'MultiEdit'}
${EXPR_12: 'Write'}
${EXPR_13: 'NotebookEdit'}
${EXPR_14: 'WebFetch'}
${EXPR_15: 'WebSearch'}
${EXPR_16: 'BashOutput'}
${EXPR_17: 'KillShell'}
Background Bash ${EXPR_18}
(command: ${EXPR_19})
(status: ${EXPR_20})
${NUM}

${EXPR_21: 'Task'};${EXPR_22: 'Bash'};${EXPR_23: 'Glob'};${EXPR_24: 'Grep'};${EXPR_25};${EXPR_26};${EXPR_27};${EXPR_28};${EXPR_29};${EXPR_30};${EXPR_31};${EXPR_32};${EXPR_33};${EXPR_34};Background Bash ${EXPR_35};(command: ${EXPR_36});(status: ${EXPR_37});${NUM}
${EXPR_38}
