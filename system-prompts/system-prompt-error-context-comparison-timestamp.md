# System Data Block: error-context-comparison

- Source: inline

## Summary

Analyzes error with context and timestamp details.

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

# Raw Prompt Text
=== ERROR ===
${EXPR_1}

=== CONTEXT COMPARISON ===
timestamp: ${EXPR_2}
model: ${EXPR_3}
mainLoopTokens: ${EXPR_4}
classifierChars: ${EXPR_5}
classifierTokensEst: ${EXPR_6}
transcriptEntries: ${EXPR_7}
messages: ${EXPR_8}
delta (classifierEst - mainLoop): ${EXPR_9}

=== ACTION BEING CLASSIFIED ===
${EXPR_10}

=== SYSTEM PROMPT ===
${EXPR_11}

=== USER PROMPT (transcript) ===
${EXPR_12}
