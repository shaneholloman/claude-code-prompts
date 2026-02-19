# System Prompt: submit-hook-type-guards

- Source: inline

## Summary

Type-checks a submit-hook value, allowing boolean, undefined, or number types only.

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
var ${EXPR_1}; var <user-prompt-submit-hook>${EXPR_2}

[output truncated - exceeded ${NUM} characters]<${PATH}> = typeof ${EXPR_3}; if (<user-prompt-submit-hook>${EXPR_4}

[output truncated - exceeded ${NUM} characters]<${PATH}> != 'boolean' && <user-prompt-submit-hook>${EXPR_5}

[output truncated - exceeded ${NUM} characters]<${PATH}> != 'undefined' && <user-prompt-submit-hook>${EXPR_6}

[output truncated - exceeded ${NUM} characters]<${PATH}> != 'number') {
