# System Data Block: 72527206

- Source: inline

## Summary

Claude API — PHP > **Note:** The PHP SDK is the official Anthropic SDK for PHP.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `OPUS_ID` | None | None |

# Raw Prompt Text
# Claude API — PHP

> **Note:** The PHP SDK is the official Anthropic SDK for PHP. Tool runner and Agent SDK are not available. Bedrock, Vertex AI, and Foundry clients are supported.

## Installation

```bash
composer require "anthropic-ai${PATH}"
```

## Client Initialization

```php
use Anthropic\Client;

// Using API key from environment variable
$client = new Client(apiKey: getenv("ANTHROPIC_API_KEY"));
```

### Amazon Bedrock

```php
use Anthropic\BedrockClient;

$client = new BedrockClient(
    region: 'us-east-${NUM}',
);
```

### Google Vertex AI

```php
use Anthropic\VertexClient;

$client = new VertexClient(
    region: 'us-east5',
    projectId: 'my-project-id',
);
```

### Anthropic Foundry

```php
use Anthropic\FoundryClient;

$client = new FoundryClient(
    authToken: getenv("ANTHROPIC_AUTH_TOKEN"),
);
```

---

## Basic Message Request

```php
$message = $client->messages->create(
    model: '{{OPUS_ID}}',
    maxTokens: ${NUM},
    messages: [
        ['role' => 'user', 'content' => 'What is the capital of France?'],
    ],
);
echo $message->content[${NUM}]->text;
```

---

## Streaming

```php
$stream = $client->messages->createStream(
    model: '{{OPUS_ID}}',
    maxTokens: ${NUM},
    messages: [
        ['role' => 'user', 'content' => 'Write a haiku'],
    ],
);

foreach ($stream as $event) {
    echo $event;
}
```

---

## Tool Use (Manual Loop)

The PHP SDK supports raw tool definitions via JSON schema. See the [shared tool use concepts](..${PATH}) for the tool definition format and agentic loop pattern.
