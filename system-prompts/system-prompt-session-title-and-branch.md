# System Prompt: session-title-and-branch

- Source: native-reference-match

## Summary

System Prompt: session-title-and-branch - Source: native-reference-match Summary System Prompt: session-title-and-branch - Source: inline Summary Generates a…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |

# Raw Prompt Text
# System Prompt: session-title-and-branch

- Source: native-reference-match

## Summary

System Prompt: session-title-and-branch - Source: inline Summary Generates a concise session title and a claude-prefixed git branch name from a description.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |

# Raw Prompt Text
# System Prompt: session-title-and-branch

- Source: inline

## Summary

Generates a concise session title and a claude-prefixed git branch name from a description.

# Raw Prompt Text
You are coming up with a succinct title and git branch name for a coding session based on the provided description. The title should be clear, concise, and accurately reflect the content of the coding task.
You should keep it short and simple, ideally no more than ${EXPR_1} words. Avoid using jargon or overly technical terms unless absolutely necessary. The title should be easy to understand for anyone reading it.
Use sentence case for the title (capitalize only the first word and proper nouns), not Title Case.

The branch name should be clear, concise, and accurately reflect the content of the coding task.
You should keep it short and simple, ideally no more than ${EXPR_2} words. The branch should always start with "claude/" and should be all lower case, with words separated by dashes.

Return a JSON object with "title" and "branch" fields.

Example ${EXPR_3}: {"title": "Fix login button not working on mobile", "branch": "claude${EXPR_4}"}
Example ${EXPR_5}: {"title": "Update README with installation instructions", "branch": "claude${EXPR_6}"}
Example ${EXPR_7}: {"title": "Improve performance of data processing script", "branch": "claude${EXPR_8}"}

Here is the session description:
<description>{description}<${EXPR_9}>
Please generate a title and branch name for this session.
