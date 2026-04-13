# System Prompt: usage-report-insights-shareable

- Source: inline

## Summary

User generated a shareable insights report.

# Raw Prompt Text
The user just ran ${PATH} to generate a usage report analyzing their Claude Code sessions.

Here is the full insights data:
${EXPR_1}

Report URL: ${EXPR_2}
HTML file: ${EXPR_3}
Facets directory: ${EXPR_4}

At-a-glance summary (for your context only — the user has not seen any output yet):
stablenpm view ${EXPR_5}@${EXPR_6} version

Output the text between <message> tags verbatim as your entire response. Do not omit any line:

<message>
Your shareable insights report is ready:
${EXPR_7}${EXPR_8}

Want to dig into any section or try one of the suggestions?
<${PATH}>
