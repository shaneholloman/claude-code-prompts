# System Prompt: stdio-arguments-stream-handling

- Source: inline

## Summary

Conditional handling of stdio arguments and stream-json option changes.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | false | None |
| `EXPR_4` | true | None |
| `EXPR_5` | stream-json | None |
| `EXPR_6` | false | None |
| `EXPR_7` | true | None |
| `EXPR_8` | stream-json | None |
| `EXPR_9` | None | None |
| `EXPR_10` | false | None |
| `EXPR_11` | true | None |
| `EXPR_12` | stream-json | None |
| `EXPR_13` | stream-json | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |

# Raw Prompt Text
${EXPR_1} == 'number' ? ( (Agent changes:
${EXPR_2} = stdio === undefined || ${EXPR_3: false}

ARGUMENTS: ${EXPR_4: true} stream-json= stdio) ? ${NUM} ${EXPR_5: 'stream-json'}= ${EXPR_6: false}

ARGUMENTS: ${EXPR_7: true} : ${NUM} ${EXPR_8: 'stream-json'} stdio ) : ( (Agent changes:
${EXPR_9} = ${EXPR_10: false}

ARGUMENTS: ${EXPR_11: true} === true) ? ${NUM} ${EXPR_12: 'stream-json'}= stdio : ${NUM} ${EXPR_13: 'stream-json'} stdio ) || ${NUM} !== ${NUM}) { var op${EXPR_14} = Agent changes:
${EXPR_15} ? 'stream-json' : 'stream-json=';
