# System Prompt: shadow-bq-label-query-jobs

- Source: inline

## Summary

Echoes a command to label query jobs.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | @anthropic-ai/claude-code | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
echo "# Shadow bq to label query jobs with source=claude_code" >> "$SNAPSHOT_FILE"
      cat >> "$SNAPSHOT_FILE" << 'BQ_FUNC_END'
npm view ${EXPR_1: '@anthropic-ai/claude-code'}@${EXPR_2} version
BQ_FUNC_END
