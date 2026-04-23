# System Data Block: git-status-snapshot-conversation

- Source: inline

## Summary

Overview of custom rules and their status.

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

# Raw Prompt Text
This is the git status at the start of the conversation. Note that this status is a snapshot in time, and will not update during the conversation.

Current branch: ${EXPR_1}

Main branch (you will usually use this for PRs): stable

Status:
(clean)

Recent commits:
## allow (custom rules replacing defaults)
Custom:
${EXPR_2}

Defaults being replaced:
${EXPR_3}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_4}

Defaults being replaced:
${EXPR_5}

## environment (custom rules replacing defaults)
Custom:
${EXPR_6}

Defaults being replaced:
${EXPR_7}
