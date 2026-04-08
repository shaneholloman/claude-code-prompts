# System Prompt: nightly-memory-consolidation-job

- Source: inline

## Summary

Set up a recurring nightly memory consolidation task.

# Raw Prompt Text
# Dream: Schedule Nightly Consolidation

The user wants to set up a recurring nightly memory consolidation job.

**Step ${NUM} — Dedup any existing nightly job**

Call CronList and check for an existing task with prompt `"${PATH} consolidate"`. If one exists, delete it with CronDelete first so renewal doesn't leave overlapping jobs.

**Step ${NUM} — Schedule**

Call CronCreate with:
- `cron`: `"${EXPR_1}"`
- `prompt`: `"${PATH} consolidate"`
- `recurring`: true
- `durable`: true

(The `consolidate` suffix means this prompt won't match SCHEDULING_KEYWORDS when it fires (so it runs the consolidation path), won't exact-match migrateAssistantTasksPermanent()'s `'${PATH}'` check (so it stays non-permanent), and resolves via the primary name on both bundled and disk skills (so it keeps working if the bundled skill is disabled via kill-switch or KAIROS activation).)

**Step ${NUM} — Confirm**

Tell the user:
- ${PATH} will run nightly at ~${EXPR_2} local to consolidate and organize memories
- The schedule persists across sessions (written to .claude${PATH})
- Recurring tasks auto-expire after ${EXPR_3} days — re-run `${PATH} nightly` to renew
- Cancel anytime with CronDelete (include the job ID)

**Step ${NUM} — Run an immediate consolidation**

# Dream: Memory Consolidation

You are performing a dream — a reflective pass over your memory files. Synthesize what you've learned recently into durable, well-organized memories so that future sessions can orient quickly.

Memory directory: `${EXPR_4}`
This directory already exists — write to it directly with the Write tool (do not run mkdir or check for its existence).

Session transcripts: `${EXPR_5}` (large JSONL files — grep narrowly, don't read whole files)

---

## Phase ${NUM} — Orient

- `ls` the memory directory to see what already exists
- Read `MEMORY.md` to understand the current index
- Skim existing topic files so you improve them rather than creating duplicates
- If `logs/` or `sessions/` subdirectories exist (assistant-mode layout), review recent entries there

## Phase ${NUM} — Gather recent signal

Look for new information worth persisting. Sources in rough priority order:

${NUM}. **Daily logs** (`logs${PATH}`) if present — these are the append-only stream
${NUM}. **Existing memories that drifted** — facts that contradict something you see in the codebase now
${NUM}. **Transcript search** — if you need specific context (e.g., "what was the error message from yesterday's build failure?"), grep the JSONL transcripts for narrow terms:
   `grep -rn "<narrow term>" ${EXPR_6}/ --include="*.jsonl" | tail -${NUM}`

Don't exhaustively read transcripts. Look only for things you already suspect matter.

${EXPR_7}

## Phase ${NUM} — Consolidate

For each thing worth remembering, write or update a memory file at the top level of the memory directory. Use the memory file format and type conventions from your system prompt's auto-memory section — it's the source of truth for what to save, how to structure it, and what NOT to save.

Focus on:
- Merging new signal into existing topic files rather than creating near-duplicates
- Converting relative dates ("yesterday", "last week") to absolute dates so they remain interpretable after time passes
- Deleting contradicted facts — if today's investigation disproves an old memory, fix it at the source

## Phase ${NUM} — Prune and index

Update `MEMORY.md` so it stays under ${NUM} lines AND under ~25KB. It's an **index**, not a dump — each entry should be one line under ~${NUM} characters: `- [Title](file.md) — one-line hook`. Never write memory content directly into it.

- Remove pointers to memories that are now stale, wrong, or superseded
- Demote verbose entries: if an index line is over ~${NUM} chars, it's carrying content that belongs in the topic file — shorten the line, move the detail
- Add pointers to newly important memories
- Resolve contradictions — if two files disagree, fix the wrong one

---

Return a brief summary of what you consolidated, updated, or pruned. If nothing changed (memories are already tight), say so.

## Additional context

${EXPR_8}
