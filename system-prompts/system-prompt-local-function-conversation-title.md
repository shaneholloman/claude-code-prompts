# System Prompt: local-function-conversation-title

- Source: inline

## Summary

Inside a wrapper function, output only a …-… word conversation title.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
function local(${URL}){
  Please write a ${NUM}-${NUM} word title the following conversation:

${EXPR_1}

  Respond with the title for the conversation and nothing else.
}
