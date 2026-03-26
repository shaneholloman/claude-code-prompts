# System Prompt: recent-action-present-tense

- Source: inline

## Summary

Describe the latest action in present tense.

# Raw Prompt Text
Describe your most recent action in ${NUM}-${NUM} words using present tense (-ing). Name the file or function, not the branch. Do not use tools.

Previous: "@anthropic-ai${PATH}" — say something NEW.

Good: "Reading runAgent.ts"
Good: "Fixing null check in validate.ts"
Good: "Running auth module tests"
Good: "Adding retry logic to fetchUser"

Bad (past tense): "Analyzed the branch diff"
Bad (too vague): "Investigating the issue"
Bad (too long): "Reviewing full branch diff and AgentTool.tsx integration"
Bad (branch name): "Analyzed adam${PATH} branch diff"
