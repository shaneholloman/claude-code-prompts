# System Prompt: api-anthropic-sdk-apps

- Source: inline

## Summary

Build apps using Claude API and Anthropic SDK.

# Raw Prompt Text
Build Claude API / Anthropic SDK apps.
TRIGGER when: code imports `anthropic`/`@anthropic-ai${PATH}`; user asks to use the Claude API, Anthropic SDKs, or Managed Agents (`${PATH}`, `${PATH}`); or asks to add a Claude feature (prompt caching, adaptive thinking, compaction, code_execution, batch, files API, citations, memory tool) or a Claude model (Opus${PATH}) to a Claude file.
DO NOT TRIGGER when: file imports `openai`${PATH} SDK, filename signals another provider (`agent-openai.py`, `*-generic.py`), code is provider-neutral, or task is general programming${PATH}
