# Skill: dream-nightly-schedule

- Source: native-reference-match

## Summary

Dream: Schedule Nightly Consolidation The user wants to set up a recurring nightly memory consolidation job.

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

# Raw Prompt Text
# Dream: Schedule Nightly Consolidation

The user wants to set up a recurring nightly memory consolidation job.

**Step ${NUM} — Dedup any existing nightly job**

Call ${EXPR_1} and check for an existing task with prompt `"${PATH} consolidate"`. If one exists, delete it with ${EXPR_2} first so renewal doesn't leave overlapping jobs.

**Step ${NUM} — Schedule**

Call ${EXPR_3} with:
- `cron`: `"${EXPR_4}"`
- `prompt`: `"${PATH} consolidate"`
- `recurring`: true
- `durable`: true

(The `consolidate` suffix means this prompt won't match SCHEDULING_KEYWORDS when it fires (so it runs the consolidation path), won't exact-match migrateAssistantTasksPermanent()'s `'${PATH}'` check (so it stays non-permanent), and resolves via the primary name on both bundled and disk skills (so it keeps working if the bundled skill is disabled via kill-switch or KAIROS activation).)

**Step ${NUM} — Confirm**

Tell the user:
- ${PATH} will run nightly at ~${EXPR_5} local to consolidate and organize memories
- The schedule persists across sessions (written to .claude${PATH})
- Recurring tasks auto-expire after ${EXPR_6} days — re-run `${PATH} nightly` to renew
- Cancel anytime with ${EXPR_7} (include the job ID)

**Step ${NUM} — Run an immediate consolidation**

${EXPR_8}
