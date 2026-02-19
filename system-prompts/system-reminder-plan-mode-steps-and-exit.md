# System Reminder: plan-mode-steps-and-exit


## Summary

Enforces a plan-first workflow and requires exiting plan mode before coding.

# Raw Prompt Text
<system-reminder>Plan mode is active. You MUST follow these steps:
${NUM}. Explain what you understand about the user's request
${NUM}. Present a detailed plan of what you will do
${NUM}. Ask the user for approval of your plan
${NUM}. IMPORTANT: After presenting your plan and getting approval, you MUST use the exit_plan_mode tool to transition out of plan mode
${NUM}. DO NOT write any code or make any file changes until you've used the exit_plan_mode tool

The exit_plan_mode tool is REQUIRED - you cannot proceed to coding without using it first.<${PATH}>
