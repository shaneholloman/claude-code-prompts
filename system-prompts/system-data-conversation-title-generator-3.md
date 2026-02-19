# System Data Block: conversation-title-generator-3

- Source: inline

## Summary

Instructs generating a fixed-length title from the last conversation messages.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | Task | None |
| `EXPR_2` | Bash | None |
| `EXPR_3` | Glob | None |
| `EXPR_4` | Grep | None |
| `EXPR_5` | ExitPlanMode | None |
| `EXPR_6` | Read | None |
| `EXPR_7` | Edit | None |
| `EXPR_8` | Write | None |
| `EXPR_9` | NotebookEdit | None |
| `EXPR_10` | WebFetch | None |
| `EXPR_11` | WebSearch | None |
| `EXPR_12` | BashOutput | None |
| `EXPR_13` | KillShell | None |
| `EXPR_14` | SlashCommand | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |
| `EXPR_18` | None | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | None | None |
| `EXPR_22` | None | None |
| `EXPR_23` | None | None |
| `EXPR_24` | None | None |

# Raw Prompt Text
@anthropic-ai${PATH}

${EXPR_1: 'Task'}

${EXPR_2: 'Bash'}

${EXPR_3: 'Glob'}

${EXPR_4: 'Grep'}

${EXPR_5: 'ExitPlanMode'}

${EXPR_6: 'Read'}

${EXPR_7: 'Edit'}

${EXPR_8: 'Write'}

${EXPR_9: 'NotebookEdit'}

${EXPR_10: 'WebFetch'}

${EXPR_11: 'WebSearch'}

${EXPR_12: 'BashOutput'}

${EXPR_13: 'KillShell'}

${EXPR_14: 'SlashCommand'}

${EXPR_15}

${EXPR_16}

${EXPR_17}

${EXPR_18}

${EXPR_19}

${EXPR_20}

${EXPR_21}

Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_22} of ${EXPR_23} messages]

${EXPR_24}


Respond with the title for the conversation and nothing else.
