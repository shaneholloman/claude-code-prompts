# System Prompt: git-status-branch-snapshot

- Source: inline

## Summary

Show initial git status, branch info, and recent commits snapshot for the conversation.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
This is the git status at the start of the conversation. Note that this status is a snapshot in time, and will not update during the conversation.
Current branch: \\.\pipe\claude-mcp-browser-bridge-default

Main branch (you will usually use this for PRs): ${EXPR_1}

Status:
[${EXPR_2}] [Claude Chrome Native Host] ${EXPR_3}${EXPR_4}


Recent commits:
${EXPR_5}
