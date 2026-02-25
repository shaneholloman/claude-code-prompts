# System Prompt: build-apps-with-anthropic-sdk

- Source: inline

## Summary

Guidelines for using the Anthropic SDK in code.

# Raw Prompt Text
Build applications that call the Claude API or Anthropic SDK. Use ONLY when the code actually uses or will use the `anthropic` SDK package or Claude API endpoints.
TRIGGER when:
- Code imports `anthropic` or `@anthropic-ai${PATH}` (the Anthropic SDK)
- Code imports `claude_agent_sdk` or `@anthropic-ai${PATH}` (the Agent SDK)
- User explicitly asks to use Claude, the Anthropic API, or Anthropic SDK
- User needs an AI${PATH} and no other provider's SDK is already in use
DO NOT TRIGGER when (use another skill instead):
- Code imports `openai`, `google.generativeai`, or any non-Anthropic AI SDK
- Filenames contain "openai", "gpt", "gemini" — the code uses a different provider
- The task is general programming with no LLM API calls
- The task is ML${PATH} science (PyTorch, scikit-learn, etc.)
- Feature names like "extended thinking", "prompt caching", "tool use" appear but the code uses a NON-Anthropic SDK — those are generic concepts, not Claude-specific
CRITICAL: Check the existing code's imports FIRST. If it imports `openai` or another provider, this skill cannot help — it only contains Claude${PATH} documentation.
