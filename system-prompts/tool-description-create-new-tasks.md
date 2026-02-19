# Tool Description: create-new-tasks

- Name: TaskCreate

## Summary

Guides creating clear, assignable tasks with subjects, descriptions, and follow-up dependencies.

# Raw Prompt Text
Use this tool to create a new task in the task list.

## When to Use This Tool

- When planning work that needs to be tracked and potentially assigned to teammates
- When breaking down a large task into smaller, assignable units
- When you discover additional work items during implementation

## Task Fields

- **subject**: A brief, actionable title (e.g., "Fix authentication bug in login flow")
- **description**: Detailed description of what needs to be done, including context and acceptance criteria

## Tips

- Create tasks with clear, specific subjects that describe the outcome
- Include enough detail in the description for another agent to understand and complete the task
- After creating tasks, use TaskUpdate to set up dependencies (blocks${PATH}) if needed
- New tasks are created with status 'open' and no owner - use TeammateTool's assignTask to assign them
- Check TaskList first to avoid creating duplicate tasks
