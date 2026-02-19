# System Data Block: title-from-conversation-snippets

- Source: inline

## Summary

Generate a …-… word title from conversation text plus appended snippets.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | Task | None |
| `EXPR_3` | Bash | None |
| `EXPR_4` | Batch | None |
| `EXPR_5` | Glob | None |
| `EXPR_6` | Grep | None |
| `EXPR_7` | LS | None |
| `EXPR_8` | Read | None |
| `EXPR_9` | Edit | None |
| `EXPR_10` | Write | None |
| `EXPR_11` | NotebookRead | None |
| `EXPR_12` | NotebookEdit | None |
| `EXPR_13` | WebFetch | None |

# Raw Prompt Text
Please write a ${NUM}-${NUM} word title the following conversation:

${EXPR_1}


Respond with the title for the conversation and nothing else.

${EXPR_2: 'Task'}

${EXPR_3: 'Bash'}

${EXPR_4: 'Batch'}

${EXPR_5: 'Glob'}

${EXPR_6: 'Grep'}

${EXPR_7: 'LS'}

${EXPR_8: 'Read'}

${EXPR_9: 'Edit'}

${EXPR_10: 'Write'}

${EXPR_11: 'NotebookRead'}

${EXPR_12: 'NotebookEdit'}

${EXPR_13: 'WebFetch'}
