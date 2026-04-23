# Agent Prompt: npm-view-version-validating-manifest

- Agent Type: inherit
- Source: inherit

## Summary

Check the version of a specific npm package.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | @anthropic-ai/claude-code | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
npm view ${EXPR_1: '@anthropic-ai/claude-code'}@${EXPR_2} version

Validating ${EXPR_3} manifest: ${EXPR_4}
