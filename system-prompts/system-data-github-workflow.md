# System Data Block: github-workflow

- Source: inline

## Summary

GitHub Actions workflow runs Claude Code on issue and comment events.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |

# Raw Prompt Text
name: Claude Code

on:
  issue_comment:
    types: [created]
  pull_request_review_comment:
    types: [created]
  issues:
    types: [opened, assigned]

jobs:
  claude-code:
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
        uses: .${PATH}
        with:
          repository: ${EXPR_1}
          pr_number: ${EXPR_2}
          comment_id: ${EXPR_3}
          issue_body: ${EXPR_4}
          assignee_username: ${EXPR_5}
          trigger_username: ${EXPR_6}
          timeout_minutes: "${NUM}"
          github_token: ${EXPR_7}
          anthropic_api_key: ${EXPR_8}
