# System Reminder: invalid-option

- Source: inline

## Summary

Warn that an agent file model value is invalid and list allowed model options.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
Agent file ${EXPR_1} has invalid model '${EXPR_2}'. Valid options: sonnet, opus, haiku, best, sonnet[1m], opus[1m], opusplan, inherit
