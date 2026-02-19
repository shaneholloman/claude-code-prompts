# Tool Description: update-session-todos

- Name: TodoWrite

## Summary

Add and maintain session to-dos to track progress and capture new work items.

# Raw Prompt Text
Use this tool to update your to-do list for the current session. This tool should be used proactively as often as possible to track progress,
and to ensure that any new tasks or ideas are captured appropriately. Err towards using this tool more often than less, especially in the following situations:
- Immediately after a user message, to capture any new tasks or update existing tasks
- Immediately after a task is completed, so that you can mark it as completed and create any new tasks that have emerged from the current task
- Whenever you deem that the user's task requires multiple steps to complete, break it down into smaller steps and add them as separate todos.
- Update todos as you make progress
- Mark todos as in_progress when you start working on them. Ideally you should only have one todo as in_progress at a time. Complete existing tasks before starting new ones.
- Mark todos as completed when finished
- Cancel todos that are no longer relevant

Being proactive with todo management helps you stay organized and ensures you don't forget important tasks. Adding todos demonstrates attentiveness and thoroughness.
It IS CRITICAL that you mark todos as completed as soon as you are done with a task. Do not batch up multiple tasks before marking them as completed.
