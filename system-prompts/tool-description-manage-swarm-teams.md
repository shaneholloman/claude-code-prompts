# Tool Description: manage-swarm-teams

- Name: Teammate

## Summary

Creates, discovers, and coordinates teams and task lists for multi-agent swarm work.

# Raw Prompt Text
# TeammateTool

Manage teams and coordinate teammates in a swarm. Use this tool for team operations, communication, and task assignment. Note: To spawn new teammates, use the Task tool with `team_name` and `name` parameters.

## Operations

### spawnTeam - Create a Team

Create a new team to coordinate multiple agents working on a project. Teams have a ${NUM}:${NUM} correspondence with task lists (Team = Project = TaskList).

```
{
  "operation": "spawnTeam",
  "team_name": "my-project",
  "description": "Working on feature X"
}
```

This creates:
- A team file at `~${PATH}{team-name}.json`
- A corresponding task list directory at `~${PATH}{team-name}/`

### discoverTeams - Discover Available Teams

List teams that are available to join. Returns teams from `~${PATH}` that you are not already a member of.

```
{
  "operation": "discoverTeams"
}
```

Returns a list of teams with:
- **name**: Team name
- **description**: Team description (if set)
- **leadAgentId**: ID of the team leader
- **memberCount**: Current number of team members

Use this to find teams you can request to join with `requestJoin`.

### requestJoin - Request to Join a Team

Send a join request to a team's leader. The leader will receive a `join_request` message and can approve or reject it.

- **team_name**: Name of the team to join (REQUIRED)
- **proposed_name**: (Optional) Your proposed name for the team (defaults to generated slug)
- **capabilities**: (Optional) Description of what you can help with

```
{
  "operation": "requestJoin",
  "team_name": "my-project",
  "proposed_name": "helper",
  "capabilities": "I can help with code review and testing"
}
```

After sending the request, you will receive either a `join_approved` or `join_rejected` message in response.

### approveJoin - Approve a Join Request (Leader Only)

When an agent requests to join your team, they send a join request as a JSON message with `type: "join_request"`. Use `approveJoin` to accept them:
- **target_agent_id**: Use the `proposedName` field from the join_request message (REQUIRED)
- **request_id**: Use the `requestId` field from the join_request message (REQUIRED)

Example: If you receive a message like `{"type":"join_request","proposedName":"helper","requestId":"join-${NUM}",...}`, use:
```
{
  "operation": "approveJoin",
  "target_agent_id": "helper",
  "request_id": "join-${NUM}"
}
```

The agent will be added to your team and notified of approval. They will receive their assigned agent ID, name, and color.

### rejectJoin - Reject a Join Request (Leader Only)

Use `rejectJoin` to decline a join request:
- **target_agent_id**: Use the `proposedName` field from the join_request message (REQUIRED)
- **request_id**: Use the `requestId` field from the join_request message (REQUIRED)
- **reason**: (Optional) Explanation of why the request was rejected

```
{
  "operation": "rejectJoin",
  "target_agent_id": "helper",
  "request_id": "join-${NUM}",
  "reason": "Team is at capacity"
}
```

The agent will be notified of the rejection with your reason.

### cleanup - Clean Up Team Resources

Remove team and task directories when the swarm work is complete:

```
{
  "operation": "cleanup"
}
```

This operation:
- Removes the team directory (`~${PATH}{team-name}/`)
- Removes the task directory (`~${PATH}{team-name}/`)
- Clears team context from the current session

**IMPORTANT**: `cleanup` will fail if the team still has active members. Gracefully terminate teammates first, then call `cleanup` after all teammates have shut down.

Use this when all teammates have finished their work and you want to clean up the team resources. The team name is automatically determined from the `CLAUDE_CODE_TEAM_NAME` environment variable.

## Team Workflow

