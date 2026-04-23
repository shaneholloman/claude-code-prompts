# Skill: build-with-claude-api-reference-guide

- Source: native-reference-match

## Summary

Reference Documentation The relevant documentation for your detected language is included below in `<doc>` tags.

# Raw Prompt Text
## Reference Documentation

The relevant documentation for your detected language is included below in `<doc>` tags. Each tag has a `path` attribute showing its original file path. Use this to find the right section:

### Quick Task Reference

**Single text classification${PATH}&A:**
→ Refer to `{lang}${PATH}`

**Chat UI or real-time response display:**
→ Refer to `{lang}${PATH}` + `{lang}${PATH}`

**Long-running conversations (may exceed context window):**
→ Refer to `{lang}${PATH}` — see Compaction section

**Migrating to a newer model or replacing a retired model:**
→ Refer to `shared${PATH}`

**Prompt caching / optimize caching / "why is my cache hit rate low":**
→ Refer to `shared${PATH}` + `{lang}${PATH}` (Prompt Caching section)

**Function calling / tool use / agents:**
→ Refer to `{lang}${PATH}` + `shared${PATH}` + `{lang}${PATH}`

**Batch processing (non-latency-sensitive):**
→ Refer to `{lang}${PATH}` + `{lang}${PATH}`

**File uploads across multiple requests:**
→ Refer to `{lang}${PATH}` + `{lang}${PATH}`

**Agent design (tool surface, context management, caching strategy):**
→ Refer to `shared${PATH}`

**Anthropic CLI (`ant`) — terminal access, version-controlled agent${PATH} YAML, scripting:**
→ Refer to `shared${PATH}`

**Managed Agents (server-managed stateful agents):**
→ Refer to `shared${PATH}` and the rest of the `shared${PATH}*.md` files. For Python, TypeScript, and cURL, language-specific code examples live in `{lang}${PATH}`. Java, Go, Ruby, and PHP also support the API — translate the calls using your SDK's patterns from `{lang}${PATH}`. C# does not currently have Managed Agents support; use raw HTTP from `curl${PATH}` as a reference.

**Error handling:**
→ Refer to `shared${PATH}`

**Latest docs via WebFetch:**
→ Refer to `shared${PATH}` for URLs
