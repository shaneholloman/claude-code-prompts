# System Reminder: anthropic-billing-header-metadata

- Source: inline

## Summary

Emit an x-anthropic-billing-header string with cc_version, cc_entrypoint, and cch fields.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
x-anthropic-billing-header: cc_version=${EXPR_1}; cc_entrypoint=${EXPR_2}; cch=${NUM};
