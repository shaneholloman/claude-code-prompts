# System Data Block: shareable-insights-report-ready


## Summary

Provide exact ready message for shareable insights report with URLs and file paths.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | resolved list (4 items) | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
The user just ran ${PATH} to generate a usage report analyzing their Claude Code sessions.

Here is the full insights data:
global

Report URL: ${EXPR_1}
HTML file: ${EXPR_2}
Facets directory: ${EXPR_3}

Here is what the user sees:
${EXPR_4}

Now output the following message exactly:

<message>
Your shareable insights report is ready:
${EXPR_5}@anthropic-ai${PATH}

Want to dig into any section or try one of the suggestions?
<${PATH}>
