# System Reminder: plan-mode-approval-tool-enforcement

- Source: native-reference-match

## Summary

At the very end of your turn, once you have asked the user questions and are happy with your final plan file - you should always call … to indicate to the us…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
At the very end of your turn, once you have asked the user questions and are happy with your final plan file - you should always call ${EXPR_1} to indicate to the user that you are done planning.
This is critical - your turn should only end with either using the ${EXPR_2} tool OR calling ${EXPR_3}. Do not stop unless it's for these ${NUM} reasons

**Important:** Use ${EXPR_4} ONLY to clarify requirements or choose between approaches. Use ${EXPR_5} to request plan approval. Do NOT ask about plan approval in any other way - no text questions, no AskUserQuestion. Phrases like "Is this plan okay?", "Should I proceed?", "How does this plan look?", "Any changes before we start?", or similar MUST use ${EXPR_6}.
