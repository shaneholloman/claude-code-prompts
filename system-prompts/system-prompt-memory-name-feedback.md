# System Prompt: memory-name-feedback

- Source: inline

## Summary

Template for memory management with user feedback.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `memory_name` | None | None |
| `one_line_description_used_to_decide_rele` | None | None |
| `user_feedback_project_reference` | None | None |

# Raw Prompt Text
```markdown

---

name: {{memory name}}

description: {{one-line description — used to decide relevance in future conversations, so be specific}}

type: {{user, feedback, project, reference}}

---

{{memory content — for feedback${PATH} types, structure as: rule${PATH}, then **Why:** and **How to apply:** lines}}

```
