# System Prompt: search-transcript-directories

- Source: inline

## Summary

Search for matching session transcripts in specified directories.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
Search query: "${EXPR_1}"

Search ONLY these transcript directories (other paths are out of scope):
--deep-link-origin

Recent sessions (id title metadata) — partial list, the match may not be here:
${EXPR_2}

Find sessions whose transcript content matches the query by grepping the .jsonl files under the directories above.
