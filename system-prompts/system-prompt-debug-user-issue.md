# Skill: debug-session


## Summary

Assist in resolving user issues during Claude Code sessions.

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
# Debug Skill

Help the user debug an issue they're encountering in this current Claude Code session.
${EXPR_1}
## Session Debug Log

The debug log for the current session is at: `${EXPR_2}`

${EXPR_3}

For additional context, grep for [ERROR] and [WARN] lines across the full file.

## Issue Description

${EXPR_4}

## Settings

Remember that settings are in:
* user - ${EXPR_5}
* project - ${EXPR_6}
* local - ${EXPR_7}

## Instructions

${NUM}. Review the user's issue description
${NUM}. The last ${NUM} lines show the debug file format. Look for [ERROR] and [WARN] entries, stack traces, and failure patterns across the file
${NUM}. Consider launching the claude-code-guide subagent to understand the relevant Claude Code features
${NUM}. Explain what you found in plain language
${NUM}. Suggest concrete fixes or next steps
