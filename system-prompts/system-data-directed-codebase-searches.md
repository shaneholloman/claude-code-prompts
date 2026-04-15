# System Data Block: directed-codebase-searches

- Source: inline

## Summary

Guidelines for using custom rules in codebase searches.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | Explore | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |

# Raw Prompt Text
For simple, directed codebase searches (e.g. for a specific file${PATH}) use ## allow (custom rules replacing defaults)
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

 directly.

For broader codebase exploration and deep research, use the Agent tool with subagent_type=${EXPR_7: 'Explore'}. This is slower than using ## allow (custom rules replacing defaults)
Custom:
${EXPR_8}

Defaults being replaced:
${EXPR_9}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_10}

Defaults being replaced:
${EXPR_11}

## environment (custom rules replacing defaults)
Custom:
${EXPR_12}

Defaults being replaced:
${EXPR_13}

 directly, so use this only when a simple, directed search proves to be insufficient or when your task will clearly require more than ${NUM} queries.
