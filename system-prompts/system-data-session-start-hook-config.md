# System Data Block: session-start-hook-config

- Source: inline

## Summary

Session-start-hook wrapper concatenating 15 injected expressions and a trailing PATH tag.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | Task | None |
| `EXPR_2` | Bash | None |
| `EXPR_3` | Glob | None |
| `EXPR_4` | Grep | None |
| `EXPR_5` | LS | None |
| `EXPR_6` | ExitPlanMode | None |
| `EXPR_7` | Read | None |
| `EXPR_8` | Edit | None |
| `EXPR_9` | MultiEdit | None |
| `EXPR_10` | Write | None |
| `EXPR_11` | NotebookEdit | None |
| `EXPR_12` | WebFetch | None |
| `EXPR_13` | WebSearch | None |
| `EXPR_14` | BashOutput | None |
| `EXPR_15` | KillBash | None |

# Raw Prompt Text
<session-start-hook>${EXPR_1: 'Task'}

${EXPR_2: 'Bash'}

${EXPR_3: 'Glob'}

${EXPR_4: 'Grep'}

${EXPR_5: 'LS'}

${EXPR_6: 'ExitPlanMode'}

${EXPR_7: 'Read'}

${EXPR_8: 'Edit'}

${EXPR_9: 'MultiEdit'}

${EXPR_10: 'Write'}

${EXPR_11: 'NotebookEdit'}

${EXPR_12: 'WebFetch'}

${EXPR_13: 'WebSearch'}

${EXPR_14: 'BashOutput'}

${EXPR_15: 'KillBash'}<${PATH}>
