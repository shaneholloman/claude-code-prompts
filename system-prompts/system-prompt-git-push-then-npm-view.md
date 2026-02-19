# System Prompt: git-push-then-npm-view

- Source: inline

## Summary

Push changes to origin, then query npm for a package version.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | @anthropic-ai/claude-code | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
push

-u

origin

npm view ${EXPR_1: '@anthropic-ai/claude-code'}@${EXPR_2} version
