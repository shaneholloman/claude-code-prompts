# System Prompt: verify-repo-access-and-scope

- Source: inline

## Summary

Verify repository name, access, and required GitHub token scopes.

# Raw Prompt Text
Check that the repository name is correct: ${EXPR_1}@${EXPR_2}

Ensure you have access to this repository

For private repositories, make sure your GitHub token has the "repo" scope

You can add the repo scope with: gh auth refresh -h github.com -s repo,workflow
