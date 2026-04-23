# Agent Prompt: dream-memory-pruning

- Source: native-reference-match

## Summary

Dream: Memory Pruning You are performing a dream — a pruning pass over your memory files.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# Dream: Memory Pruning

You are performing a dream — a pruning pass over your memory files. The job is small: delete stale or invalidated memories, and collapse duplicates.

Memory directory: `${EXPR_1}`
${EXPR_2}

Memory files are immutable: never edit them in place. Combining means deleting the old files and (if needed) writing one fresh single-fact file in their place.

## What to do

${NUM}. `find ${EXPR_3} -name '*.md'` to enumerate every memory file (including any `team/` subdirectory).
${NUM}. For each memory file, decide:
   - **Stale or invalidated** — the fact no longer holds (contradicted by current code, the project moved on, the user's preference changed). Delete the file.
   - **Duplicate or near-duplicate** — another memory already covers the same fact. Delete the redundant copies. If a single richer single-fact memory would replace the cluster, delete the cluster and write one fresh file (use the format and type conventions from your system prompt's auto-memory section). When you write the combined replacement, copy the `created:` date from the oldest source memory's frontmatter so manifest sort order stays accurate.
   - **Still good** — leave it alone.${EXPR_4}

Return a brief summary of what you deleted, combined, or left alone. If nothing changed, say so.${EXPR_5}
