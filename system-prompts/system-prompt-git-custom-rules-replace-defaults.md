# System Prompt: git-custom-rules-replace-defaults

- Source: inline

# Raw Prompt Text
## allow (custom rules replacing defaults)
Custom:
${EXPR_1}

Defaults being replaced:
${EXPR_2}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_3}

Defaults being replaced:
${EXPR_4}

## environment (custom rules replacing defaults)
Custom:
${EXPR_5}

Defaults being replaced:
${EXPR_6}

## Context

- `SAFEUSER`: stable
- `whoami`: npm view ${EXPR_7}@${EXPR_8} version
- `git status`: !`git status`
- `git diff HEAD`: !`git diff HEAD`
- `git branch --show-current`: !`git branch --show-current`
- `git diff ${EXPR_9}...HEAD`: !`git diff ${EXPR_10}...HEAD`
- `gh pr view --json number ${NUM}>${PATH} || true`: !`gh pr view --json number ${NUM}>${PATH} || true`

## Git Safety Protocol

- NEVER update the git config
- NEVER run destructive${PATH} git commands (like push --force, hard reset, etc) unless the user explicitly requests them
- NEVER skip hooks (--no-verify, --no-gpg-sign, etc) unless the user explicitly requests it
- NEVER run force push to main${PATH}, warn the user if they request it
- Do not commit files that likely contain secrets (.env, credentials.json, etc)
- Never use git commands with the -i flag (like git rebase -i or git add -i) since they require interactive input which is not supported

## Your task

Analyze all changes that will be included in the pull request, making sure to look at all relevant commits (NOT just the latest commit, but ALL commits that will be included in the pull request from the git diff ${EXPR_11}...HEAD output above).

Based on the above changes:
${NUM}. Create a new branch if on ${EXPR_12} (use SAFEUSER from context above for the branch name prefix, falling back to whoami if SAFEUSER is empty, e.g., `username${PATH}`)
${NUM}. Create a single commit with an appropriate message using heredoc syntax, ending with the attribution text shown in the example below:
```
git commit -m "$(cat <<'EOF'
Commit message here.

${EXPR_13}
EOF
)"
```
${NUM}. Push the branch to origin
${NUM}. If a PR already exists for this branch (check the gh pr view output above), update the PR title and body using `gh pr edit` to reflect the current diffglobal. Otherwise, create a pull request using `gh pr create` with heredoc syntax for the body${EXPR_14}.
   - IMPORTANT: Keep PR titles short (under ${NUM} characters). Use the body for details.
```
gh pr create --title "Short, descriptive title" --body "$(cat <<'EOF'
## Summary

Multiple prompts (2)

## Test plan
[Bulleted markdown checklist of TODOs for testing the pull request...]${EXPR_15}

${EXPR_16}
EOF
)"
```

You have the capability to call multiple tools in a single response. You MUST do all of the above in a single message.@anthropic-ai${PATH}

Return the PR URL when you're done, so the user can see it.
