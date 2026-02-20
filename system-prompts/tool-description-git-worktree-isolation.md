# Tool Description: git-worktree-isolation

- Name: EnterWorktree

## Summary

Create isolated worktrees for user tasks.

# Raw Prompt Text
Use this tool when the user asks to work in isolation, in a worktree, or on a separate branch without affecting the main working tree. This tool creates an isolated worktree and switches the current session into it.

## When to Use

- The user says "start a worktree", "work in a worktree", "create a worktree"
- The user wants to work on a feature in isolation
- The user wants to make changes on a separate branch without affecting the current one

## Requirements

- Must be in a git repository, OR have WorktreeCreate${PATH} hooks configured in settings.json
- Must not already be in a worktree

## Behavior

- In a git repository: creates a new git worktree inside `.claude${PATH}` with a new branch based on HEAD
- Outside a git repository: delegates to WorktreeCreate${PATH} hooks for VCS-agnostic isolation
- Switches the session's working directory to the new worktree
- On session exit, the user will be prompted to keep or remove the worktree

## Parameters

- `name` (optional): A name for the worktree. If not provided, a random name is generated.
