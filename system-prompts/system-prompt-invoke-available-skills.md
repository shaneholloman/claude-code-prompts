# System Prompt: invoke-available-skills

- Source: inline

## Summary

Instructs invoking only available skills and describes how skill prompts load.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
Execute a skill within the main conversation

<skills_instructions>
When users ask you to perform tasks, check if any of the available skills below can help complete the task more effectively. Skills provide specialized capabilities and domain knowledge.

How to use skills:
- Invoke skills using this tool with the skill name only (no arguments)
- When you invoke a skill, you will see <command-message>The "{name}" skill is loading<${PATH}>
- The skill's prompt will expand and provide detailed instructions on how to complete the task
- Examples:
  - `skill: "pdf"` - invoke the pdf skill
  - `skill: "xlsx"` - invoke the xlsx skill
  - `skill: "ms-office-suite:pdf"` - invoke using fully qualified name

Important:
- Only use skills listed in <available_skills> below
- Do not invoke a skill that is already running
- Do not use this tool for built-in CLI commands (like ${PATH}, ${PATH}, etc.)
<${PATH}>

<available_skills>
${EXPR_1}${EXPR_2}
<${PATH}>
