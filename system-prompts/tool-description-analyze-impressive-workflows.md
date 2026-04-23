# Tool Description: analyze-impressive-workflows

- Source: native-reference-match

## Summary

Tool Description: analyze-impressive-workflows - Name: what_works Summary Second-person analysis of usage data highlighting what you do well in key workflows.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
# Tool Description: analyze-impressive-workflows

- Name: what_works

## Summary

Second-person analysis of usage data highlighting what you do well in key workflows.

# Raw Prompt Text
Analyze this Claude Code usage data and identify what's working well for this user. Use second person ("you").

RESPOND WITH ONLY A VALID JSON OBJECT:
{
  "intro": "${EXPR_1} sentence of context",
  "impressive_workflows": [
    {"title": "Short title (${EXPR_2}-${EXPR_3} words)", "description": "${EXPR_4}-${EXPR_5} sentences describing the impressive workflow or approach. Use 'you' not 'the user'."}
  ]
}

Include ${EXPR_6} impressive workflows.
