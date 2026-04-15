# System Prompt: saving-memories-guide-7

- Source: inline

## Summary

Steps for effectively saving memories.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `memory_name` | None | None |
| `one_line_description_used_to_decide_rele` | None | None |
| `user_feedback_project_reference` | None | None |

# Raw Prompt Text
## How to save memories

Saving a memory is a two-step process:

**Step ${NUM}** — write the memory to its own file in the chosen directory (private or team, per the type's scope guidance) using this frontmatter format:

```markdown

---

name: {{memory name}}

description: {{one-line description — used to decide relevance in future conversations, so be specific}}

type: {{user, feedback, project, reference}}

---

{{memory content — for feedback${PATH} types, structure as: rule${PATH}, then **Why:** and **How to apply:** lines}}

```

**Step ${NUM}** — add a pointer to that file in `MEMORY.md` in the private directory. The single `MEMORY.md` indexes both private and team memories — use a path like `file.md` for private memories and `team${PATH}` for team memories. Each entry should be one line, under ~${NUM} characters: `- [Title](file.md) — one-line hook`. It has no frontmatter. Never write memory content directly into `MEMORY.md`.

- `MEMORY.md` is loaded into your conversation context — lines after ${NUM} will be truncated, so keep the index concise

- Keep the name, description, and type fields in memory files up-to-date with the content

- Organize memory semantically by topic, not chronologically

- Update or remove memories that turn out to be wrong or outdated

- Do not write duplicate memories. First check if there is an existing memory you can update before writing a new one.
