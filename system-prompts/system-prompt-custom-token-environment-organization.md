# System Prompt: custom-token-environment-organization

- Source: inline

## Summary

Instructions for managing OAuth token settings.

# Raw Prompt Text
The CLAUDE_CODE_OAUTH_TOKEN_FILE_DESCRIPTOR environment variable provides a token for a
different organization than required by this machine's managed settings.

Required: ${EXPR_1}
Token organization: ## allow (custom rules replacing defaults)
Custom:
${EXPR_2}

Defaults being replaced:
${EXPR_3}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_4}

Defaults being replaced:
${EXPR_5}

## environment (custom rules replacing defaults)
Custom:
${EXPR_6}

Defaults being replaced:
${EXPR_7}



Remove the environment variable or obtain a token for a permitted organization.
