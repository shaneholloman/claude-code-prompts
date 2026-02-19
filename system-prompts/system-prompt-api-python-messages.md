# System Prompt: api-python-messages

- Source: inline

## Summary

Python SDK quickstart showing Anthropic client setup, message requests, system prompts, and vision examples.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
# Claude API — Python

## Installation

```bash
pip install anthropic
```

## Client Initialization

```python
import anthropic

# Default (uses ANTHROPIC_API_KEY env var)
client = anthropic.Anthropic()

# Explicit API key
client = anthropic.Anthropic(api_key="your-api-key")

# Async client
async_client = anthropic.AsyncAnthropic()
```

---

## Basic Message Request

```python
response = client.messages.create(
    model="claude-opus-${NUM}-${NUM}",
    max_tokens=${NUM},
    messages=[
        {"role": "user", "content": "What is the capital of France?"}
    ]
)
print(response.content[${NUM}].text)
```

---

## System Prompts

```python
response = client.messages.create(
    model="claude-opus-${NUM}-${NUM}",
    max_tokens=${NUM},
    system="You are a helpful coding assistant. Always provide examples in Python.",
    messages=[{"role": "user", "content": "How do I read a JSON file?"}]
)
```

---

## Vision (Images)

### Base64

```python
import base64

with open("image.png", "rb") as f:
    image_data = base64.standard_b64encode(f.read()).decode("utf-${NUM}")

response = client.messages.create(
    model="claude-opus-${NUM}-${NUM}",
    max_tokens=${NUM},
    messages=[{
        "role": "user",
        "content": [
            {
                "type": "image",
                "source": {
                    "type": "base64",
                    "media_type": "image${PATH}",
                    "data": image_data
                }
            },
            {"type": "text", "text": "What's in this image?"}
        ]
    }]
)
```

### URL

```python
response = client.messages.create(
    model="claude-opus-${NUM}-${NUM}",
    max_tokens=${NUM},
    messages=[{
        "role": "user",
        "content": [
            {
                "type": "image",
                "source": {
                    "type": "url",
                    "url": "${URL}
                }
            },
            {"type": "text", "text": "Describe this image"}
        ]
    }]
)
```

---

## Prompt Caching

Cache large context to reduce costs (up to ${NUM}% savings).

```python
response = client.messages.create(
    model="claude-opus-${NUM}-${NUM}",
    max_tokens=${NUM},
    system=[{
        "type": "text",
        "text": "You are an expert on this large document...",
        "cache_control": {"type": "ephemeral"}
    }],
    messages=[{"role": "user", "content": "Summarize the key points"}]
)
```

---

## Extended Thinking

> **Opus ${NUM}:** Use adaptive thinking. `budget_tokens` is deprecated on Opus ${NUM}.
> **Older models:** Use `thinking: {type: "enabled", budget_tokens: N}` (must be < `max_tokens`, min ${NUM}).

```python
# Opus ${NUM}: adaptive thinking (recommended)
response = client.messages.create(
    model="claude-opus-${NUM}-${NUM}",
    max_tokens=${NUM},
    thinking={"type": "adaptive"},
    output_config={"effort": "high"},  # low | medium | high (default) | max
    messages=[{"role": "user", "content": "Solve this step by step..."}]
)

# Access thinking and response
for block in response.content:
    if block.type == "thinking":
        print(f"Thinking: {block.thinking}")
    elif block.type == "text":
        print(f"Response: {block.text}")
```

---

## Error Handling

```python
import anthropic

try:
    response = client.messages.create(...)
except anthropic.BadRequestError as e:
    print(f"Bad request: {e.message}")
except anthropic.AuthenticationError:
    print("Invalid API key")
except anthropic.PermissionDeniedError:
    print("API key lacks required permissions")
except anthropic.NotFoundError:
    print("Invalid model or endpoint")
except anthropic.RateLimitError as e:
    retry_after = getattr(e, "retry_after", ${NUM})
    print(f"Rate limited. Retry after {retry_after}s.")
except anthropic.APIStatusError as e:
    if e.status_code >= ${NUM}:
        print(f"Server error ({e.status_code}). Retry later.")
    else:
        print(f"API error: {e.message}")
except anthropic.APIConnectionError:
    print("Network error. Check internet connection.")
```

---

## Multi-Turn Conversations

The API is stateless — send the full conversation history each time.

