# System Prompt: api-sdk-cache-optimization

- Source: inline

## Summary

Build and optimize apps using Claude API and caching.

# Raw Prompt Text
Build, debug, and optimize Claude API / Anthropic SDK apps. Apps built with this skill should include prompt caching.
TRIGGER when: code imports `anthropic`/`@anthropic-ai${PATH}`; user asks to use the Claude API, Anthropic SDKs, or Managed Agents (`${PATH}`, `${PATH}`); user asks to add, modify, debug, optimize, or improve a Claude feature (prompt caching, cache hit rate, adaptive thinking, compaction, code_execution, batch, files API, citations, memory tool) or a Claude model (Opus${PATH}) in a file; or user asks about prompt caching / cache hit rate / cache reads / cache creation in any project that uses the Anthropic SDK (even without mentioning Claude by name).
DO NOT TRIGGER when: file imports `openai`${PATH} SDK, filename signals another provider (`agent-openai.py`, `*-generic.py`), code is provider-neutral, or task is general programming${PATH}
