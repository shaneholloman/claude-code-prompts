# System Data Block: npm-view-version-with-context

- Source: inline

## Summary

Runs npm view to fetch a package version using name and tag placeholders.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | @anthropic-ai/claude-code | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
---
npm view ${EXPR_1: '@anthropic-ai/claude-code'}@${EXPR_2} version---
${EXPR_3}
