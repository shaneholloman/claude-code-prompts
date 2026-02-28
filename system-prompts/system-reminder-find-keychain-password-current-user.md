# System Reminder: find-keychain-password-current-user

- Source: inline

## Summary

Retrieve a macOS keychain generic password for the current user and service.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
security find-generic-password -a $USER -w -s "${EXPR_1}"
