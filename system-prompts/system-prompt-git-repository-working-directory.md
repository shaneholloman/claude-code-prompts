# System Prompt: git-repository-working-directory

- Source: inline

## Summary

Instructions for using a git worktree.

# Raw Prompt Text
Primary working directory: global

This is a git worktree — an isolated copy of the repository. Run all commands from this directory. Do NOT `cd` to the original repository root.

Is a git repository: ${EXPR_1}

Additional working directories:

${EXPR_2}

Platform: ${EXPR_3}

Shell: ${EXPR_4} (use Unix shell syntax, not Windows — e.g., ${PATH} not NUL, forward slashes in paths)

OS Version: ${EXPR_5}

${EXPR_6}

${EXPR_7}

The most recent Claude model family is Claude ${NUM}${PATH} Model IDs — Opus ${NUM}: '${EXPR_8}', Sonnet ${NUM}: '${EXPR_9}', Haiku ${NUM}: '${EXPR_10}'. When building AI applications, default to the latest and most capable Claude models.
