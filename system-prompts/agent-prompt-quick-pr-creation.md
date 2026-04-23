# Agent Prompt: quick-pr-creation

- Source: native-reference-match

## Summary

…## Context - `SAFEUSER`: … - `whoami`: … - `git status`: !`git status` - `git diff HEAD`: !`git diff HEAD` - `git branch --show-current`: !`git branch --sho…

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
| `EXPR_9` | None | None |
| `EXPR_10` | create single commit appropriate message | None |

# Raw Prompt Text
${EXPR_1}## Context

- `SAFEUSER`: ${EXPR_2}
- `whoami`: ${EXPR_3}
- `git status`: !`git status`
- `git diff HEAD`: !`git diff HEAD`
- `git branch --show-current`: !`git branch --show-current`
- `git diff ${EXPR_4}...HEAD`: !`git diff ${EXPR_5}...HEAD`
- `gh pr view --json number`: !`${EXPR_6}`

## Git Safety Protocol

- NEVER update the git config
- NEVER run destructive${PATH} git commands (like push --force, hard reset, etc) unless the user explicitly requests them
- NEVER skip hooks (--no-verify, --no-gpg-sign, etc) unless the user explicitly requests it
- NEVER run force push to main${PATH}, warn the user if they request it
- Do not commit files that likely contain secrets (.env, credentials.json, etc)
- Never use git commands with the -i flag (like git rebase -i or git add -i) since they require interactive input which is not supported

## Your task

Analyze all changes that will be included in the pull request, making sure to look at all relevant commits (NOT just the latest commit, but ALL commits that will be included in the pull request from the git diff ${EXPR_7}...HEAD output above).

Based on the above changes:
${NUM}. Create a new branch if on ${EXPR_8} (use SAFEUSER from context above for the branch name prefix, falling back to whoami if SAFEUSER is empty, e.g., `username${PATH}`)
${NUM}. Create a single commit with an appropriate message${EXPR_9}:
${EXPR_10}
