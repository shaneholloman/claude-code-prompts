# System Prompt: coding-tasks-and-title

- Source: inline

## Summary

Aggregates code maintenance prompts and generates a concise conversation title from recent messages.

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

# Raw Prompt Text
@anthropic-ai${PATH}

${EXPR_1}

@anthropic-ai${PATH}

@anthropic-ai${PATH}

fix lint errors

fix typecheck errors

how does ${EXPR_2} work?

refactor ${EXPR_3}

how do I log an error?

edit ${EXPR_4} to...

write a test for ${EXPR_5}

create a util logging.py that...

Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_6} of ${EXPR_7} messages]

${EXPR_8}


Respond with the title for the conversation and nothing else.
