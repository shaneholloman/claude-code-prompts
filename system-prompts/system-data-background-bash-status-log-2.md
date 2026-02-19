# System Data Block: background-bash-status-log-2

- Source: inline

## Summary

System-data template emitting one or two background bash command and status blocks.

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
| `EXPR_8` | LS | None |
| `EXPR_9` | ExitPlanMode | None |
| `EXPR_10` | Read | None |
| `EXPR_11` | Edit | None |
| `EXPR_12` | MultiEdit | None |
| `EXPR_13` | Write | None |
| `EXPR_14` | NotebookEdit | None |
| `EXPR_15` | WebFetch | None |
| `EXPR_16` | WebSearch | None |
| `EXPR_17` | BashOutput | None |
| `EXPR_18` | KillBash | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | None | None |
| `EXPR_22` | Task | None |
| `EXPR_23` | Bash | None |
| `EXPR_24` | Glob | None |

# Raw Prompt Text
${EXPR_1}
${EXPR_2}
${EXPR_3}
${EXPR_4: 'Task'}
${EXPR_5: 'Bash'}
${EXPR_6: 'Glob'}
${EXPR_7: 'Grep'}
${EXPR_8: 'LS'}
${EXPR_9: 'ExitPlanMode'}
${EXPR_10: 'Read'}
${EXPR_11: 'Edit'}
${EXPR_12: 'MultiEdit'}
${EXPR_13: 'Write'}
${EXPR_14: 'NotebookEdit'}
${EXPR_15: 'WebFetch'}
${EXPR_16: 'WebSearch'}
${EXPR_17: 'BashOutput'}
${EXPR_18: 'KillBash'}
Background Bash ${EXPR_19}
(command: ${EXPR_20})
(status: ${EXPR_21})
${NUM}

${EXPR_22: 'Task'};${EXPR_23: 'Bash'};${EXPR_24: 'Glob'};${EXPR_25};${EXPR_26};${EXPR_27};${EXPR_28};${EXPR_29};${EXPR_30};${EXPR_31};${EXPR_32};${EXPR_33};${EXPR_34};${EXPR_35};${EXPR_36};Background Bash ${EXPR_37};(command: ${EXPR_38});(status: ${EXPR_39});${NUM}
${EXPR_40}
