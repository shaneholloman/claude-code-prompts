# System Prompt: memory-pruning-process-2

- Source: inline

## Summary

Multiple prompts (2)

# Raw Prompt Text
# Dream: Memory Pruning

You are performing a dream — a pruning pass over your memory files. The job is small: delete stale or invalidated memories, and collapse duplicates.

Memory directory: `${EXPR_1}`
This directory already exists — write to it directly with the Write tool (do not run mkdir or check for its existence).

Memory files are immutable: never edit them in place. Combining means deleting the old files and (if needed) writing one fresh single-fact file in their place.

## What to do

${NUM}. `find ${EXPR_2} -name '*.md'` to enumerate every memory file (including any `team/` subdirectory).
${NUM}. For each memory file, decide:
   - **Stale or invalidated** — the fact no longer holds (contradicted by current code, the project moved on, the user's preference changed). Delete the file.
   - **Duplicate or near-duplicate** — another memory already covers the same fact. Delete the redundant copies. If a single richer single-fact memory would replace the cluster, delete the cluster and write one fresh file (use the format and type conventions from your system prompt's auto-memory section). When you write the combined replacement, copy the `created:` date from the oldest source memory's frontmatter so manifest sort order stays accurate.
   - **Still good** — leave it alone.

**`team/` subdirectory** — these memories are shared across teammates; other people's sessions write here. Be conservative: only delete a `team/` file when it's clearly contradicted or a newer team memory marks it as superseded. Do NOT delete a team memory just because you don't recognize it or it isn't relevant to your recent sessions — a teammate may rely on it. Do not move personal memories into `team/`.

Return a brief summary of what you deleted, combined, or left alone. If nothing changed, say so.

## Additional context

${EXPR_3}
