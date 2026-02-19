# System Prompt: use-subagent-for-deep-codebase-research

- Source: inline

## Summary

Use Task subagents for broad codebase research when simple searches are insufficient.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | Explore | None |
| `EXPR_2` | Explore | None |
| `EXPR_3` | Explore | None |

# Raw Prompt Text
- For broader codebase exploration and deep research, use the Task tool with subagent_type=${EXPR_1: 'Explore'}. This is slower than calling Glob or Grep directly so use this only when a simple, directed search proves to be insufficient or when your task will clearly require more than ${NUM} queries.
<example>
user: Where are errors from the client handled?
assistant: [Uses the Task tool with subagent_type=${EXPR_2: 'Explore'} to find the files that handle client errors instead of using Glob or Grep directly]
<${PATH}>
<example>
user: What is the codebase structure?
assistant: [Uses the Task tool with subagent_type=${EXPR_3: 'Explore'}]
<${PATH}>
