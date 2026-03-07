# System Prompt: 0db311fc

- Source: inline

## Summary

Claude API — Go > **Note:** The Go SDK supports the Claude API and beta tool use with `BetaToolRunner`.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `OfTool_addTool` | None | None |

# Raw Prompt Text
# Claude API — Go

> **Note:** The Go SDK supports the Claude API and beta tool use with `BetaToolRunner`. Agent SDK is not yet available for Go.

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
response, err := client.Messages.New(context.Background(), anthropic.MessageNewParams{
    Model:     anthropic.ModelClaudeOpus4_6,
    MaxTokens: ${NUM},
    Messages: []anthropic.MessageParam{
        anthropic.NewUserMessage(anthropic.NewTextBlock("What is the capital of France?")),
    },
})
if err != nil {
    log.Fatal(err)
}
for _, block := range response.Content {
    switch variant := block.AsAny().(type) {
    case anthropic.TextBlock:
        fmt.Println(variant.Text)
    }
}
```

---

## Streaming

```go
stream := client.Messages.NewStreaming(context.Background(), anthropic.MessageNewParams{
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

## Tool Use

### Tool Runner (Beta — Recommended)

**Beta:** The Go SDK provides `BetaToolRunner` for automatic tool use loops via the `toolrunner` package.

```go
import (
    "context"
    "fmt"
    "log"

    "github.com${PATH}"
    "github.com${PATH}"
)

// Define tool input with jsonschema tags for automatic schema generation
type GetWeatherInput struct {
    City string `json:"city" jsonschema:"required,description=The city name"`
}

// Create a tool with automatic schema generation from struct tags
weatherTool, err := toolrunner.NewBetaToolFromJSONSchema(
    "get_weather",
    "Get current weather for a city",
    func(ctx context.Context, input GetWeatherInput) (anthropic.BetaToolResultBlockParamContentUnion, error) {
        return anthropic.BetaToolResultBlockParamContentUnion{
            OfText: &anthropic.BetaTextBlockParam{
                Text: fmt.Sprintf("The weather in %s is sunny, ${NUM}°F", input.City),
            },
        }, nil
    },
)
if err != nil {
    log.Fatal(err)
}

// Create a tool runner that handles the conversation loop automatically
runner := client.Beta.Messages.NewToolRunner(
    []anthropic.BetaTool{weatherTool},
    anthropic.BetaToolRunnerParams{
        BetaMessageNewParams: anthropic.BetaMessageNewParams{
            Model:     anthropic.ModelClaudeOpus4_6,
            MaxTokens: ${NUM},
            Messages: []anthropic.BetaMessageParam{
                anthropic.NewBetaUserMessage(anthropic.NewBetaTextBlock("What's the weather in Paris?")),
            },
        },
        MaxIterations: ${NUM},
    },
)

// Run until Claude produces a final response
message, err := runner.RunToCompletion(context.Background())
if err != nil {
    log.Fatal(err)
}
fmt.Println(message.Content[${NUM}].Text)
```

**Key features of the Go tool runner:**

- Automatic schema generation from Go structs via `jsonschema` tags
- `RunToCompletion()` for simple one-shot usage
- `All()` iterator for processing each message in the conversation
- `NextMessage()` for step-by-step iteration
- Streaming variant via `NewToolRunnerStreaming()` with `AllStreaming()`

### Manual Loop

For fine-grained control over the agentic loop, define tools with `ToolParam`, check `StopReason`, execute tools yourself, and feed `tool_result` blocks back. This is the pattern when you need to intercept, validate, or log tool calls.

Derived from `anthropic-sdk-go${PATH}`.

```go
package main

import (
    "context"
    "encoding${PATH}"
    "fmt"
    "log"

    "github.com${PATH}"
)

func main() {
    client := anthropic.NewClient()

    // ${NUM}. Define tools. ToolParam.InputSchema uses a map, no struct tags needed.
    addTool := anthropic.ToolParam{
        Name:        "add",
        Description: anthropic.String("Add two integers"),
        InputSchema: anthropic.ToolInputSchemaParam{
            Properties: map[string]any{
                "a": map[string]any{"type": "integer"},
                "b": map[string]any{"type": "integer"},
            },
        },
    }
    // ToolParam must be wrapped in ToolUnionParam for the Tools slice
    tools := []anthropic.ToolUnionParam{{OfTool: &addTool}}

    messages := []anthropic.MessageParam{
        anthropic.NewUserMessage(anthropic.NewTextBlock("What is ${NUM} + ${NUM}?")),
    }

    for {
        resp, err := client.Messages.New(context.Background(), anthropic.MessageNewParams{
            Model:     anthropic.ModelClaudeSonnet4_6,
            MaxTokens: ${NUM},
            Messages:  messages,
            Tools:     tools,
        })
        if err != nil {
            log.Fatal(err)
        }

        // ${NUM}. Append the assistant response to history BEFORE processing tool calls.
        //    resp.ToParam() converts Message → MessageParam in one call.
        messages = append(messages, resp.ToParam())

        // ${NUM}. Walk content blocks. ContentBlockUnion is a flattened struct;
        //    use block.AsAny().(type) to switch on the actual variant.
        toolResults := []anthropic.ContentBlockParamUnion{}
        for _, block := range resp.Content {
            switch variant := block.AsAny().(type) {
            case anthropic.TextBlock:
                fmt.Println(variant.Text)
            case anthropic.ToolUseBlock:
                // ${NUM}. Parse the tool input. Use variant.JSON.Input.Raw() to get the
                //    raw JSON — block.Input is json.RawMessage, not the parsed value.
                var in struct {
                    A int `json:"a"`
                    B int `json:"b"`
                }
                if err := json.Unmarshal([]byte(variant.JSON.Input.Raw()), &in); err != nil {
                    log.Fatal(err)
                }
                result := fmt.Sprintf("%d", in.A+in.B)
                // ${NUM}. NewToolResultBlock(toolUseID, content, isError) builds the
                //    ContentBlockParamUnion for you. block.ID is the tool_use_id.
                toolResults = append(toolResults,
                    anthropic.NewToolResultBlock(block.ID, result, false))
            }
        }

        // ${NUM}. Exit when Claude stops asking for tools
        if resp.StopReason != anthropic.StopReasonToolUse {
            break
        }

        // ${NUM}. Tool results go in a user message (variadic: all results in one turn)
        messages = append(messages, anthropic.NewUserMessage(toolResults...))
    }
}
```

**Key API surface:**

| Symbol | Purpose |
|---|---|
| `resp.ToParam()` | Convert `Message` response → `MessageParam` for history |
| `block.AsAny().(type)` | Type-switch on `ContentBlockUnion` variants |
| `variant.JSON.Input.Raw()` | Raw JSON string of tool input (for `json.Unmarshal`) |
| `anthropic.NewToolResultBlock(id, content, isError)` | Build `tool_result` block |
| `anthropic.NewUserMessage(blocks...)` | Wrap tool results as a user turn |
| `anthropic.StopReasonToolUse` | `StopReason` constant to check loop termination |
| `anthropic.ToolUnionParam{OfTool: &t}` | Wrap `ToolParam` in the union for `Tools:` |

---

## Extended Thinking

Enable Claude's internal reasoning by setting `Thinking` in `MessageNewParams`. The response will contain `ThinkingBlock` content before the final `TextBlock`.

Derived from `anthropic-sdk-go${PATH}:${NUM}` (`ThinkingConfigParamOfEnabled`).

```go
resp, err := client.Messages.New(context.Background(), anthropic.MessageNewParams{
    Model:     anthropic.ModelClaudeSonnet4_6,
    MaxTokens: ${NUM},  // must be > budget_tokens
    // ThinkingConfigParamOfEnabled(budgetTokens) is the helper constructor.
    // budgetTokens must be >= ${NUM} and < MaxTokens.
    Thinking: anthropic.ThinkingConfigParamOfEnabled(${NUM}),
    Messages: []anthropic.MessageParam{
        anthropic.NewUserMessage(anthropic.NewTextBlock("How many r's in strawberry?")),
    },
})
if err != nil {
    log.Fatal(err)
}

// Thinking blocks come before text blocks in Content
for _, block := range resp.Content {
    switch variant := block.AsAny().(type) {
    case anthropic.ThinkingBlock:
        fmt.Println("[thinking]", variant.Thinking)
    case anthropic.TextBlock:
        fmt.Println("[response]", variant.Text)
    }
}
```

To disable: `anthropic.NewThinkingConfigDisabledParam()`. For adaptive thinking (model decides budget): `anthropic.NewThinkingConfigAdaptiveParam()`.