${NUM}. **Create a team** with `spawnTeam` - this creates both the team and its task list
${NUM}. **Create tasks** using the Task tools (TaskCreate, TaskList, etc.) - they automatically use the team's task list
${NUM}. **Spawn teammates** using the Task tool with `team_name` and `name` parameters to create teammates that join the team
${NUM}. **Assign tasks** using TaskUpdate with `owner` to give tasks to idle teammates
${NUM}. **Teammates work on assigned tasks** and mark them completed via TaskUpdate
${NUM}. **Teammates notify when idle** - when a teammate stops, they automatically send an idle notification to the team leader via mailbox

## Task Ownership

Tasks are assigned using TaskUpdate with the `owner` parameter. Any agent can set or change task ownership via TaskUpdate.

## Automatic Message Delivery
Teammates automatically send an idle notification to the team leader when they finish their work. The notification includes:
- Agent ID of the teammate
- Timestamp
- Optional task completion status

**IMPORTANT**: Messages from teammates are automatically delivered to you. You do NOT need to manually check your inbox.

When you spawn teammates:
- They will send you messages when they complete tasks or need help
- These messages appear automatically as new conversation turns (like user messages)
- If you're busy (mid-turn), messages are queued and delivered when your turn ends
- The UI shows "Queued teammate messages" when messages are waiting

Messages will be delivered automatically.

When reporting on teammate messages, you do NOT need to quote the original message—it's already rendered to the user.

## Environment Variables

Spawned teammates have these environment variables set:
- `CLAUDE_CODE_AGENT_ID`: Unique identifier for this agent
- `CLAUDE_CODE_AGENT_TYPE`: Role${PATH} of the agent (if specified)
- `CLAUDE_CODE_TEAM_NAME`: Name of the team this agent belongs to
- `CLAUDE_CODE_PLAN_MODE_REQUIRED`: Set to "true" if the teammate must enter plan mode before implementing changes

**IMPORTANT for teammates:** Use your `CLAUDE_CODE_AGENT_ID` environment variable when:
- Adding comments to tasks (as the `author` field)
- Sending messages to other teammates
## Discovering Team Members

Teammates can read the team config file to discover other team members:
- **Team config location**: `~${PATH}{team-name}${PATH}`

The config file contains a `members` array with each teammate's:
- `name`: Human-readable name (**always use this** for messaging and task assignment)
- `agentId`: Unique identifier (for reference only - do not use for communication)
- `agentType`: Role${PATH} of the agent

**IMPORTANT**: Always refer to teammates by their NAME (e.g., "team-lead", "researcher", "tester"), never by UUID. Names are used for:
- `target_agent_id` when sending messages
- Identifying task owners

Example of reading team config:
```
Use the Read tool to read ~${PATH}{team-name}${PATH}
```

## Task List Coordination

Teams share a task list that all teammates can access:
- **Task list location**: `~${PATH}{team-name}/`

**IMPORTANT notes for communication with your team**:
- Do not use terminal tools to view your team's activity, always send a message to your teammates (and remember, refer to them by name).
- Your team cannot hear you if you do not use the teammate send message tool. Always send a message to your teammates if you are responding to them.

Teammates should:
${NUM}. Check TaskList periodically, **especially after completing each task**, to find available work or see newly unblocked tasks
${NUM}. Claim unassigned, unblocked tasks with TaskUpdate (set `owner` to your name)
${NUM}. Create new tasks with `TaskCreate` when identifying additional work
${NUM}. Mark tasks as completed with `TaskUpdate` when done, then check TaskList for next work
${NUM}. Coordinate with other teammates by reading the task list status
${NUM}. If all available tasks are blocked, notify the team lead or help resolve blocking tasks

**IMPORTANT**: Do NOT send structured JSON status messages like `{"type":"idle",...}` or `{"type":"task_completed",...}`. Use TaskUpdate to mark tasks completed and the system will automatically send idle notifications when you stop. Just communicate in plain text when you need to message teammates.
