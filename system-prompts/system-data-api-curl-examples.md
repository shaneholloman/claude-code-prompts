# System Data Block: api-curl-examples

- Source: inline

## Summary

Provides raw HTTP cURL examples for basic and streaming Claude message requests.

# Raw Prompt Text
# Claude API — cURL / Raw HTTP

Use these examples when the user needs raw HTTP requests or is working in a language without an official SDK.

## Setup

```bash
export ANTHROPIC_API_KEY="your-api-key"
```

---

## Basic Message Request

```bash
curl ${URL} \
  -H "Content-Type: application${PATH}" \
  -H "x-api-key: $ANTHROPIC_API_KEY" \
  -H "anthropic-version: ${DATE}" \
  -d '{
    "model": "claude-opus-${NUM}-${NUM}",
    "max_tokens": ${NUM},
    "messages": [
      {"role": "user", "content": "What is the capital of France?"}
    ]
  }'
```

---

## Streaming (SSE)

```bash
curl ${URL} \
  -H "Content-Type: application${PATH}" \
  -H "x-api-key: $ANTHROPIC_API_KEY" \
  -H "anthropic-version: ${DATE}" \
  -d '{
    "model": "claude-opus-${NUM}-${NUM}",
    "max_tokens": ${NUM},
    "stream": true,
    "messages": [{"role": "user", "content": "Write a haiku"}]
  }'
```

The response is a stream of Server-Sent Events:

```
event: message_start
data: {"type":"message_start","message":{"id":"msg_...","type":"message",...}}

event: content_block_start
data: {"type":"content_block_start","index":${NUM},"content_block":{"type":"text","text":""}}

event: content_block_delta
data: {"type":"content_block_delta","index":${NUM},"delta":{"type":"text_delta","text":"Hello"}}

event: content_block_stop
data: {"type":"content_block_stop","index":${NUM}}

event: message_delta
data: {"type":"message_delta","delta":{"stop_reason":"end_turn"},"usage":{"output_tokens":${NUM}}}

event: message_stop
data: {"type":"message_stop"}
```

---

## Tool Use

```bash
curl ${URL} \
  -H "Content-Type: application${PATH}" \
  -H "x-api-key: $ANTHROPIC_API_KEY" \
  -H "anthropic-version: ${DATE}" \
  -d '{
    "model": "claude-opus-${NUM}-${NUM}",
    "max_tokens": ${NUM},
    "tools": [{
      "name": "get_weather",
      "description": "Get current weather for a location",
      "input_schema": {
        "type": "object",
        "properties": {
          "location": {"type": "string", "description": "City name"}
        },
        "required": ["location"]
      }
    }],
    "messages": [{"role": "user", "content": "What is the weather in Paris?"}]
  }'
```

When Claude responds with a `tool_use` block, send the result back:

```bash
curl ${URL} \
  -H "Content-Type: application${PATH}" \
  -H "x-api-key: $ANTHROPIC_API_KEY" \
  -H "anthropic-version: ${DATE}" \
  -d '{
    "model": "claude-opus-${NUM}-${NUM}",
    "max_tokens": ${NUM},
    "tools": [{
      "name": "get_weather",
      "description": "Get current weather for a location",
      "input_schema": {
        "type": "object",
        "properties": {
          "location": {"type": "string", "description": "City name"}
        },
        "required": ["location"]
      }
    }],
    "messages": [
      {"role": "user", "content": "What is the weather in Paris?"},
      {"role": "assistant", "content": [
        {"type": "text", "text": "Let me check the weather."},
        {"type": "tool_use", "id": "toolu_abc123", "name": "get_weather", "input": {"location": "Paris"}}
      ]},
      {"role": "user", "content": [
        {"type": "tool_result", "tool_use_id": "toolu_abc123", "content": "${NUM}°F and sunny"}
      ]}
    ]
  }'
```

---

## Extended Thinking

> **Opus ${NUM} and Sonnet ${NUM}:** Use adaptive thinking. `budget_tokens` is deprecated on both Opus ${NUM} and Sonnet ${NUM}.
> **Older models:** Use `"type": "enabled"` with `"budget_tokens": N` (must be < `max_tokens`, min ${NUM}).

```bash
# Opus ${NUM}: adaptive thinking (recommended)
curl ${URL} \
  -H "Content-Type: application${PATH}" \
  -H "x-api-key: $ANTHROPIC_API_KEY" \
  -H "anthropic-version: ${DATE}" \
  -d '{
    "model": "claude-opus-${NUM}-${NUM}",
    "max_tokens": ${NUM},
    "thinking": {
      "type": "adaptive"
    },
    "output_config": {
      "effort": "high"
    },
    "messages": [{"role": "user", "content": "Solve this step by step..."}]
  }'
```

---

## Required Headers

| Header              | Value              | Description                |
| ------------------- | ------------------ | -------------------------- |
| `Content-Type`      | `application${PATH}` | Required                   |
| `x-api-key`         | Your API key       | Authentication             |
| `anthropic-version` | `${DATE}`       | API version                |
| `anthropic-beta`    | Beta feature IDs   | Required for beta features |
