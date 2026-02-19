# System Prompt: pull-request-review-workflow

- Source: inline

## Summary

Pull request-triggered GitHub Actions job checks out code and runs Claude review action.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
name: Claude Code Review

on:
  pull_request:
    types: [opened, synchronize]
    # Optional: Only run on specific file changes
    # paths:
    #   - "src/**/*.ts"
    #   - "src/**/*.tsx"
    #   - "src/**/*.js"
    #   - "src/**/*.jsx"

jobs:
  claude-review:
    # Optional: Filter by PR author
    # if: |
    #   github.event.pull_request.user.login == 'external-contributor' ||
    #   github.event.pull_request.user.login == 'new-developer' ||
    #   github.event.pull_request.author_association == 'FIRST_TIME_CONTRIBUTOR'

    runs-on: ubuntu-latest
    permissions:
      contents: read
      pull-requests: read
      issues: read
      id-token: write

    steps:
      - name: Checkout repository
        uses: actions${PATH}@v4
        with:
          fetch-depth: ${NUM}

      - name: Run Claude Code Review
        id: claude-review
        uses: anthropics${PATH}@beta
        with:
          anthropic_api_key: ${EXPR_1}

          # Optional: Specify model (defaults to Claude Sonnet ${NUM}, uncomment for Claude Opus ${NUM})
          # model: "claude-opus-${NUM}-${NUM}"

          # Direct prompt for automated review (no @claude mention needed)
          direct_prompt: |
            Please review this pull request and provide feedback on:
            - Code quality and best practices
            - Potential bugs or issues
            - Performance considerations
            - Security concerns
            - Test coverage

            Be constructive and helpful in your feedback.

          # Optional: Use sticky comments to make Claude reuse the same comment on subsequent pushes to the same PR
          # use_sticky_comment: true

          # Optional: Customize review based on file types
          # direct_prompt: |
          #   Review this PR focusing on:
          #   - For TypeScript files: Type safety and proper interface usage
          #   - For API endpoints: Security, input validation, and error handling
          #   - For React components: Performance, accessibility, and best practices
          #   - For tests: Coverage, edge cases, and test quality

          # Optional: Different prompts for different authors
          # direct_prompt: |
          #   ${EXPR_2}

          # Optional: Add specific tools for running tests or linting
          # allowed_tools: "Bash(npm run test),Bash(npm run lint),Bash(npm run typecheck)"

          # Optional: Skip review for certain conditions
          # if: |
          #   !contains(github.event.pull_request.title, '[skip-review]') &&
          #   !contains(github.event.pull_request.title, '[WIP]')
