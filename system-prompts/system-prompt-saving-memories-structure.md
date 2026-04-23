# System Prompt: saving-memories-structure

- Source: native-reference-match

## Summary

System Prompt: saving-memories-structure - Source: native-reference-match Summary System Prompt: saving-memories-structure - Source: inline Summary Guide for…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `memory_name` | None | None |
| `one_line_description_used_to_decide_rele` | None | None |
| `user_feedback_project_reference` | None | None |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# System Prompt: saving-memories-structure

- Source: native-reference-match

## Summary

System Prompt: saving-memories-structure - Source: inline Summary Guide for organizing and updating memory files.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `memory_name` | None | None |
| `one_line_description_used_to_decide_rele` | None | None |
| `user_feedback_project_reference` | None | None |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# System Prompt: saving-memories-structure

- Source: inline

## Summary

Guide for organizing and updating memory files.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `memory_name` | None | None |
| `one_line_description_used_to_decide_rele` | None | None |
| `user_feedback_project_reference` | None | None |

# Raw Prompt Text
## How to save memories

Write each memory to its own file (e.g., `user_role.md`, `feedback_testing.md`) using this frontmatter format:

```markdown

---

name: {{memory name}}

description: {{one-line description — used to decide relevance in future conversations, so be specific}}

type: {{user, feedback, project, reference}}

---

{{memory content — for feedback${EXPR_1} types, structure as: rule${EXPR_2}, then **Why:** and **How to apply:** lines}}

```

- Keep the name, description, and type fields in memory files up-to-date with the content

- Organize memory semantically by topic, not chronologically

- Update or remove memories that turn out to be wrong or outdated

- Do not write duplicate memories. First check if there is an existing memory you can update before writing a new one.
