# System Data Block: uninstall-force-title-generation

- Source: inline

## Summary

Create a brief conversation title from recent messages containing uninstall and force flags.

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
| `EXPR_8` | MultiEdit | None |
| `EXPR_9` | Write | None |
| `EXPR_10` | NotebookEdit | None |
| `EXPR_11` | WebFetch | None |
| `EXPR_12` | WebSearch | None |
| `EXPR_13` | BashOutput | None |
| `EXPR_14` | KillShell | None |
| `EXPR_15` | SlashCommand | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |
| `EXPR_18` | None | None |

# Raw Prompt Text
uninstall

-g

--force

${EXPR_1: 'Task'}

${EXPR_2: 'Bash'}

${EXPR_3: 'Glob'}

${EXPR_4: 'Grep'}

${EXPR_5: 'ExitPlanMode'}

${EXPR_6: 'Read'}

${EXPR_7: 'Edit'}

${EXPR_8: 'MultiEdit'}

${EXPR_9: 'Write'}

${EXPR_10: 'NotebookEdit'}

${EXPR_11: 'WebFetch'}

${EXPR_12: 'WebSearch'}

${EXPR_13: 'BashOutput'}

${EXPR_14: 'KillShell'}

${EXPR_15: 'SlashCommand'}

Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_16} of ${EXPR_17} messages]

${EXPR_18}


Respond with the title for the conversation and nothing else.
