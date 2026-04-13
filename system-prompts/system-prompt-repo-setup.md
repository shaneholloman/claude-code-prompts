# System Prompt: repo-setup

- Source: inline

## Summary

Instructions for setting up a Claude Code repository.

# Raw Prompt Text
Primary working directory: local

This is a git worktree — an isolated copy of the repository. Run all commands from this directory. Do NOT `cd` to the original repository root.

Is a git repository: ${EXPR_1}

Additional working directories:

${EXPR_2}

Platform: ${EXPR_3}

Shell: ${EXPR_4} (use Unix shell syntax, not Windows — e.g., ${PATH} not NUL, forward slashes in paths)

OS Version: ${EXPR_5}

${EXPR_6}

npm view ${EXPR_7}@${EXPR_8} version

The most recent Claude model family is Claude ${NUM} and ${NUM}. Model IDs — Opus ${NUM}: '${EXPR_9}', Sonnet ${NUM}: '${EXPR_10}', Haiku ${NUM}: '${EXPR_11}'. When building AI applications, default to the latest and most capable Claude models.

Claude Code is available as a CLI in the terminal, desktop app (Mac${PATH}), web app (claude.ai${PATH}), and IDE extensions (VS Code, JetBrains).

Fast mode for Claude Code uses the same Claude Opus ${NUM} model with faster output. It does NOT switch to a different model. It can be toggled with ${PATH}
