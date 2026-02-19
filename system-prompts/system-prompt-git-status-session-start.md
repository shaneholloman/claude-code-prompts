# System Prompt: git-status-session-start

- Source: inline

## Summary

Record starting git status snapshot, including current branch and recent commits.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
This is the git status at the start of the conversation. Note that this status is a snapshot in time, and will not update during the conversation.
Current branch: ${EXPR_1}

Main branch (you will usually use this for PRs): ${EXPR_2}

Status:
mcp__${EXPR_3}__

Recent commits:
${EXPR_4}
