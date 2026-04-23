# Skill: dynamic-pacing-loop-execution

- Source: native-reference-match

## Summary

…. **Run … now**, following the instructions inlined below.

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
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |

# Raw Prompt Text
${NUM}. **Run ${EXPR_1} now**, following the instructions inlined below.
${NUM}. **If the next tick is gated on an event** (CI finishing, a PR comment, a log line) and no ${EXPR_2} is already running for it: arm one now with `persistent: true`. Its events wake this loop immediately — you do not wait for the ${EXPR_3} deadline. Arm once; on later ticks call ${EXPR_4} first and skip if a monitor is already running.
${NUM}. **At the end of this turn, call ${EXPR_5}** with:
   - `delaySeconds`: with a ${EXPR_6} armed this is the fallback heartbeat (lean ${NUM}–1800s). Without one, pick based on what you observed this turn — quiet branch? wait longer. Lots in flight? wait shorter. Read the tool's own description for cache-aware delay guidance.
   - `reason`: one short sentence on why you picked that delay.
   - `prompt`: the literal string `${EXPR_7}` — the dynamic-mode sentinel expands at fire time to the full instructions (first fire / first fire post-compact / loop.md edited) or a dynamic-pacing-specific short reminder (subsequent fires). Do not pass the full instructions; that is handled automatically.
${NUM}. **If woken by a `<task-notification>`** rather than this prompt: handle the event, then call ${EXPR_8} again with `${EXPR_9}` and the same ${NUM}–1800s `delaySeconds` — the ${EXPR_10} remains the wake signal; this only resets the safety net.
${NUM}. **To stop the loop**, omit the ${EXPR_11} call and ${EXPR_12} any ${EXPR_13} you armed (use ${EXPR_14} to find the task ID if it is no longer in context).${EXPR_15}
${NUM}. Briefly confirm: ${EXPR_16}, whether a ${EXPR_17} is the primary wake signal, and what fallback delay you picked.
