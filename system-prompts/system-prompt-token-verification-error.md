# System Prompt: token-verification-error

- Source: inline

## Summary

Error verifying organization due to token scope issues.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Unable to verify organization for the current authentication token.
This machine requires ${EXPR_1} but the profile could not be fetched.
This may be a network error, or the token may lack the user:profile scope required for
verification (tokens from 'claude setup-token' do not include this scope).
Try again, or obtain a full-scope token via 'claude auth login'.
