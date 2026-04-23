# System Reminder: use-context-only-when-relevant

- Source: native-reference-match

## Summary

System Reminder: use-context-only-when-relevant - Source: inline Summary Multiple prompts (…) Placeholder Hints (source-backed) | Expression | Hint | Referen…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# System Reminder: use-context-only-when-relevant

- Source: inline

## Summary

Multiple prompts (${NUM})

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
<system-reminder>
As you answer the user's questions, you can use the following context:
${EXPR_1}

      IMPORTANT: this context may or may not be relevant to your tasks. You should not respond to this context unless it is highly relevant to your task.
<${EXPR_2}>
