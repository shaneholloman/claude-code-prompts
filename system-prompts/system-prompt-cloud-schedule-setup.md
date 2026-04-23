# System Prompt: cloud-schedule-setup

- Source: inline

## Summary

Check conditions for cloud scheduling options.

# Raw Prompt Text
## Offer cloud first

Before any scheduling step, check whether EITHER is true:
- the parsed interval (rule ${NUM} or ${NUM}) is **≥${NUM} minutes**, or
- regardless of which rule matched, the original input uses daily phrasing ("every morning", "daily", "every day", "each night", "every weekday")

If either is true, call AskUserQuestion first:
- `question`: "This loop stops when you close this session. Set it up as a cloud schedule instead so it keeps running?"
- `header`: "Schedule"
- `options`: `[{label: "Cloud schedule (recommended)", description: "Runs in Anthropic's cloud even after you close this session"}, {label: "This session only", description: "Runs in this terminal until you exit"}]`

If they pick **Cloud schedule**: do NOT call CronCreate. Invoke the `schedule` skill directly via the Skill tool with `args` set to their original input verbatim (e.g. `Skill({skill: "schedule", args: "every morning tell me a joke"})`), then follow that skill's instructions to completion. Do NOT tell the user to run ${PATH} themselves. **Then stop — do not continue to any section below** (no CronCreate, no ScheduleWakeup, no "execute the prompt now").
If they pick **This session only**:
- If the trigger was a parsed ≥${NUM}-minute interval (rule ${NUM} or ${NUM}): continue below with that interval.
- If the trigger was daily phrasing only (rule ${NUM}, no parsed interval): do NOT call CronCreate. Explain that a daily-cadence loop won't fire before this session closes, so there's nothing useful to schedule locally — suggest they either pick Cloud schedule, or re-run `${PATH}` with an explicit shorter interval (e.g. `${PATH} 1h <prompt>`) if they want a session loop. Then stop.
If neither trigger condition was met: continue below.
