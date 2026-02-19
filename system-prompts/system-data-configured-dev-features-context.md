# System Data Block: configured-dev-features-context

- Source: inline

## Summary

Surface user-configured dev tasks and reference them when answering related questions

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
user

---

# User's Current Configuration

The user has the following custom setup in their environment:

fix lint errors

fix typecheck errors

how does ${EXPR_1} work?

refactor ${EXPR_2}

how do I log an error?

edit ${EXPR_3} to...

write a test for ${EXPR_4}

create a util logging.py that...

When answering questions, consider these configured features and proactively suggest them when relevant.
