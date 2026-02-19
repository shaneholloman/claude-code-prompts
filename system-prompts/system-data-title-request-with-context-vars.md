# System Data Block: title-request-with-context-vars

- Source: inline

## Summary

Requests a word-limited conversation title and appends additional context variables.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | Task | None |
| `EXPR_6` | Bash | None |
| `EXPR_7` | Glob | None |
| `EXPR_8` | Grep | None |
| `EXPR_9` | ExitPlanMode | None |
| `EXPR_10` | Read | None |
| `EXPR_11` | Edit | None |
| `EXPR_12` | MultiEdit | None |
| `EXPR_13` | Write | None |
| `EXPR_14` | NotebookEdit | None |
| `EXPR_15` | WebFetch | None |
| `EXPR_16` | WebSearch | None |
| `EXPR_17` | BashOutput | None |
| `EXPR_18` | KillShell | None |
| `EXPR_19` | SlashCommand | None |

# Raw Prompt Text
${EXPR_1}

Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_2} of ${EXPR_3} messages]

${EXPR_4}


Respond with the title for the conversation and nothing else.

@anthropic-ai${PATH}

${EXPR_5: 'Task'}

${EXPR_6: 'Bash'}

${EXPR_7: 'Glob'}

${EXPR_8: 'Grep'}

${EXPR_9: 'ExitPlanMode'}

${EXPR_10: 'Read'}

${EXPR_11: 'Edit'}

${EXPR_12: 'MultiEdit'}

${EXPR_13: 'Write'}

${EXPR_14: 'NotebookEdit'}

${EXPR_15: 'WebFetch'}

${EXPR_16: 'WebSearch'}

${EXPR_17: 'BashOutput'}

${EXPR_18: 'KillShell'}

${EXPR_19: 'SlashCommand'}
