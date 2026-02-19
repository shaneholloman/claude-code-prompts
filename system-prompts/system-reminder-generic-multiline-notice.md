# System Reminder: generic-multiline-notice

- Source: inline

## Summary

Renders a nine-line message composed entirely from provided placeholder text segments.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | resolved list (4 items) | None |
| `EXPR_4` | None | None |
| `EXPR_5` | Read | None |
| `EXPR_6` | Glob | None |
| `EXPR_7` | Grep | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |

# Raw Prompt Text
${EXPR_1}

${EXPR_2}

${EXPR_3}

${EXPR_4}

${EXPR_5: 'Read'}

${EXPR_6: 'Glob'}

${EXPR_7: 'Grep'}

${EXPR_8}

${EXPR_9}