```python
class ConversationManager:
    """Manage multi-turn conversations with the Claude API."""

    def __init__(self, client: anthropic.Anthropic, model: str, system: str = None):
        self.client = client
        self.model = model
        self.system = system
        self.messages = []

    def send(self, user_message: str, **kwargs) -> str:
        """Send a message and get a response."""
        self.messages.append({"role": "user", "content": user_message})

        response = self.client.messages.create(
            model=self.model,
            max_tokens=kwargs.get("max_tokens", ${NUM}),
            system=self.system,
            messages=self.messages,
            **kwargs
        )

        assistant_message = response.content[${NUM}].text
        self.messages.append({"role": "assistant", "content": assistant_message})

        return assistant_message

# Usage
conversation = ConversationManager(
    client=anthropic.Anthropic(),
    model="claude-opus-${NUM}-${NUM}",
    system="You are a helpful assistant."
)

response1 = conversation.send("My name is Alice.")
response2 = conversation.send("What's my name?")  # Claude remembers "Alice"
```

**Rules:**

- Messages must alternate between `user` and `assistant`
- First message must be `user`

---

### Compaction (long conversations)

> **Beta, Opus ${NUM} only.** When conversations approach the 200K context window, compaction automatically summarizes earlier context server-side. The API returns a `compaction` block; you must pass it back on subsequent requests — append `response.content`, not just the text.

```python
import anthropic

client = anthropic.Anthropic()
messages = []

def chat(user_message: str) -> str:
    messages.append({"role": "user", "content": user_message})

    response = client.beta.messages.create(
        betas=["compact-${DATE}"],
        model="claude-opus-${NUM}-${NUM}",
        max_tokens=${NUM},
        messages=messages,
        context_management={
            "edits": [{"type": "compact_20260112"}]
        }
    )

    # Append full content — compaction blocks must be preserved
    messages.append({"role": "assistant", "content": response.content})

    return next(block.text for block in response.content if block.type == "text")

# Compaction triggers automatically when context grows large
print(chat("Help me build a Python web scraper"))
print(chat("Add support for JavaScript-rendered pages"))
print(chat("Now add rate limiting and error handling"))
```

---

## Cost Optimization Strategies

### ${NUM}. Use Prompt Caching for Repeated Context

```python
# Cache large system prompts or documents
system_with_cache = [{
    "type": "text",
    "text": large_document_text,  # e.g., 50KB of context
    "cache_control": {"type": "ephemeral"}
}]

# First request: full cost
# Subsequent requests: ~${NUM}% cheaper for cached portion
```

### ${NUM}. Choose the Right Model

```python
# Default to Opus for most tasks
response = client.messages.create(
    model="claude-opus-${NUM}-${NUM}",  # $${NUM}/$${NUM} per 1M tokens
    max_tokens=${NUM},
    messages=[{"role": "user", "content": "Explain quantum computing"}]
)

# Use Sonnet for high-volume production workloads
standard_response = client.messages.create(
    model="claude-sonnet-${NUM}-${NUM}",  # $${NUM}/$${NUM} per 1M tokens
    max_tokens=${NUM},
    messages=[{"role": "user", "content": "Summarize this document"}]
)

# Use Haiku only for simple, speed-critical tasks
simple_response = client.messages.create(
    model="claude-haiku-${NUM}-${NUM}",  # $${NUM}/$${NUM} per 1M tokens
    max_tokens=${NUM},
    messages=[{"role": "user", "content": "Classify this as positive or negative"}]
)
```

### ${NUM}. Use Token Counting Before Requests

```python
count_response = client.messages.count_tokens(
    model="claude-opus-${NUM}-${NUM}",
    messages=messages,
    system=system
)

estimated_input_cost = count_response.input_tokens * ${NUM}  # $${NUM}/1M tokens
print(f"Estimated input cost: ${EXPR_1}")
```

---

## Retry with Exponential Backoff

> **Note:** The Anthropic SDK automatically retries rate limit (${NUM}) and server errors (5xx) with exponential backoff. You can configure this with `max_retries` (default: ${NUM}). Only implement custom retry logic if you need behavior beyond what the SDK provides.

```python
import time
import random
import anthropic

def call_with_retry(
    client: anthropic.Anthropic,
    max_retries: int = ${NUM},
    base_delay: float = ${NUM},
    max_delay: float = ${NUM},
    **kwargs
):
    """Call the API with exponential backoff retry."""
    last_exception = None

    for attempt in range(max_retries):
        try:
            return client.messages.create(**kwargs)
        except anthropic.RateLimitError as e:
            last_exception = e
        except anthropic.APIStatusError as e:
            if e.status_code >= ${NUM}:
                last_exception = e
            else:
                raise  # Client errors (4xx except ${NUM}) should not be retried

        delay = min(base_delay * (${NUM} ** attempt) + random.uniform(${NUM}, ${NUM}), max_delay)
        print(f"Retry {attempt + ${NUM}}/{max_retries} after {delay:.1f}s")
        time.sleep(delay)

    raise last_exception
```
