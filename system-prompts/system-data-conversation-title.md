# System Data Block: conversation-title

- Source: inline

## Summary

Repeats title-generation directions with appended anthropic-ai path context.

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
| `EXPR_18` | Write | None |
| `EXPR_19` | NotebookEdit | None |
| `EXPR_20` | WebFetch | None |
| `EXPR_21` | WebSearch | None |
| `EXPR_22` | BashOutput | None |
| `EXPR_23` | KillShell | None |
| `EXPR_24` | SlashCommand | None |

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

${EXPR_18: 'Write'}

${EXPR_19: 'NotebookEdit'}

${EXPR_20: 'WebFetch'}

${EXPR_21: 'WebSearch'}

${EXPR_22: 'BashOutput'}

${EXPR_23: 'KillShell'}

${EXPR_24: 'SlashCommand'}
