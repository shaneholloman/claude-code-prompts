# Tool Description: friction-points-json-categories

- Source: native-reference-match

## Summary

Tool Description: friction-points-json-categories - Name: friction_analysis Summary JSON schema and instructions to categorize user friction patterns with de…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# Tool Description: friction-points-json-categories

- Name: friction_analysis

## Summary

JSON schema and instructions to categorize user friction patterns with descriptions and examples in second person.

# Raw Prompt Text
Analyze this Claude Code usage data and identify friction points for this user. Use second person ("you").

RESPOND WITH ONLY A VALID JSON OBJECT:
{
  "intro": "${EXPR_1} sentence summarizing friction patterns",
  "categories": [
    {"category": "Concrete category name", "description": "${EXPR_2}-${EXPR_3} sentences explaining this category and what could be done differently. Use 'you' not 'the user'.", "examples": ["Specific example with consequence", "Another example"]}
  ]
}

Include ${EXPR_4} friction categories with ${EXPR_5} examples each.
