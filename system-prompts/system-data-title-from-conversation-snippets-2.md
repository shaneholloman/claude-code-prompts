# System Data Block: title-from-conversation-snippets-2

- Source: inline

## Summary

Generate a …-… word title from conversation text plus appended snippets.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | Task | None |
| `EXPR_2` | Bash | None |
| `EXPR_3` | Batch | None |
| `EXPR_4` | Glob | None |
| `EXPR_5` | Grep | None |
| `EXPR_6` | LS | None |
| `EXPR_7` | Read | None |
| `EXPR_8` | Edit | None |
| `EXPR_9` | Write | None |
| `EXPR_10` | NotebookRead | None |
| `EXPR_11` | NotebookEdit | None |
| `EXPR_12` | WebFetch | None |
| `EXPR_13` | TodoRead | None |
| `EXPR_14` | TodoWrite | None |
| `EXPR_15` | None | None |

# Raw Prompt Text
${EXPR_1: 'Task'}

${EXPR_2: 'Bash'}

${EXPR_3: 'Batch'}

${EXPR_4: 'Glob'}

${EXPR_5: 'Grep'}

${EXPR_6: 'LS'}

${EXPR_7: 'Read'}

${EXPR_8: 'Edit'}

${EXPR_9: 'Write'}

${EXPR_10: 'NotebookRead'}

${EXPR_11: 'NotebookEdit'}

${EXPR_12: 'WebFetch'}

${EXPR_13: 'TodoRead'}

${EXPR_14: 'TodoWrite'}

Please write a ${NUM}-${NUM} word title the following conversation:

${EXPR_15}


Respond with the title for the conversation and nothing else.
