# System Data Block: conversation-title-with-context

- Source: inline

## Summary

Requests a short title for a conversation while including additional context blocks.

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
| `EXPR_11` | Task | None |
| `EXPR_12` | Bash | None |
| `EXPR_13` | Glob | None |
| `EXPR_14` | Grep | None |
| `EXPR_15` | ExitPlanMode | None |
| `EXPR_16` | Read | None |
| `EXPR_17` | Edit | None |
| `EXPR_18` | MultiEdit | None |
| `EXPR_19` | Write | None |
| `EXPR_20` | NotebookEdit | None |
| `EXPR_21` | WebFetch | None |
| `EXPR_22` | WebSearch | None |
| `EXPR_23` | BashOutput | None |
| `EXPR_24` | KillShell | None |

# Raw Prompt Text
${EXPR_1}

${EXPR_2}

${EXPR_3}

${EXPR_4}

${EXPR_5}

${EXPR_6}

${EXPR_7}

Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_8} of ${EXPR_9} messages]

${EXPR_10}


Respond with the title for the conversation and nothing else.

@anthropic-ai${PATH}

${EXPR_11: 'Task'}

${EXPR_12: 'Bash'}

${EXPR_13: 'Glob'}

${EXPR_14: 'Grep'}

${EXPR_15: 'ExitPlanMode'}

${EXPR_16: 'Read'}

${EXPR_17: 'Edit'}

${EXPR_18: 'MultiEdit'}

${EXPR_19: 'Write'}

${EXPR_20: 'NotebookEdit'}

${EXPR_21: 'WebFetch'}

${EXPR_22: 'WebSearch'}

${EXPR_23: 'BashOutput'}

${EXPR_24: 'KillShell'}

${EXPR_25}
