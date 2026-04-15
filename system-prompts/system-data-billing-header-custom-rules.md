# System Data Block: billing-header-custom-rules

- Source: inline

## Summary

Custom rules are used to replace default settings.

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

# Raw Prompt Text
x-anthropic-billing-header: cc_version=${EXPR_1}; cc_entrypoint=${EXPR_2};stable## allow (custom rules replacing defaults)
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
