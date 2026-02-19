# System Prompt: shell-cwd-reset-logic

- Source: inline

## Summary

Set and validate shell cwd reset flags using conditional checks and defaults.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | true | None |
| `EXPR_2` | None | None |
| `EXPR_3` | true | None |
| `EXPR_4` | None | None |
| `EXPR_5` | true | None |
| `EXPR_6` | None | None |
| `EXPR_7` | true | None |
| `EXPR_8` | None | None |
| `EXPR_9` | true | None |
| `EXPR_10` | None | None |
| `EXPR_11` | true | None |
| `EXPR_12` | None | None |

# Raw Prompt Text
var ${EXPR_1: true}
Shell cwd was reset to ${EXPR_2}; if (${EXPR_3: true}_${EXPR_4} === false || ${EXPR_5: true}_${EXPR_6} === undefined) ${EXPR_7: true}
Shell cwd was reset to ${EXPR_8} = true; else if (typeof ${EXPR_9: true}_${EXPR_10} != 'boolean') ${EXPR_11: true}
Shell cwd was reset to ${EXPR_12} = false; else {
