# Skill: debug-session


## Summary

Guides debugging a reported Claude Code session issue using the session log and settings.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
# Debug Skill

Help the user debug an issue they're encountering in this current Claude Code session.

## Session Debug Log

The debug log for the current session is at: `${EXPR_1}`

${EXPR_2}

For additional context, grep for [ERROR] and [WARN] lines across the full file.

## Issue Description

${EXPR_3}

## Settings

Remember that settings are in:
* user - ${EXPR_4}
* project - ${EXPR_5}
* local - ${EXPR_6}

## Instructions

${NUM}. Review the user's issue description
${NUM}. The last ${NUM} lines show the debug file format. Look for [ERROR] and [WARN] entries, stack traces, and failure patterns across the file
${NUM}. Consider launching the claude-code-guide subagent to understand the relevate Claude Code features
${NUM}. Explain what you found in plain language
${NUM}. Suggest concrete fixes or next steps
