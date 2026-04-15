# System Prompt: custom-defaults-rules

- Source: inline

## Summary

Custom rules replace default settings in the model.

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
| `EXPR_13` | @anthropic-ai/claude-code | None |
| `EXPR_14` | None | None |
| `EXPR_15` | claude-opus-4-6 | None |
| `EXPR_16` | claude-sonnet-4-6 | None |
| `EXPR_17` | claude-haiku-4-5-20251001 | None |

# Raw Prompt Text
Primary working directory: ## allow (custom rules replacing defaults)
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



This is a git worktree — an isolated copy of the repository. Run all commands from this directory. Do NOT `cd` to the original repository root.

Is a git repository: ${EXPR_7}

Additional working directories:

${EXPR_8}

Platform: ${EXPR_9}

Shell: ${EXPR_10} (use Unix shell syntax, not Windows — e.g., ${PATH} not NUL, forward slashes in paths)

OS Version: ${EXPR_11}

${EXPR_12}

npm view ${EXPR_13: '@anthropic-ai/claude-code'}@${EXPR_14} version

The most recent Claude model family is Claude ${NUM} and ${NUM}. Model IDs — Opus ${NUM}: '${EXPR_15: 'claude-opus-4-6'}', Sonnet ${NUM}: '${EXPR_16: 'claude-sonnet-4-6'}', Haiku ${NUM}: '${EXPR_17: 'claude-haiku-4-5-20251001'}'. When building AI applications, default to the latest and most capable Claude models.

Claude Code is available as a CLI in the terminal, desktop app (Mac${PATH}), web app (claude.ai${PATH}), and IDE extensions (VS Code, JetBrains).

Fast mode for Claude Code uses the same Claude Opus ${NUM} model with faster output. It does NOT switch to a different model. It can be toggled with ${PATH}
