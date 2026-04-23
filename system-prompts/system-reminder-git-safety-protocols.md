# System Reminder: git-safety-protocols

- Source: native-reference-match

## Summary

System Reminder: git-safety-protocols - Source: native-reference-match Summary Guidelines for safe git operations.

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
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |
| `EXPR_18` | None | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | None | None |
| `EXPR_22` | None | None |
| `EXPR_23` | None | None |
| `EXPR_24` | None | None |

# Raw Prompt Text
# System Reminder: git-safety-protocols

- Source: native-reference-match

## Summary

Guidelines for safe git operations.

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
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |
| `EXPR_18` | None | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | None | None |
| `EXPR_22` | None | None |
| `EXPR_23` | None | None |
| `EXPR_24` | None | None |

# Raw Prompt Text
# System Reminder: git-safety-protocols

- Source: inline

## Summary

Guidelines for safe git operations.

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
| `EXPR_10` | None | None |

# Raw Prompt Text
${EXPR_1}## Context

- `SAFEUSER`: stable
- `whoami`: ${EXPR_2}
- `git status`: !`git status`
- `git diff HEAD`: !`git diff HEAD`
- `git branch --show-current`: !`git branch --show-current`
- `git diff ${EXPR_3}...HEAD`: !`git diff ${EXPR_4}...HEAD`
- `gh pr view --json number ${EXPR_5}>${EXPR_6} || true`: !`gh pr view --json number ${EXPR_7}>${EXPR_8} || true`

## Git Safety Protocol

- NEVER update the git config
- NEVER run destructive${EXPR_9} git commands (like push --force, hard reset, etc) unless the user explicitly requests them
- NEVER skip hooks (--no-verify, --no-gpg-sign, etc) unless the user explicitly requests it
- NEVER run force push to main${EXPR_10}, warn the user if they request it
- Do not commit files that likely contain secrets (.env, credentials.json, etc)
- Never use git commands with the -i flag (like git rebase -i or git add -i) since they require interactive input which is not supported

## Your task

Analyze all changes that will be included in the pull request, making sure to look at all relevant commits (NOT just the latest commit, but ALL commits that will be included in the pull request from the git diff ${EXPR_11}...HEAD output above).

Based on the above changes:
${EXPR_12}. Create a new branch if on ${EXPR_13} (use SAFEUSER from context above for the branch name prefix, falling back to whoami if SAFEUSER is empty, e.g., `username${EXPR_14}`)
${EXPR_15}. Create a single commit with an appropriate message using heredoc syntax, ending with the attribution text shown in the example below:
```
git commit -m "$(cat <<'EOF'
Commit message here.${EXPR_16}
EOF
)"
```
${EXPR_17}. Push the branch to origin
${EXPR_18}. If a PR already exists for this branch (check the gh pr view output above), update the PR title and body using `gh pr edit` to reflect the current diffglobal. Otherwise, create a pull request using `gh pr create` with heredoc syntax for the body${EXPR_19}.
   - IMPORTANT: Keep PR titles short (under ${EXPR_20} characters). Use the body for details.
```
gh pr create --title "Short, descriptive title" --body "$(cat <<'EOF'
## Summary
<${EXPR_21}-${EXPR_22} bullet points>

## Test plan
[Bulleted markdown checklist of TODOs for testing the pull request...]${EXPR_23}${EXPR_24}
EOF
)"
```

You have the capability to call multiple tools in a single response. You MUST do all of the above in a single message.@anthropic-ai${EXPR_25}

Return the PR URL when you're done, so the user can see it.
