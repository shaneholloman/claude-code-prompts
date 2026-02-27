# System Data Block: 5f7d3481

- Source: inline

## Summary

Covers Go SDK installation, client initialization, and basic messages requests with notes on tool use.

# Raw Prompt Text
# Claude API — Go

> **Note:** The Go SDK supports the Claude API. Tool runner and Agent SDK are not yet available for Go — use the manual agentic loop for tool use.

## Installation

```bash
go get github.com${PATH}
```

## Client Initialization

```go
import (
    "github.com${PATH}"
    "github.com${PATH}"
)

// Default (uses ANTHROPIC_API_KEY env var)
client := anthropic.NewClient()

// Explicit API key
client := anthropic.NewClient(
    option.WithAPIKey("your-api-key"),
)
```

---

## Basic Message Request

```go
response, err := client.Messages.New(context.TODO(), anthropic.MessageNewParams{
    Model:     anthropic.ModelClaudeOpus4_6,
    MaxTokens: ${NUM},
    Messages: []anthropic.MessageParam{
        anthropic.NewUserMessage(anthropic.NewTextBlock("What is the capital of France?")),
    },
})
if err != nil {
    log.Fatal(err)
}
fmt.Println(response.Content[${NUM}].Text)
```

---

## Streaming

```go
stream := client.Messages.NewStreaming(context.TODO(), anthropic.MessageNewParams{
    Model:     anthropic.ModelClaudeOpus4_6,
    MaxTokens: ${NUM},
    Messages: []anthropic.MessageParam{
        anthropic.NewUserMessage(anthropic.NewTextBlock("Write a haiku")),
    },
})

for stream.Next() {
    event := stream.Current()
    switch eventVariant := event.AsAny().(type) {
    case anthropic.ContentBlockDeltaEvent:
        switch deltaVariant := eventVariant.Delta.AsAny().(type) {
        case anthropic.TextDelta:
            fmt.Print(deltaVariant.Text)
        }
    }
}
if err := stream.Err(); err != nil {
    log.Fatal(err)
}
```

---

## Tool Use (Manual Loop)

The Go SDK supports raw tool definitions via JSON schema. See the [shared tool use concepts](..${PATH}) for the tool definition format and agentic loop pattern.
