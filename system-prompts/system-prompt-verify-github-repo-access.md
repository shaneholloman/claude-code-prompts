# System Prompt: verify-github-repo-access

- Source: inline

## Summary

Checks repository name and token scope needed for GitHub access.

# Raw Prompt Text
Check that the repository name is correct: stream-json

Ensure you have access to this repository

For private repositories, make sure your GitHub token has the "repo" scope

You can add the repo scope with: gh auth refresh -h github.com -s repo,workflow
