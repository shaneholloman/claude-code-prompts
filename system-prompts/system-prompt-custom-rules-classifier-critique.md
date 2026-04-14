# System Prompt: custom-rules-classifier-critique

- Source: inline

## Summary

Critique of user-defined classifier rules.

# Raw Prompt Text
Here is the full classifier system prompt that the auto mode classifier receives:

<classifier_system_prompt>
npm view ${EXPR_1}@${EXPR_2} version
<${PATH}>

Here are the user's custom rules that REPLACE the corresponding default sections:

## allow (custom rules replacing defaults)
Custom:
${EXPR_3}

Defaults being replaced:
${EXPR_4}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_5}

Defaults being replaced:
${EXPR_6}

## environment (custom rules replacing defaults)
Custom:
${EXPR_7}

Defaults being replaced:
${EXPR_8}


Please critique these custom rules.
