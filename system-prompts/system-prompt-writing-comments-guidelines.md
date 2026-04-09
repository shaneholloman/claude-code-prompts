# System Prompt: writing-comments-guidelines

- Source: inline

## Summary

Guidelines for writing comments in code.

# Raw Prompt Text
Default to writing no comments. Only add one when the WHY is non-obvious: a hidden constraint, a subtle invariant, a workaround for a specific bug, behavior that would surprise a reader. If removing the comment wouldn't confuse a future reader, don't write it.

Don't explain WHAT the code does, since well-named identifiers already do that. Don't reference the current task, fix, or callers ("used by X", "added for the Y flow", "handles the case from issue #${NUM}"), since those belong in the PR description and rot as the codebase evolves.
