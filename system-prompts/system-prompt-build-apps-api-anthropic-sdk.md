# System Prompt: bd2dfddf

- Source: inline

## Summary

Build apps with the Claude API or Anthropic SDK.

# Raw Prompt Text
Build apps with the Claude API or Anthropic SDK.
TRIGGER when: code imports `anthropic`/`@anthropic-ai${PATH}`/`claude_agent_sdk`, or user asks to use Claude API, Anthropic SDKs, or Agent SDK.
DO NOT TRIGGER when: code imports `openai`${PATH} AI SDK, general programming, or ML${PATH} tasks.
