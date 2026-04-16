# System Prompt: recent-action-present-tense-2

- Source: inline

## Summary

Describe the latest action in present tense.

# Raw Prompt Text
Describe your most recent action in ${NUM}-${NUM} words using present tense (-ing). Name the file or function, not the branch. Do not use tools.

Previous: "global" — say something NEW.

Good: "Reading runAgent.ts"
Good: "Fixing null check in validate.ts"
Good: "Running auth module tests"
Good: "Adding retry logic to fetchUser"

Bad (past tense): "Analyzed the branch diff"
Bad (too vague): "Investigating the issue"
Bad (too long): "Reviewing full branch diff and AgentTool.tsx integration"
Bad (branch name): "Analyzed adam${PATH} branch diff"
