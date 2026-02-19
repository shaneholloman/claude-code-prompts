# System Data Block: workspace-and-info

- Source: inline

## Summary

Describe working directories, environment details, and recommended latest Claude model ID strings.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | resolved list (4 items) | None |
| `EXPR_8` | claude-opus-4-6 | None |
| `EXPR_9` | claude-sonnet-4-6 | None |
| `EXPR_10` | claude-haiku-4-5-20251001 | None |

# Raw Prompt Text
Primary working directory: ${EXPR_1}

Is a git repository: ${EXPR_2}

Additional working directories:

${EXPR_3}

Platform: ${EXPR_4}

Shell: ${EXPR_5} (use Unix shell syntax, not Windows — e.g., ${PATH} not NUL, forward slashes in paths)

OS Version: ${EXPR_6}

${EXPR_7}

global

The most recent Claude model family is Claude ${NUM}${PATH} Model IDs — Opus ${NUM}: '${EXPR_8: 'claude-opus-4-6'}', Sonnet ${NUM}: '${EXPR_9: 'claude-sonnet-4-6'}', Haiku ${NUM}: '${EXPR_10: 'claude-haiku-4-5-20251001'}'. When building AI applications, default to the latest and most capable Claude models.
