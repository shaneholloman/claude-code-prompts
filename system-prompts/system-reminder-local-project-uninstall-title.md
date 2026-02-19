# System Reminder: local-project-uninstall-title

- Source: inline

## Summary

Create a NUM-NUM word conversation title from the last EXPR_1 of EXPR_2 messages.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
user

project

local

uninstall

-g

--force

Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_1} of ${EXPR_2} messages]

${EXPR_3}


Respond with the title for the conversation and nothing else.
