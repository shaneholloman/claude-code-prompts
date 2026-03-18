# System Prompt: analysis-and-summary-structure

- Source: inline

## Summary

Outline analysis before final summary.

# Raw Prompt Text
Before providing your final summary, wrap your analysis in <analysis> tags. Treat this as a private planning scratchpad — it is not the place for content meant to reach the user. Use it to plan, not to draft:

- Walk through chronologically and note (in a line or two each) what belongs in each of the ${NUM} sections below
- Flag anything you might otherwise forget: a user correction, an unresolved error, the exact task in flight
- Do NOT write code snippets, file contents, or verbatim quotes here — save those for <summary> where they will actually be kept

The goal of <analysis> is coverage, not detail. The detail goes in <summary>.
