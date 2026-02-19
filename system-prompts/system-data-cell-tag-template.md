# System Data Block: cell-tag-template


## Summary

XML-like cell tag with multiple dynamic attributes and nested path element.

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
| `EXPR_14` | TodoRead | None |
| `EXPR_15` | TodoWrite | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |

# Raw Prompt Text
<cell ${EXPR_1}>${EXPR_2: 'Task'}${EXPR_3: 'Bash'}${EXPR_4: 'Batch'}${EXPR_5: 'Glob'}${EXPR_6: 'Grep'}${EXPR_7: 'LS'}${EXPR_8: 'Read'}${EXPR_9: 'Edit'}${EXPR_10: 'Write'}${EXPR_11: 'NotebookRead'}${EXPR_12: 'NotebookEdit'}${EXPR_13: 'WebFetch'}${EXPR_14: 'TodoRead'}${EXPR_15: 'TodoWrite'}${EXPR_16}<${PATH} ${EXPR_17}>
