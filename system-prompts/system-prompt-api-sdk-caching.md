# System Prompt: api-sdk-caching

- Source: inline

## Summary

Build and optimize Claude API applications.

# Raw Prompt Text
Build, debug, and optimize Claude API / Anthropic SDK apps. Apps built with this skill should include prompt caching. Also handles migrating existing Claude API code between Claude model versions (${NUM} → ${NUM}, ${NUM} → ${NUM}, retired-model replacements).
TRIGGER when: code imports `anthropic`/`@anthropic-ai${PATH}`; user asks for the Claude API, Anthropic SDK, or Managed Agents; user adds${PATH} a Claude feature (caching, thinking, compaction, tool use, batch, files, citations, memory) or model (Opus${PATH}) in a file; questions about prompt caching / cache hit rate in an Anthropic SDK project.
SKIP: file imports `openai`${PATH} SDK, filename like `*-openai.py`/`*-generic.py`, provider-neutral code, general programming${PATH}
