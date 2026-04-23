# System Prompt: http-error-codes-reference-2

- Source: native-reference-match

## Summary

System Prompt: http-error-codes-reference-… - Source: native-reference-match Summary System Prompt: http-error-codes-reference-… - Source: inline Summary Doc…

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
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |
| `OPUS_ID` | None | None |
| `EXPR_18` | None | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | None | None |
| `EXPR_22` | None | None |
| `EXPR_23` | None | None |

# Raw Prompt Text
# System Prompt: http-error-codes-reference-${NUM}

- Source: native-reference-match

## Summary

System Prompt: http-error-codes-reference-… - Source: inline Summary Documentation of HTTP error codes for Claude API.

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
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `OPUS_ID` | None | None |
| `EXPR_17` | None | None |
| `EXPR_18` | None | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | None | None |
| `EXPR_22` | None | None |
| `EXPR_23` | None | None |

# Raw Prompt Text
# System Prompt: http-error-codes-reference-${EXPR_1}

- Source: inline

## Summary

Documentation of HTTP error codes for Claude API.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `OPUS_ID` | None | None |
| `EXPR_1` | None | None |

# Raw Prompt Text
# HTTP Error Codes Reference

This file documents HTTP error codes returned by the Claude API, their common causes, and how to handle them. For language-specific error handling examples, see the `python/` or `typescript/` folders.

## Error Code Summary

| Code | Error Type              | Retryable | Common Cause                         |
| ---- | ----------------------- | --------- | ------------------------------------ |
| ${EXPR_2}  | `invalid_request_error` | No        | Invalid request format or parameters |
| ${EXPR_3}  | `authentication_error`  | No        | Invalid or missing API key           |
| ${EXPR_4}  | `permission_error`      | No        | API key lacks permission             |
| ${EXPR_5}  | `not_found_error`       | No        | Invalid endpoint or model ID         |
| ${EXPR_6}  | `request_too_large`     | No        | Request exceeds size limits          |
| ${EXPR_7}  | `rate_limit_error`      | Yes       | Too many requests                    |
| ${EXPR_8}  | `api_error`             | Yes       | Anthropic service issue              |
| ${EXPR_9}  | `overloaded_error`      | Yes       | API is temporarily overloaded        |

## Detailed Error Information

### ${EXPR_10} Bad Request

**Causes:**

- Malformed JSON in request body
- Missing required parameters (`model`, `max_tokens`, `messages`)
- Invalid parameter types (e.g., string where integer expected)
- Empty messages array
- Messages not alternating user${EXPR_11}

**Example error:**

```json
{
  "type": "error",
  "error": {
    "type": "invalid_request_error",
    "message": "messages: roles must alternate between \"user\" and \"assistant\""
  },
  "request_id": "req_011CSHoEeqs5C35K2UUqR7Fy"
}
```

**Fix:** Validate request structure before sending. Check that:

- `model` is a valid model ID
- `max_tokens` is a positive integer
- `messages` array is non-empty and alternates correctly

---

### ${EXPR_12} Unauthorized

**Causes:**

- Missing `x-api-key` header or `Authorization` header
- Invalid API key format
- Revoked or deleted API key

**Fix:** Ensure `ANTHROPIC_API_KEY` environment variable is set correctly.

---

### ${EXPR_13} Forbidden

**Causes:**

- API key doesn't have access to the requested model
- Organization-level restrictions
- Attempting to access beta features without beta access

**Fix:** Check your API key permissions in the Console. You may need a different API key or to request access to specific features.

---

### ${EXPR_14} Not Found

**Causes:**

- Typo in model ID (e.g., `claude-sonnet-${EXPR_15}` instead of `claude-sonnet-${EXPR_16}-${EXPR_17}`)
- Using deprecated model ID
- Invalid API endpoint

**Fix:** Use exact model IDs from the models documentation. You can use aliases (e.g., `{{OPUS_ID}}`).

---

### ${EXPR_18} Request Too Large

**Causes:**

- Request body exceeds maximum size
- Too many tokens in input
- Image data too large

**Fix:** Reduce input size — truncate conversation history, compress${EXPR_19} images, or split large documents into chunks.

---

### ${EXPR_20} Validation Errors

Some ${EXPR_21} errors are specifically related to parameter validation:

- `max_tokens` exceeds model's limit
- Invalid `temperature` value (must be ${EXPR_22}-${EXPR_23})
- `budget_tokens` >= `max_tokens` in extended thinking
- Invalid tool definition schema

**Model-specific 400s on Opus ${EXPR_24}:**

