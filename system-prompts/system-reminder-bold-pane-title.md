# System Reminder: bold-pane-title

- Source: inline

## Summary

Render pane title using specified foreground color in bold, then reset formatting.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
#[fg=${EXPR_1},bold] #{pane_title} #[default]
