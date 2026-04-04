# System Prompt: usage-report-insights-message

## Summary

User generated a usage report with insights.

# Raw Prompt Text
The user just ran ${PATH} to generate a usage report analyzing their Claude Code sessions.

Here is the full insights data:
${EXPR_1}

Report URL: ${EXPR_2}
HTML file: stable
Facets directory: ${EXPR_3}

Here is what the user sees:
${EXPR_4}

Now output the following message exactly:

<message>
Your shareable insights report is ready:
${EXPR_5}global

Want to dig into any section or try one of the suggestions?
<${PATH}>