- `temperature`, `top_p`, `top_k` are removed — sending any of them returns ${EXPR_25}. Delete the parameter; see `shared${EXPR_26}` → Per-SDK Syntax Reference.
- `thinking: {type: "enabled", budget_tokens: N}` is removed — sending it returns ${EXPR_27}. Use `thinking: {type: "adaptive"}` instead.

**Common mistake with extended thinking on older models (Opus ${EXPR_28} and earlier):**

```
# Wrong: budget_tokens must be < max_tokens
thinking: budget_tokens=${EXPR_29}, max_tokens=${EXPR_30}  → Error!

# Correct
thinking: budget_tokens=${EXPR_31}, max_tokens=${EXPR_32}
```

---

### ${EXPR_33} Rate Limited

**Causes:**

- Exceeded requests per minute (RPM)
- Exceeded tokens per minute (TPM)
- Exceeded tokens per day (TPD)

**Headers to check:**

- `retry-after`: Seconds to wait before retrying
- `x-ratelimit-limit-*`: Your limits
- `x-ratelimit-remaining-*`: Remaining quota

**Fix:** The Anthropic SDKs automatically retry ${EXPR_34} and 5xx errors with exponential backoff (default: `max_retries=${EXPR_35}`). For custom retry behavior, see the language-specific error handling examples.

---

### ${EXPR_36} Internal Server Error

**Causes:**

- Temporary Anthropic service issue
- Bug in API processing

**Fix:** Retry with exponential backoff. If persistent, check [status.anthropic.com](${EXPR_37}).

---

### ${EXPR_38} Overloaded

**Causes:**

- High API demand
- Service capacity reached

**Fix:** Retry with exponential backoff. Consider using a different model (Haiku is often less loaded), spreading requests over time, or implementing request queuing.

---

## Common Mistakes and Fixes

| Mistake                         | Error            | Fix                                                     |
| ------------------------------- | ---------------- | ------------------------------------------------------- |
| `temperature`/`top_p`/`top_k` on Opus ${EXPR_39} | ${EXPR_40}    | Remove the parameter (see `shared${EXPR_41}`)  |
| `budget_tokens` on Opus ${EXPR_42}     | ${EXPR_43}              | Use `thinking: {type: "adaptive"}`                      |
| `budget_tokens` >= `max_tokens` (older models) | ${EXPR_44} | Ensure `budget_tokens` < `max_tokens`                  |
| Typo in model ID                | ${EXPR_45}              | Use valid model ID like `{{OPUS_ID}}`               |
| First message is `assistant`    | ${EXPR_46}              | First message must be `user`                            |
| Consecutive same-role messages  | ${EXPR_47}              | Alternate `user` and `assistant`                        |
| API key in code                 | ${EXPR_48} (leaked key) | Use environment variable                                |
| Custom retry needs              | ${EXPR_49}${EXPR_50}          | SDK retries automatically; customize with `max_retries` |

## Typed Exceptions in SDKs

**Always use the SDK's typed exception classes** instead of checking error messages with string matching. Each HTTP error code maps to a specific exception class:

| HTTP Code | TypeScript Class                  | Python Class                      |
| --------- | --------------------------------- | --------------------------------- |
| ${EXPR_51}       | `Anthropic.BadRequestError`       | `anthropic.BadRequestError`       |
| ${EXPR_52}       | `Anthropic.AuthenticationError`   | `anthropic.AuthenticationError`   |
| ${EXPR_53}       | `Anthropic.PermissionDeniedError` | `anthropic.PermissionDeniedError` |
| ${EXPR_54}       | `Anthropic.NotFoundError`         | `anthropic.NotFoundError`         |
| ${EXPR_55}       | `Anthropic.RateLimitError`        | `anthropic.RateLimitError`        |
| ${EXPR_56}+      | `Anthropic.InternalServerError`   | `anthropic.InternalServerError`   |
| Any       | `Anthropic.APIError`              | `anthropic.APIError`              |

```typescript
// ✅ Correct: use typed exceptions
try {
  const response = await client.messages.create({...});
} catch (error) {
  if (error instanceof Anthropic.RateLimitError) {
    // Handle rate limiting
  } else if (error instanceof Anthropic.APIError) {
    console.error(`API error ${EXPR_57}:`, error.message);
  }
}

// ❌ Wrong: don't check error messages with string matching
try {
  const response = await client.messages.create({...});
} catch (error) {
  const msg = error instanceof Error ? error.message : String(error);
  if (msg.includes("${EXPR_58}") || msg.includes("rate_limit")) { ... }
}
```

All exception classes extend `Anthropic.APIError`, which has a `status` property. Use `instanceof` checks from most specific to least specific (e.g., check `RateLimitError` before `APIError`).
