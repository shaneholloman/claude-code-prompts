# Tool Description: retrieve-task-details

- Name: TaskGet

## Summary

Fetch full task information, comments, and dependency links by ID.

# Raw Prompt Text
Use this tool to retrieve a task by its ID from the task list.

## When to Use This Tool

- When you need the full description and context before starting work on a task
- To check comments and progress history on a task
- To understand task dependencies (what it blocks, what blocks it)
- After being assigned a task, to get complete requirements

## Output

Returns full task details:
- **subject**: Task title
- **description**: Detailed requirements and context
- **status**: 'open' or 'resolved'
- **comments**: Progress notes and discussions from agents
- **references**: Related tasks (bidirectional links)
- **blocks**: Tasks waiting on this one to complete
- **blockedBy**: Tasks that must complete before this one can start

Use TaskList to see all tasks in summary form.
