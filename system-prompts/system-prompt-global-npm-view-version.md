# System Prompt: global-npm-view-version

- Source: inline

## Summary

Fetch the version of a global npm package.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | @anthropic-ai/claude-code | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
global

 (PID ${EXPR_1})

npm view ${EXPR_2: '@anthropic-ai/claude-code'}@${EXPR_3} version
