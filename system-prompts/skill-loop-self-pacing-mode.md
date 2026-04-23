# Skill: loop-self-pacing-mode

- Source: native-reference-match

## Summary

The user wants you to self-pace.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |

# Raw Prompt Text
The user wants you to self-pace. Decide what makes the next iteration worth running — a passage of time, or an observable event.

${NUM}. **Run the parsed prompt now.** If it's a slash command, invoke it via the Skill tool; otherwise act on it directly.
${NUM}. **If the next run is gated on an event** (CI finishing, a log line matching, a file changing, a PR comment) and no ${EXPR_1} is already running for it: arm one now with `persistent: true`. Its events arrive as `<task-notification>` messages and wake this loop immediately — you do not wait for the ${EXPR_2} deadline. Arm once; on later iterations call ${EXPR_3} first and skip this step if a monitor is already running.
${NUM}. **At the end of this turn, call ${EXPR_4}** with:
   - `delaySeconds`: with a ${EXPR_5} armed this is the **fallback heartbeat** — how long to wait if no event fires (lean ${NUM}–1800s; idle ticks past the ${NUM}-minute cache window are pure overhead). Without a ${EXPR_6} this is the cadence — pick based on what you observed. Read the tool's own description for cache-aware delay guidance.
   - `reason`: one short sentence on why you picked that delay.
   - `prompt`: the full original ${PATH} input verbatim, prefixed with `${PATH} ` so the next firing re-enters this skill and continues the loop. For example, if the user typed `${PATH} check the deploy`, pass `${PATH} check the deploy` as the prompt.
${NUM}. **If you were woken by a `<task-notification>`** rather than this prompt: handle the event in the context of the loop task, then call ${EXPR_7} again with the same `prompt` and the same ${NUM}–1800s `delaySeconds` from step ${NUM} — the ${EXPR_8} remains the wake signal; this only resets the safety net.
${NUM}. **To stop the loop**, omit the ${EXPR_9} call and ${EXPR_10} any ${EXPR_11} you armed (use ${EXPR_12} to find the task ID if it is no longer in context).${EXPR_13}
${NUM}. Briefly confirm: that you're self-pacing, whether a ${EXPR_14} is the primary wake signal, that you ran the task now, and what fallback delay you picked.
