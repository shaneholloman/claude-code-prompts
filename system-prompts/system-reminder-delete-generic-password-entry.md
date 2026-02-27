# System Reminder: 5885de94

- Source: inline

## Summary

Shows command to delete a generic password entry for the current user.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
security delete-generic-password -a $USER -s "${EXPR_1}"
