# System Data Block: fix-running-issues-help

- Source: native-reference-match

## Summary

System Data Block: fix-running-issues-help - Source: native-reference-match Summary System Prompt: fix-running-issues-help - Source: inline Summary Assist wi…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# System Data Block: fix-running-issues-help

- Source: native-reference-match

## Summary

System Prompt: fix-running-issues-help - Source: inline Summary Assist with reported issues and confirm fixes before execution.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# System Prompt: fix-running-issues-help

- Source: inline

## Summary

Assist with reported issues and confirm fixes before execution.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Help me fix the issues reported by ${EXPR_1} below.
For each issue: briefly explain what the fix will do, then ask me to confirm before running any shell command that deletes files, modifies global config, or changes my installation. Safe read-only checks are fine without asking. If a suggested fix looks wrong for my setup, say so instead of running it.
${EXPR_2}
