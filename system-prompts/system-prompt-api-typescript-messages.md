# System Prompt: api-typescript-messages

- Source: inline

## Summary

Shows TypeScript SDK installation, client setup, and basic messages with system prompts.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
# Claude API — TypeScript

## Installation

```bash
npm install @anthropic-ai${PATH}
```

## Client Initialization

```typescript
import Anthropic from "@anthropic-ai${PATH}";

// Default (uses ANTHROPIC_API_KEY env var)
const client = new Anthropic();

// Explicit API key
const client = new Anthropic({ apiKey: "your-api-key" });
```

---

## Basic Message Request

```typescript
const response = await client.messages.create({
  model: "claude-opus-${NUM}-${NUM}",
  max_tokens: ${NUM},
  messages: [{ role: "user", content: "What is the capital of France?" }],
});
console.log(response.content[${NUM}].text);
```

---

## System Prompts

```typescript
const response = await client.messages.create({
  model: "claude-opus-${NUM}-${NUM}",
  max_tokens: ${NUM},
  system:
    "You are a helpful coding assistant. Always provide examples in Python.",
  messages: [{ role: "user", content: "How do I read a JSON file?" }],
});
```

---

## Vision (Images)

### URL

```typescript
const response = await client.messages.create({
  model: "claude-opus-${NUM}-${NUM}",
  max_tokens: ${NUM},
  messages: [
    {
      role: "user",
      content: [
        {
          type: "image",
          source: { type: "url", url: "${URL} },
        },
        { type: "text", text: "Describe this image" },
      ],
    },
  ],
});
```

### Base64

```typescript
import fs from "fs";

const imageData = fs.readFileSync("image.png").toString("base64");

const response = await client.messages.create({
  model: "claude-opus-${NUM}-${NUM}",
  max_tokens: ${NUM},
  messages: [
    {
      role: "user",
      content: [
        {
          type: "image",
          source: { type: "base64", media_type: "image${PATH}", data: imageData },
        },
        { type: "text", text: "What's in this image?" },
      ],
    },
  ],
});
```

---

## Prompt Caching

```typescript
const response = await client.messages.create({
  model: "claude-opus-${NUM}-${NUM}",
  max_tokens: ${NUM},
  system: [
    {
      type: "text",
      text: "You are an expert on this large document...",
      cache_control: { type: "ephemeral" },
    },
  ],
  messages: [{ role: "user", content: "Summarize the key points" }],
});
```

---

## Extended Thinking

> **Opus ${NUM}:** Use adaptive thinking. `budget_tokens` is deprecated on Opus ${NUM}.
> **Older models:** Use `thinking: {type: "enabled", budget_tokens: N}` (must be < `max_tokens`, min ${NUM}).

```typescript
// Opus ${NUM}: adaptive thinking (recommended)
const response = await client.messages.create({
  model: "claude-opus-${NUM}-${NUM}",
  max_tokens: ${NUM},
  thinking: { type: "adaptive" },
  output_config: { effort: "high" }, // low | medium | high (default) | max
  messages: [
    { role: "user", content: "Solve this math problem step by step..." },
  ],
});

for (const block of response.content) {
  if (block.type === "thinking") {
    console.log("Thinking:", block.thinking);
  } else if (block.type === "text") {
    console.log("Response:", block.text);
  }
}
```

---

## Error Handling

```typescript
import Anthropic from "@anthropic-ai${PATH}";

try {
  const response = await client.messages.create({...});
} catch (error) {
  if (error instanceof Anthropic.BadRequestError) {
    console.error("Bad request:", error.message);
  } else if (error instanceof Anthropic.AuthenticationError) {
    console.error("Invalid API key");
  } else if (error instanceof Anthropic.RateLimitError) {
    console.error("Rate limited - retry later");
  } else if (error instanceof Anthropic.APIError) {
    console.error(`API error ${EXPR_1}:`, error.message);
  }
}
```

---

## Multi-Turn Conversations

The API is stateless — send the full conversation history each time.

```typescript
const messages = [
  { role: "user", content: "My name is Alice." },
  { role: "assistant", content: "Hello Alice! Nice to meet you." },
  { role: "user", content: "What's my name?" },
];

const response = await client.messages.create({
  model: "claude-opus-${NUM}-${NUM}",
  max_tokens: ${NUM},
  messages: messages,
});
```

**Rules:**

- Messages must alternate between `user` and `assistant`
- First message must be `user`

---

### Compaction (long conversations)

> **Beta, Opus ${NUM} only.** When conversations approach the 200K context window, compaction automatically summarizes earlier context server-side. The API returns a `compaction` block; you must pass it back on subsequent requests — append `response.content`, not just the text.

```typescript
import Anthropic from "@anthropic-ai${PATH}";

const client = new Anthropic();
const messages: Anthropic.Beta.BetaMessageParam[] = [];

async function chat(userMessage: string): Promise<string> {
  messages.push({ role: "user", content: userMessage });

  const response = await client.beta.messages.create({
    betas: ["compact-${DATE}"],
    model: "claude-opus-${NUM}-${NUM}",
    max_tokens: ${NUM},
    messages,
    context_management: {
      edits: [{ type: "compact_20260112" }],
    },
  });

  // Append full content — compaction blocks must be preserved
  messages.push({ role: "assistant", content: response.content });

  const textBlock = response.content.find((block) => block.type === "text");
  return textBlock?.text ?? "";
}

// Compaction triggers automatically when context grows large
console.log(await chat("Help me build a Python web scraper"));
console.log(await chat("Add support for JavaScript-rendered pages"));
console.log(await chat("Now add rate limiting and error handling"));
```

---

## Cost Optimization Strategies

### ${NUM}. Use Prompt Caching for Repeated Context

```typescript
const systemWithCache = [
  {
    type: "text",
    text: largeDocumentText, // e.g., 50KB of context
    cache_control: { type: "ephemeral" },
  },
];

// First request: full cost
// Subsequent requests: ~${NUM}% cheaper for cached portion
```

### ${NUM}. Use Token Counting Before Requests

```typescript
const countResponse = await client.messages.countTokens({
  model: "claude-opus-${NUM}-${NUM}",
  messages: messages,
  system: system,
});

const estimatedInputCost = countResponse.input_tokens * ${NUM}; // $${NUM}/1M tokens
console.log(`Estimated input cost: $${EXPR_2}`);
```
