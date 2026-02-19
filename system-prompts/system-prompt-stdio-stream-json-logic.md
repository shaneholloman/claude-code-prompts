# System Prompt: stdio-stream-json-logic

- Source: inline

## Summary

Ternary logic updates stdio handling and chooses stream-json flag formatting based on conditions

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | stream-json | None |
| `EXPR_4` | stream-json | None |
| `EXPR_5` | None | None |
| `EXPR_6` | stream-json | None |
| `EXPR_7` | stream-json | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |

# Raw Prompt Text
${EXPR_1} == 'number' ? ( (Agent changes:
${EXPR_2} = stdio === undefined || null stream-json= stdio) ? ${NUM} ${EXPR_3: 'stream-json'}= null : ${NUM} ${EXPR_4: 'stream-json'} stdio ) : ( (Agent changes:
${EXPR_5} = null === true) ? ${NUM} ${EXPR_6: 'stream-json'}= stdio : ${NUM} ${EXPR_7: 'stream-json'} stdio ) || ${NUM} !== ${NUM}) { var op${EXPR_8} = Agent changes:
${EXPR_9} ? 'stream-json' : 'stream-json=';
