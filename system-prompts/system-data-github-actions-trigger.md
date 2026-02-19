# System Data Block: github-actions-trigger

- Source: inline

## Summary

GitHub Actions workflow triggers on @claude mentions in issues or comment events.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
name: Claude Code

on:
  issue_comment:
    types: [created, edited]
  pull_request_review_comment:
    types: [created, edited]
  issues:
    types: [opened, assigned, edited]
  pull_request_review:
    types: [submitted, edited]

jobs:
  claude:
    if: |
      (github.event_name == 'issue_comment' && contains(github.event.comment.body, '@claude')) ||
      (github.event_name == 'pull_request_review_comment' && contains(github.event.comment.body, '@claude')) ||
      (github.event_name == 'pull_request_review' && contains(github.event.review.body, '@claude')) ||
      (github.event_name == 'issues' && contains(github.event.issue.body, '@claude'))
    runs-on: ubuntu-latest
    permissions:
      contents: read
      id-token: write
    steps:
      - name: Checkout repository
        uses: actions${PATH}@v4
        with:
          fetch-depth: ${NUM}

      - name: Run Claude Code
        uses: anthropics${PATH}@beta
        with:
          anthropic_api_key: ${EXPR_1}
