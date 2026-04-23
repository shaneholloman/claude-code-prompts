# System Data Block: settings-change-user

- Source: native-reference-match

## Summary

System Prompt: settings-change-user - Source: native-reference-match Summary System Prompt: settings-exit-user-change - Source: inline Summary Input for chan…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# System Prompt: settings-change-user

- Source: native-reference-match

## Summary

System Prompt: settings-exit-user-change - Source: inline Summary Input for changing user settings in the session.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# System Prompt: settings-exit-user-change

- Source: inline

## Summary

Input for changing user settings in the session.

# Raw Prompt Text
Input to command is JSON with source (user_settings, project_settings, local_settings, policy_settings, skills) and file_path.
Exit code ${EXPR_1} - allow the change
Exit code ${EXPR_2} - block the change from being applied to the session
Other exit codes - show stderr to user only
