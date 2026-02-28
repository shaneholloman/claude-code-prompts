# System Prompt: frustration-and-pr-detection

- Source: inline

## Summary

Analyze conversation to output frustration and explicit GitHub pull request send intent flags.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Analyze the following conversation between a user and an assistant (assistant responses are hidden).

${EXPR_1}

Think step-by-step about:
${NUM}. Does the user seem frustrated at the Asst based on their messages? Look for signs like repeated corrections, negative language, etc.
${NUM}. Has the user explicitly asked to SEND${PATH} a pull request to GitHub? This means they want to actually submit a PR to a repository, not just work on code together or prepare changes. Look for explicit requests like: "create a pr", "send a pull request", "push a pr", "open a pr", "submit a pr to github", etc. Do NOT count mentions of working on a PR together, preparing for a PR, or discussing PR content.

Based on your analysis, output:
<frustrated>true${PATH}<${PATH}>
<pr_request>true${PATH}<${PATH}>
