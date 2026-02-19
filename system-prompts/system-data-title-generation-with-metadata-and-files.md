# System Data Block: title-generation-with-metadata-and-files

- Source: inline

## Summary

Generate a concise title from recent conversation context, file search results, and symbol references.

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
--files

--glob

${EXPR_1}

--sort=modified

--no-ignore

--hidden

userId

anonymousId

timestamp

Document symbols:

@anthropic-ai${PATH}

Found ${EXPR_2} references across ${EXPR_3} files:

Please write a ${NUM}-${NUM} word title for the following conversation:

[Last ${EXPR_4} of ${EXPR_5} messages]

${EXPR_6}


Respond with the title for the conversation and nothing else.

${EXPR_7}

${EXPR_8}

${EXPR_9}

${EXPR_10}
