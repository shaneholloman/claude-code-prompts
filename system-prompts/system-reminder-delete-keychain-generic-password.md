# System Reminder: delete-keychain-generic-password

- Source: inline

## Summary

Run macOS security command to delete a generic password for account and service.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
security delete-generic-password -a "${EXPR_1}" -s "${EXPR_2}"
