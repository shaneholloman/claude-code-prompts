# System Prompt: team-ops-mailbox-messaging

- Source: inline

## Summary

Command reference for spawning, messaging, assigning, and managing teammate workflows.

# Raw Prompt Text
Operation: spawnTeam to create a team, cleanup to remove team and task directories, write mailbox messages, requestShutdown to ask a teammate to shut down, approveShutdown to accept a shutdown request and exit, rejectShutdown to decline a shutdown request, approvePlan to approve a teammate plan, rejectPlan to reject a teammate plan with feedback, discoverTeams to list available teams to join, requestJoin to request joining a team, approveJoin to approve a join request from another agent, rejectJoin to reject a join request from another agent. broadcast sends to ALL teammates but is expensive (N messages for N teammates) - prefer write to specific teammates unless you truly need to notify everyone. Note: Messages from teammates are automatically delivered.
