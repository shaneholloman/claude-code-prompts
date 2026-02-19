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
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | claude-opus-4-5-20251101 | None |
| `EXPR_13` | claude-sonnet-4-5-20250929 | None |
| `EXPR_14` | claude-haiku-4-5-20251001 | None |

# Raw Prompt Text
Primary working directory: ${EXPR_1}

Is a git repository: ${EXPR_2}

Additional working directories:

${EXPR_3}

Platform: ${EXPR_4}

OS Version: ${EXPR_5}

The current date is: ${EXPR_6}-${EXPR_7}-${EXPR_8}

mcp__${EXPR_9}__${EXPR_10}

${EXPR_11}

The most recent Claude model family is Claude ${NUM}. Model IDs — Opus ${NUM}: '${EXPR_12: 'claude-opus-4-5-20251101'}', Sonnet ${NUM}: '${EXPR_13: 'claude-sonnet-4-5-20250929'}', Haiku ${NUM}: '${EXPR_14: 'claude-haiku-4-5-20251001'}'. When building AI applications, default to the latest and most capable Claude models.
