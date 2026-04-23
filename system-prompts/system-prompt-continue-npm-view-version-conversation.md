# System Prompt: continue-npm-view-version-conversation

- Source: inline

## Summary

Resume the conversation without interruptions.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | @anthropic-ai/claude-code | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
npm view ${EXPR_1: '@anthropic-ai/claude-code'}@${EXPR_2} version
Continue the conversation from where it left off without asking the user any further questions. Resume directly — do not acknowledge the summary, do not recap what was happening, do not preface with "I'll continue" or similar. Pick up the last task as if the break never happened.
