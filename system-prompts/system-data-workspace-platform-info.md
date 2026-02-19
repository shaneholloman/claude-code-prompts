# System Data Block: workspace-platform-info

- Source: inline

## Summary

Lists workspace paths, git status, platform metadata, current date, MCP info, and latest model IDs.

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
| `EXPR_9` | resolved list (4 items) | None |
| `EXPR_10` | claude-opus-4-6 | None |
| `EXPR_11` | claude-sonnet-4-5-20250929 | None |
| `EXPR_12` | claude-haiku-4-5-20251001 | None |

# Raw Prompt Text
Primary working directory: ${EXPR_1}

Is a git repository: ${EXPR_2}

Additional working directories:

${EXPR_3}

Platform: ${EXPR_4}

OS Version: ${EXPR_5}

The current date is: ${EXPR_6}-${EXPR_7}-${EXPR_8}

${EXPR_9}

global

The most recent Claude model family is Claude ${NUM}${PATH} Model IDs — Opus ${NUM}: '${EXPR_10: 'claude-opus-4-6'}', Sonnet ${NUM}: '${EXPR_11: 'claude-sonnet-4-5-20250929'}', Haiku ${NUM}: '${EXPR_12: 'claude-haiku-4-5-20251001'}'. When building AI applications, default to the latest and most capable Claude models.
