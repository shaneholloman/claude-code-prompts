# System Prompt: stream-json-flag-argument-parsing

- Source: inline

## Summary

Conditional logic for selecting stream-json flag based on argument types.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | true | None |
| `EXPR_5` | stream-json | None |
| `EXPR_6` | None | None |
| `EXPR_7` | true | None |
| `EXPR_8` | stream-json | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | true | None |
| `EXPR_12` | stream-json | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |

# Raw Prompt Text
${EXPR_1} == 'number' ? ( (${EXPR_2}${NUM} = ${EXPR_3} === undefined || ${EXPR_4: true}

ARGUMENTS: ${EXPR_5: 'stream-json'} stream-json= ${EXPR_6}) ? ${NUM} stream-json= ${EXPR_7: true}

ARGUMENTS: ${EXPR_8: 'stream-json'} : ${NUM} stream-json ${EXPR_9} ) : ( (${EXPR_10}${NUM} = ${EXPR_11: true}

ARGUMENTS: ${EXPR_12: 'stream-json'} === true) ? ${NUM} stream-json= ${EXPR_13} : ${NUM} stream-json ${EXPR_14} ) || ${NUM} !== ${NUM}) { var op${EXPR_15} = ${EXPR_16}${NUM} ? 'stream-json' : 'stream-json=';
