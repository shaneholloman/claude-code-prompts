# System Prompt: schedule-recurring-2

- Source: inline

## Summary

Schedule prompts based on specified intervals.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
# ${PATH} — schedule a recurring or self-paced prompt

Parse the input below into `[interval] <prompt…>` and schedule it.

## Parsing (in priority order)

${NUM}. **Leading token**: if the first whitespace-delimited token matches `^\d+[smhd]$` (e.g. `5m`, `2h`), that's the interval; the rest is the prompt.
${NUM}. **Trailing "every" clause**: otherwise, if the input ends with `every <N><unit>` or `every <N> <unit-word>` (e.g. `every 20m`, `every ${NUM} minutes`, `every ${NUM} hours`), extract that as the interval and strip it from the prompt. Only match when what follows "every" is a time expression — `check every PR` has no interval.
${NUM}. **No interval**: otherwise, the entire input is the prompt and you'll self-pace dynamically (see "Dynamic mode" below).

If the resulting prompt is empty, show usage `${PATH} [interval] <prompt>` and stop.

Examples:
- `5m ${PATH}` → interval `5m`, prompt `${PATH}` (rule ${NUM})
- `check the deploy every 20m` → interval `20m`, prompt `check the deploy` (rule ${NUM})
- `run tests every ${NUM} minutes` → interval `5m`, prompt `run tests` (rule ${NUM})
- `check the deploy` → no interval → dynamic mode, prompt `check the deploy` (rule ${NUM})
- `check every PR` → no interval → dynamic mode, prompt `check every PR` (rule ${NUM} — "every" not followed by time)
- `5m` → empty prompt → show usage

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

## Fixed-interval mode (rules ${NUM} and ${NUM})

Convert the interval to a cron expression:

| Interval pattern      | Cron expression     | Notes                                    |
|-----------------------|---------------------|------------------------------------------|
| `Nm` where N ≤ ${NUM}   | `*/N * * * *`     | every N minutes                          |
| `Nm` where N ≥ ${NUM}   | `${NUM} */H * * *`     | round to hours (H = N/${NUM}, must divide ${NUM})|
| `Nh` where N ≤ ${NUM}   | `${NUM} */N * * *`     | every N hours                            |
| `Nd`                | `${NUM} ${NUM} */N * *`     | every N days at midnight local           |
| `Ns`                | treat as `ceil(N/${NUM})m` | cron minimum granularity is ${NUM} minute  |

**If the interval doesn't cleanly divide its unit** (e.g. `7m` → `*/${NUM} * * * *` gives uneven gaps at :${NUM}→:${NUM}; `90m` → ${NUM}.5h which cron can't express), pick the nearest clean interval and tell the user what you rounded to before scheduling.

Then:
${NUM}. Call CronCreate with: `cron` (the expression above), `prompt` (the parsed prompt verbatim), `recurring: true`.
${NUM}. Briefly confirm: what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_1} days, and that the user can cancel sooner with CronDelete (include the job ID). Only if you did NOT show the cloud-offer AskUserQuestion above (i.e., neither trigger condition applied), end the confirmation with this exact line on its own, italicized: `_Runs until you close this session · For durable cloud-based loops, use ${PATH}`. If the user already answered that question, omit this line.
${NUM}. **Then immediately execute the parsed prompt now** — don't wait for the first cron fire. If it's a slash command, invoke it via the Skill tool; otherwise act on it directly.

## Dynamic mode (rule ${NUM} — no interval)

${EXPR_2}

## Input

${EXPR_3}
