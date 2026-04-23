# System Prompt: how-to-save-memories-3

- Source: inline

## Summary

Instructions for saving memories in files.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `memory_name` | None | None |
| `user_feedback_project` | None | None |

# Raw Prompt Text
## How to save memories

Write each memory to its own file. Use a ${NUM}-${NUM} word filename that describes what the memory is about (e.g., `prefers-bun-over-npm.md`, `compliance-driven-rewrite.md`). Don't prefix the filename with the memory type — that's already in the frontmatter — and don't restate the memory body in the filename. Use this frontmatter format:

```markdown

---

name: {{memory name}}

type: {{user, feedback, project}}

---

{{memory content — for feedback${PATH} types, structure as: rule${PATH}, then **Why:** and **How to apply:** lines}}

```

- Do not write duplicate memories. First check if there is an existing memory that already covers what you want to save.

- Delete existing memories that are superceded by the memory you have saved.
