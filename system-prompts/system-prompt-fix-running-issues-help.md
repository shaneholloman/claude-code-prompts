# System Prompt: fix-running-issues-help

- Source: inline

## Summary

Assist with reported issues and confirm fixes before execution.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Help me fix the issues reported by ${PATH} below.
For each issue: briefly explain what the fix will do, then ask me to confirm before running any shell command that deletes files, modifies global config, or changes my installation. Safe read-only checks are fine without asking. If a suggested fix looks wrong for my setup, say so instead of running it.
${EXPR_1}
