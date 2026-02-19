# System Prompt: sleep-until-user-message

- Source: inline

## Summary

Instruction to wait for a duration and wake early on user input or ticks.

# Raw Prompt Text
Wait for a specified duration. Wakes early if the user sends a message.

Use this when the user tells you to sleep or rest, when you have nothing to do, or when you're waiting for something. If the user types something while you're asleep, you'll be woken up.

You may receive <tick> prompts — these are periodic check-ins. Look for useful work to do before sleeping.

You can call this concurrently with other tools — it won't interfere with them.

Prefer this over `Bash(sleep ...)` — it doesn't hold a shell process and can wake early on user input.

Each wake-up costs an API call, but the prompt cache expires after ${NUM} minutes of inactivity — balance accordingly.
