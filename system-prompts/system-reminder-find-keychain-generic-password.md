# System Reminder: find-keychain-generic-password

- Source: inline

## Summary

Retrieve a macOS keychain generic password for a specified account and service.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
security find-generic-password -a "${EXPR_1}" -w -s "${EXPR_2}"
