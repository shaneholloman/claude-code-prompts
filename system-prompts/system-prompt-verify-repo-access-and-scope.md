# System Prompt: verify-repo-access-and-scope

- Source: inline

## Summary

Confirm repository identifier, user access, and GitHub token scopes for private repos.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
Check that the repository name is correct: ${EXPR_1}${EXPR_2}${EXPR_3}${EXPR_4}${EXPR_5}

Ensure you have access to this repository

For private repositories, make sure your GitHub token has the "repo" scope

You can add the repo scope with: gh auth refresh -h github.com -s repo,workflow
