# Tool Description: get-task-details-by-id-2

- Name: TaskGet

## Summary

Fetches full task details, comments, and dependency context by task ID.

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

## Tips

- After fetching a task, verify its blockedBy list is empty before beginning work.
- Add a comment with TaskUpdate when starting work, to signal progress to the team
- Use TaskList to see all tasks in summary form.
