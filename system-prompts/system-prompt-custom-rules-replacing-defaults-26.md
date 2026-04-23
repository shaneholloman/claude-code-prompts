# System Data Block: custom-defaults-rules-replacing-2

- Source: inline

## Summary

Defines custom rules to replace default settings.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |

# Raw Prompt Text
((${NUM}|[${NUM}-${NUM}][\d_]*|\d[\d_]*|[\d_]+?\d)(\.\d*|## allow (custom rules replacing defaults)
Custom:
${EXPR_1}

Defaults being replaced:
${EXPR_2}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_3}

Defaults being replaced:
${EXPR_4}

## environment (custom rules replacing defaults)
Custom:
${EXPR_5}

Defaults being replaced:
${EXPR_6}

)|\d+\.(${NUM}|[${NUM}-${NUM}][\d_]*|\d[\d_]*|[\d_]+?\d)|\.(${NUM}|[${NUM}-${NUM}][\d_]*)## allow (custom rules replacing defaults)
Custom:
${EXPR_7}

Defaults being replaced:
${EXPR_8}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_9}

Defaults being replaced:
${EXPR_10}

## environment (custom rules replacing defaults)
Custom:
${EXPR_11}

Defaults being replaced:
${EXPR_12}

?)
