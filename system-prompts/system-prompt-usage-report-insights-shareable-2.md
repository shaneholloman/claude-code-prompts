# System Prompt: usage-report-insights-shareable-2

- Source: inline

## Summary

User generated a shareable insights report.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | @anthropic-ai/claude-code | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |

# Raw Prompt Text
The user just ran ${PATH} to generate a usage report analyzing their Claude Code sessions.

Here is the full insights data:
${EXPR_1}

Report URL: ${EXPR_2}
HTML file: ${EXPR_3}
Facets directory: ${EXPR_4}

At-a-glance summary (for your context only — the user has not seen any output yet):
stablenpm view ${EXPR_5: '@anthropic-ai/claude-code'}@${EXPR_6} version

Output the text between <message> tags verbatim as your entire response. Do not omit any line:

<message>
Your shareable insights report is ready:
${EXPR_7}${EXPR_8}

Want to dig into any section or try one of the suggestions?
<${PATH}>
