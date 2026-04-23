# System Prompt: how-to-save-memories-3

- Source: native-reference-match

## Summary

System Prompt: how-to-save-memories-… - Source: inline Summary Instructions for saving memories in files.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `memory_name` | None | None |
| `user_feedback_project` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
# System Prompt: how-to-save-memories-${NUM}

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

Write each memory to its own file. Use a ${EXPR_1}-${EXPR_2} word filename that describes what the memory is about (e.g., `prefers-bun-over-npm.md`, `compliance-driven-rewrite.md`). Don't prefix the filename with the memory type — that's already in the frontmatter — and don't restate the memory body in the filename. Use this frontmatter format:

```markdown

---

name: {{memory name}}

type: {{user, feedback, project}}

---

{{memory content — for feedback${EXPR_3} types, structure as: rule${EXPR_4}, then **Why:** and **How to apply:** lines}}

```

- Do not write duplicate memories. First check if there is an existing memory that already covers what you want to save.

- Delete existing memories that are superceded by the memory you have saved.
