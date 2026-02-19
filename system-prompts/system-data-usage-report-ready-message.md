# System Data Block: usage-report-ready-message


## Summary

Provides usage insights data and instructs outputting an exact shareable report-ready message.

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

# Raw Prompt Text
The user just ran ${PATH} to generate a usage report analyzing their Claude Code sessions.

Here is the full insights data:
${EXPR_1}

Report URL: ${EXPR_2}
HTML file: ${EXPR_3}
Facets directory: ${EXPR_4}

Here is what the user sees:
${EXPR_5}

Now output the following message exactly:

<message>
Your shareable insights report is ready:
${EXPR_6}${EXPR_7}

Want to dig into any section or try one of the suggestions?
<${PATH}>
