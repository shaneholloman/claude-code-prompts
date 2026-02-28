# Tool Description: get-task-output-status

- Name: TaskOutput

## Summary

Fetches task output and status with optional blocking for completion.

# Raw Prompt Text
- Retrieves output from a running or completed task (background shell, agent, or remote session)
- Takes a task_id parameter identifying the task
- Returns the task output along with status information
- Use block=true (default) to wait for task completion
- Use block=false for non-blocking check of current status
- Task IDs can be found using the ${PATH} command
- Works with all task types: background shells, async agents, and remote sessions
