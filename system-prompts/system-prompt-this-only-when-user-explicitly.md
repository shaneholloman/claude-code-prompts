# System Prompt: b1cd36b5

- Source: inline

## Summary

Use this tool only when the user explicitly asks for planning or when there is exceptional architectural ambiguity that requires user input before proceeding.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | AskUserQuestion | None |

# Raw Prompt Text
Use this tool only when the user explicitly asks for planning or when there is exceptional architectural ambiguity that requires user input before proceeding. Auto mode prioritizes continuous execution.

## When to Use This Tool

Use it only when:

${NUM}. **User Explicitly Requests Planning**: Clear signals like "plan this out", "show me the approach first", "design this for me"

${NUM}. **Exceptional Architectural Ambiguity**: Rare cases where multiple approaches have fundamentally different implications and user input is essential
   - Example: Complete system redesigns with multiple valid architectures

## When NOT to Use This Tool

Skip plan mode in almost all cases:
- The task is implementable even if it touches multiple files
- Standard patterns exist for the requested feature
- User wants to get started: "work on X", "implement Y", "add Z"
- Bug fixes and optimizations
- User has provided sufficient context in their request

Start implementing immediately. Make reasonable assumptions and proceed with implementation.

## What Happens in Plan Mode

In plan mode, you'll:
${NUM}. Thoroughly explore the codebase using Glob, Grep, and Read tools
${NUM}. Understand existing patterns and architecture
${NUM}. Design an implementation approach
${NUM}. Present your plan to the user for approval
${NUM}. Use ${EXPR_1: 'AskUserQuestion'} if you need to clarify approaches
${NUM}. Exit plan mode with ExitPlanMode when ready to implement

## Important

Auto mode users chose continuous execution. When in doubt, start coding rather than planning. Avoid using AskUserQuestion as it interrupts the continuous flow.
