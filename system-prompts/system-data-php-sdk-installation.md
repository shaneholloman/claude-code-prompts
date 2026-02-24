# System Data Block: php-sdk-installation

- Source: inline

## Summary

Installation and usage of the PHP SDK for Claude.

# Raw Prompt Text
# Claude API — PHP

> **Note:** The PHP SDK is the official Anthropic SDK for PHP. Tool runner and Agent SDK are not available.

## Installation

```bash
composer require "anthropic-ai${PATH} ${NUM}.${NUM}"
```

## Client Initialization

```php
use Anthropic\Client;

// Using API key from environment variable
$client = new Client(apiKey: getenv("ANTHROPIC_API_KEY"));
```

---

## Basic Message Request

```php
$message = $client->messages->create(
    model: 'claude-opus-${NUM}-${NUM}',
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
    model: 'claude-opus-${NUM}-${NUM}',
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
