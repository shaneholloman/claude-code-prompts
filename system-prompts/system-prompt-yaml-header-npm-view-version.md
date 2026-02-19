# System Prompt: yaml-header-npm-view-version

- Source: inline

## Summary

YAML header with dynamic name/description, then runs npm view to fetch package version

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | 100000000 | None |
| `EXPR_4` | None | None |
| `EXPR_5` | @anthropic-ai/claude-code | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
---
name: ${EXPR_1}
description: ${EXPR_2}${EXPR_3: 100000000}${EXPR_4}null
---

npm view ${EXPR_5: '@anthropic-ai/claude-code'}@${EXPR_6} version
