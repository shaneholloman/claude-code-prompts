# System Data Block: custom-defaults-task-rules-replacing

- Source: inline

## Summary

Defines custom rules to replace default settings.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | @anthropic-ai/claude-code | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |

# Raw Prompt Text
<task-notification>
<task-id>${EXPR_1}<${PATH}>npm view ${EXPR_2: '@anthropic-ai/claude-code'}@${EXPR_3} version
<task-type>remote_agent<${PATH}>
<output-file>## allow (custom rules replacing defaults)
Custom:
${EXPR_4}

Defaults being replaced:
${EXPR_5}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_6}

Defaults being replaced:
${EXPR_7}

## environment (custom rules replacing defaults)
Custom:
${EXPR_8}

Defaults being replaced:
${EXPR_9}

<${PATH}>
<status>${EXPR_10}<${PATH}>
<summary>Remote task "${EXPR_11}" stable<${PATH}>
<${PATH}>
