# Agent Prompt: batch-slash-command

- Source: native-reference-match

## Summary

Batch: Parallel Work Orchestration You are orchestrating a large, parallelizable change across this codebase.

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

# Raw Prompt Text
# Batch: Parallel Work Orchestration

You are orchestrating a large, parallelizable change across this codebase.

## User Instruction

${EXPR_1}

## Phase ${NUM}: Research and Plan (Plan Mode)

Call the `${EXPR_2}` tool now to enter plan mode, then:

${NUM}. **Understand the scope.** Launch one or more subagents (in the foreground — you need their results) to deeply research what this instruction touches. Find all the files, patterns, and call sites that need to change. Understand the existing conventions so the migration is consistent.

${NUM}. **Decompose into independent units.** Break the work into ${EXPR_3}–${EXPR_4} self-contained units. Each unit must:
   - Be independently implementable in an isolated git worktree (no shared state with sibling units)
   - Be mergeable on its own without depending on another unit's PR landing first
   - Be roughly uniform in size (split large units, merge trivial ones)

   Scale the count to the actual work: few files → closer to ${EXPR_5}; hundreds of files → closer to ${EXPR_6}. Prefer per-directory or per-module slicing over arbitrary file lists.

${NUM}. **Determine the e2e test recipe.** Figure out how a worker can verify its change actually works end-to-end — not just that unit tests pass. Look for:
   - A `claude-in-chrome` skill or browser-automation tool (for UI changes: click through the affected flow, screenshot the result)
   - A `tmux` or CLI-verifier skill (for CLI changes: launch the app interactively, exercise the changed behavior)
   - A dev-server + curl pattern (for API changes: start the server, hit the affected endpoints)
   - An existing e2e${PATH} test suite the worker can run

   If you cannot find a concrete e2e path, use the `${EXPR_7}` tool to ask the user how to verify this change end-to-end. Offer ${NUM}–${NUM} specific options based on what you found (e.g., "Screenshot via chrome extension", "Run `bun run dev` and curl the endpoint", "No e2e — unit tests are sufficient"). Do not skip this — the workers cannot ask the user themselves.

   Write the recipe as a short, concrete set of steps that a worker can execute autonomously. Include any setup (start a dev server, build first) and the exact command${PATH} to verify.

${NUM}. **Write the plan.** In your plan file, include:
   - A summary of what you found during research
   - A numbered list of work units — for each: a short title, the list of files${PATH} it covers, and a one-line description of the change
   - The e2e test recipe (or "skip e2e because …" if the user chose that)
   - The exact worker instructions you will give each agent (the shared template)

${NUM}. Call `${EXPR_8}` to present the plan for approval.

## Phase ${NUM}: Spawn Workers (After Plan Approval)

Once the plan is approved, spawn one background agent per work unit using the `${EXPR_9}` tool. **All agents must use `isolation: "worktree"` and `run_in_background: true`.** Launch them all in a single message block so they run in parallel.

For each agent, the prompt must be fully self-contained. Include:
- The overall goal (the user's instruction)
- This unit's specific task (title, file list, change description — copied verbatim from your plan)
- Any codebase conventions you discovered that the worker needs to follow
- The e2e test recipe from your plan (or "skip e2e because …")
- The worker instructions below, copied verbatim:

```
${EXPR_10}
```

Use `subagent_type: "general-purpose"` unless a more specific agent type fits.

## Phase ${NUM}: Track Progress

After launching all workers, render an initial status table:

| # | Unit | Status | PR |
|---|------|--------|----|
| ${NUM} | <title> | running | — |
| ${NUM} | <title> | running | — |

As background-agent completion notifications arrive, parse the `PR: <url>` line from each agent's result and re-render the table with updated status (`done` / `failed`) and PR links. Keep a brief failure note for any agent that did not produce a PR.

When all agents have reported, render the final table and a one-line summary (e.g., "${NUM}/${NUM} units landed as PRs").
