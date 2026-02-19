# System Data Block: github-events-trigger

- Source: inline

## Summary

GitHub Actions workflow triggers Claude Code job when @claude appears in events.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
name: Claude Code

on:
  issue_comment:
    types: [created]
  pull_request_review_comment:
    types: [created]
  issues:
    types: [opened, assigned]
  pull_request_review:
    types: [submitted]

jobs:
  claude:
    if: |
      (github.event_name == 'issue_comment' && contains(github.event.comment.body, '@claude')) ||
      (github.event_name == 'pull_request_review_comment' && contains(github.event.comment.body, '@claude')) ||
      (github.event_name == 'pull_request_review' && contains(github.event.review.body, '@claude')) ||
      (github.event_name == 'issues' && (contains(github.event.issue.body, '@claude') || contains(github.event.issue.title, '@claude')))
    runs-on: ubuntu-latest
    permissions:
      contents: read
      pull-requests: read
      issues: read
      id-token: write
      actions: read # Required for Claude to read CI results on PRs
    steps:
      - name: Checkout repository
        uses: actions${PATH}@v4
        with:
          fetch-depth: ${NUM}

      - name: Run Claude Code
        id: claude
        uses: anthropics${PATH}@beta
        with:
          anthropic_api_key: ${EXPR_1}

          # This is an optional setting that allows Claude to read CI results on PRs
          additional_permissions: |
            actions: read

          # Optional: Specify model (defaults to Claude Sonnet ${NUM}, uncomment for Claude Opus ${NUM})
          # model: "claude-opus-${NUM}-${NUM}-${NUM}"

          # Optional: Customize the trigger phrase (default: @claude)
          # trigger_phrase: "${PATH}"

          # Optional: Trigger when specific user is assigned to an issue
          # assignee_trigger: "claude-bot"

          # Optional: Allow Claude to run specific commands
          # allowed_tools: "Bash(npm install),Bash(npm run build),Bash(npm run test:*),Bash(npm run lint:*)"

          # Optional: Add custom instructions for Claude to customize its behavior for your project
          # custom_instructions: |
          #   Follow our coding standards
          #   Ensure all new code has tests
          #   Use TypeScript for new files

          # Optional: Custom environment variables for Claude
          # claude_env: |
          #   NODE_ENV: test
