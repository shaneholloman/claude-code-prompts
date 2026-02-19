# System Prompt: verrors-array-push-snippet

- Source: inline

## Summary

JavaScript builds err from submit-hook expression, pushes into vErrors, increments errors counter.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
var err = <user-prompt-submit-hook>${EXPR_1}

[output truncated - exceeded ${NUM} characters]<${PATH}>;  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++;
