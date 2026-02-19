# System Prompt: git-status-at-start

- Source: inline

## Summary

Captures initial git snapshot: current branch, main branch, clean status, recent commits.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
This is the git status at the start of the conversation. Note that this status is a snapshot in time, and will not update during the conversation.
Current branch: ${EXPR_1}

Main branch (you will usually use this for PRs): ${EXPR_2}

Status:
(clean)

Recent commits:
global
