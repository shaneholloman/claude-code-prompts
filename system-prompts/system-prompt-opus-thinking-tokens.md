# System Prompt: opus-thinking-tokens

- Source: inline

## Summary

Guide for migrating to newer Claude models.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `OPUS_ID` | None | None |

# Raw Prompt Text
# Model Migration Guide

How to move existing code to newer Claude models. Covers breaking changes, deprecated parameters, and drop-in replacements for retired models.

For the latest, authoritative version (with code samples in every supported language), WebFetch the **Migration Guide** URL from `shared${PATH}`. Use this file for the consolidated, skill-resident reference; fall back to the live docs whenever a model launch or breaking change may have shifted the picture.

**This file is large.** Use the section names below to jump (or `Grep` this file for the heading text). Read Step ${NUM} and Step ${NUM} first — they apply to every migration. Then read only the per-target section for the model you are migrating to.

| Section | When you need it |
|---|---|
| Step ${NUM}: Confirm the migration scope | Always — before any edits |
| Step ${NUM}: Classify each file | Always — decides whether to swap, add-alongside, or skip |
| Per-SDK Syntax Reference | Translate the Python examples in this guide to TypeScript / Go / Ruby / Java / C# / PHP |
| Destination Models / Retired Model Replacements | Picking a target model |
| Breaking Changes by Source Model | Migrating to Opus ${NUM} / Sonnet ${NUM} |
| Migrating to Opus ${NUM} | Migrating to Opus ${NUM} (breaking changes, silent defaults, behavioral shifts) |
| Opus ${NUM} Migration Checklist | The required vs optional items for ${NUM}, tagged `[BLOCKS]` / `[TUNE]` |
| Verify the Migration | After edits — runtime spot-check |

**TL;DR:** Change the model ID string. If you were using `budget_tokens`, switch to `thinking: {type: "adaptive"}`. If you were using assistant prefills, they ${NUM} on both Opus ${NUM} and Sonnet ${NUM} — switch to one of the prefill replacements (most often `output_config.format`; see the table in Breaking Changes by Source Model). If you're moving from Sonnet ${NUM} to Sonnet ${NUM}, set `effort` explicitly — ${NUM} defaults to `high`. Remove the `effort-${DATE}` and `fine-grained-tool-streaming-${DATE}` beta headers (GA on ${NUM}); remove `interleaved-thinking-${DATE}` once you're on adaptive thinking (keep it only while using the transitional `budget_tokens` escape hatch). Then drop back from `client.beta.messages.create` to `client.messages.create`. Dial back any aggressive "CRITICAL: YOU MUST" tool instructions; ${NUM} follows the system prompt much more closely.

---

## Step ${NUM}: Confirm the migration scope

**Before any Write, Edit, or MultiEdit call, confirm the scope.** If the user's request does not explicitly name a single file, a specific directory, or an explicit file list, **ask first — do not start editing**. This is non-negotiable: even imperative-sounding requests like "migrate my codebase", "move my project to X", "upgrade to Sonnet ${NUM}", or bare "migrate to Opus ${NUM}" leave the scope ambiguous and require a clarifying question. Phrases like "my project", "my code", "my codebase", "the whole thing", "everywhere", or "across the repo" are **ambiguous, not directive** — they tell you *what* to do but not *where*. Ask before doing.

Offer the common scopes explicitly and wait for the answer before touching any file:

${NUM}. The entire working directory
${NUM}. A specific subdirectory (e.g. `src/`, `app/`, `services${PATH}`)
${NUM}. A specific file or a list of files

Surface this as a single clarifying question so the user can answer in one turn. **Proceed without asking only when the scope is already unambiguous** — the user named an exact file ("migrate `extract.py` to Sonnet ${NUM}"), pointed at a specific directory ("migrate everything under `services${PATH}` to Opus ${NUM}"), listed specific files ("update `a.py` and `b.py`"), or already answered the scope question in an earlier turn. If you can answer the question "which files is this change going to touch?" with a precise list from the prompt alone, proceed. If not, ask.

**Worked example.** If the user says *"Move my project to Opus ${NUM}. I want adaptive thinking everywhere it makes sense."* you do not know whether "my project" means the whole working directory, just `src/`, just the production code, or something else — the `everywhere` makes the intent clear (update every call site *within scope*) but the scope itself is still not defined. Do not start editing. Respond with:

> Before I start editing, can you confirm the scope? I can migrate:
> ${NUM}. Every `.py` file in the working directory
> ${NUM}. Just the files under `src/` (production code)
> ${NUM}. A specific subdirectory or list of files you name
>
> Which one?

Then wait for the answer. The same applies to *"Migrate to Opus ${NUM}"* and bare *"Help me upgrade to Sonnet ${NUM}"* — ask before editing.

**Sizing the scope question (large repos).** Before asking, get a per-directory count so the user can pick concretely:

```sh
rg -l "<old-model-id>" --type-not md | cut -d/ -f1 | sort | uniq -c | sort -rn
```

Present the breakdown in your scope question (e.g. *"Found ${NUM} references across ${NUM} directories: api/ (${NUM}), api-go/ (${NUM}), routing/ (${NUM}). Which to migrate?"*). Also confirm `git status` is clean before surveying — unexpected modifications mean a concurrent process; stop and investigate before proceeding.

---

## Step ${NUM}: Classify each file

Not every file that contains the old model ID is a **caller** of the API. Before editing, classify each file into one of these buckets — the right action differs:

| # | Bucket | What it looks like | Action |
|---|---|---|---|
| ${NUM} | **Calls the API${PATH}** | `client.messages.create(model=…)`, `anthropic.Anthropic()`, request payloads | Swap the model ID **and** apply the breaking-change checklist for the target version (below). |
| ${NUM} | **Defines or serves the model** | Model registries, OpenAPI specs, routing${PATH} configs, model-policy enums, generated catalogs | The old entry **stays** (the model is still served). Ask whether to (a) add the new model alongside, (b) leave alone, or (c) retire the old model — never blind-replace. **If you can't ask, default to (a): add the new model alongside and flag it** — replacing would de-register a model that's still in production. |
| ${NUM} | **References the ID as an opaque string** | UI fallback constants, capability-gate substring checks, generic test fixtures, label parsers, env defaults | Usually swap the string and verify any parser${PATH} match handles the new ID — but check the sub-cases below first. |
| ${NUM} | **Suffixed variant ID** | `claude-<model>-<suffix>` like `-fast`, `-1024k`, `-200k`, `[1m]`, dated snapshots | These are deployment${PATH} identifiers, not the public model ID. **Do not assume a new-model equivalent exists.** Verify in the registry first; if absent, leave the string alone and flag it. |

**Bucket ${NUM} sub-cases — before swapping a string reference, check:**

- **Capability gate** (e.g. `if 'opus-${NUM}-${NUM}' in model_id:` enables a feature) → **add the new ID alongside**, don't replace. The old model is still served and still has the capability, so replacing would silently disable the feature for any old-model traffic that still flows through. If you know no old-model traffic will hit this gate (single-caller codebase fully migrating), replacing is fine; if unsure, add alongside.
- **Registry-assert test** (e.g. `assert "claude-X" in supported_models`, `test_X_has_N_clusters`) → **add an assertion for the new model alongside; keep the old one.** The old model is still served, so its assertion stays valid — but the registry should also include the new model, so assert that too. Heuristic: if the test references multiple model versions in a list, it's a registry test; if one model in a struct compared only to itself, it's a generic fixture.
- **Frozen / generated snapshot** → **regenerate**, don't hand-edit.
- **Coupled to a definer** (e.g. an integration test that passes model authorization via a shared `conftest` seed list, or asserts on a billing-tier / rate-limit-group enum or a generated SKU${PATH} catalog) → **verify the definer has a new-model entry first.** If not, add a seed entry (reusing the nearest existing tier as a placeholder); if you can't confidently do that, ask the user how to populate the definer. **Do not skip the test.** Swapping without populating the definer will make the test fail at runtime.

When migrating tests specifically: breaking parameters (`temperature`, `top_p`, `budget_tokens`) are usually absent — test fixtures rarely set sampling params on placeholder models. The breaking-change scan is still required, but expect mostly clean results.

**Find intentionally-flagged sync points first.** Many codebases tag spots that must change at every model launch with comment markers like `MODEL LAUNCH`, `KEEP IN SYNC`, `@model-update`, or similar. Grep for whatever convention the repo uses *before* the broad model-ID grep — those markers point at the load-bearing changes.

---

## Per-SDK Syntax Reference

Code examples in this guide are Python. **The same fields exist in every official Anthropic SDK** — Stainless generates all ${NUM} from the same OpenAPI spec, so JSON field names map ${NUM}:${NUM} with only case-convention differences. Use the rows below to translate the Python examples to the SDK you are migrating.

> **Verify type and method names against the SDK source before writing them into customer code.** WebFetch the relevant repository from the SDK source-code table in `shared${PATH}` (one row per SDK) and confirm the exact symbol — particularly for typed SDKs (Go, Java, C#) where union${PATH} names can differ from the JSON shape. Do not guess type names that aren't in the table below or in `<lang>${PATH}`.

<!-- The rows below were verified against each SDK's `synced${PATH}` branch. -->

### `thinking` — `budget_tokens` → adaptive

| SDK | Before | After |
|---|---|---|
| Python | `thinking={"type": "enabled", "budget_tokens": N}` | `thinking={"type": "adaptive"}` |
| TypeScript | `thinking: { type: 'enabled', budget_tokens: N }` | `thinking: { type: 'adaptive' }` |
| Go | `Thinking: anthropic.ThinkingConfigParamOfEnabled(N)` | `Thinking: anthropic.ThinkingConfigParamUnion{OfAdaptive: &anthropic.ThinkingConfigAdaptiveParam{}}` |
| Ruby | `thinking: { type: "enabled", budget_tokens: N }` | `thinking: { type: "adaptive" }` |
| Java | `.thinking(ThinkingConfigEnabled.builder().budgetTokens(N).build())` | `.thinking(ThinkingConfigAdaptive.builder().build())` |
| C# | `Thinking = new ThinkingConfigEnabled { BudgetTokens = N }` | `Thinking = new ThinkingConfigAdaptive()` |
| PHP | `thinking: ['type' => 'enabled', 'budget_tokens' => N]` | `thinking: ['type' => 'adaptive']` |

### Sampling parameters — `temperature` / `top_p` / `top_k`

(Remove the field entirely on Opus ${NUM}; on Claude ${NUM}.x keep at most one of `temperature` or `top_p`.)

| SDK | Field(s) to remove |
|---|---|
| Python | `temperature=…`, `top_p=…`, `top_k=…` |
| TypeScript | `temperature: …`, `top_p: …`, `top_k: …` |
| Go | `Temperature: anthropic.Float(…)`, `TopP: anthropic.Float(…)`, `TopK: anthropic.Int(…)` |
| Ruby | `temperature: …`, `top_p: …`, `top_k: …` |
| Java | `.temperature(…)`, `.topP(…)`, `.topK(…)` |
| C# | `Temperature = …`, `TopP = …`, `TopK = …` |
| PHP | `temperature: …`, `topP: …`, `topK: …` |

### Prefill replacement — structured outputs via `output_config.format`

| SDK | Remove (last assistant turn) | Add |
|---|---|---|
| Python | `{"role": "assistant", "content": "…"}` | `output_config={"format": {"type": "json_schema", "schema": SCHEMA}}` |
| TypeScript | `{ role: 'assistant', content: '…' }` | `output_config: { format: { type: 'json_schema', schema: SCHEMA } }` |
| Go | trailing `anthropic.MessageParam{Role: "assistant", …}` | `OutputConfig: anthropic.OutputConfigParam{Format: anthropic.JSONOutputFormatParam{…}}` |
| Ruby | `{ role: "assistant", content: "…" }` | `output_config: { format: { type: "json_schema", schema: SCHEMA } }` |
| Java | trailing `Message.builder().role(ASSISTANT)…` | `.outputConfig(OutputConfig.builder().format(JsonOutputFormat.builder()…build()).build())` |
| C# | trailing `new Message { Role = "assistant", … }` | `OutputConfig = new OutputConfig { Format = new JsonOutputFormat { … } }` |
| PHP | trailing `['role' => 'assistant', 'content' => '…']` | `outputConfig: ['format' => ['type' => 'json_schema', 'schema' => $SCHEMA]]` |

### `thinking.display` — opt back into summarized reasoning (Opus ${NUM})

| SDK | Add |
|---|---|
| Python | `thinking={"type": "adaptive", "display": "summarized"}` |
| TypeScript | `thinking: { type: 'adaptive', display: 'summarized' }` |
| Go | `Thinking: anthropic.ThinkingConfigParamUnion{OfAdaptive: &anthropic.ThinkingConfigAdaptiveParam{Display: anthropic.ThinkingConfigAdaptiveDisplaySummarized}}` |
| Ruby | `thinking: { type: "adaptive", display: "summarized" }` (or `display_:` when constructing the model class directly) |
| Java | `.thinking(ThinkingConfigAdaptive.builder().display(ThinkingConfigAdaptive.Display.SUMMARIZED).build())` |
| C# | `Thinking = new ThinkingConfigAdaptive { Display = Display.Summarized }` |
| PHP | `thinking: ['type' => 'adaptive', 'display' => 'summarized']` |

For any field not in these tables, the JSON key in the Python example translates directly: `snake_case` for Python${PATH}, `camelCase` named args for PHP, `PascalCase` struct fields for Go/C#, `camelCase` builder methods for Java.

---

## Explain every change you make

Migration edits often look arbitrary to a user who hasn't read the release notes — a removed `temperature`, a deleted prefill, a rewritten system-prompt sentence. **For each edit, tell the user what you changed and why**, tied to the specific API or behavioral change that motivates it. Do this in your summary as you work, not just at the end.

Be especially explicit about **system-prompt edits**. Users are rightly protective of their prompts, and prompt-tuning changes are judgment calls (not hard API requirements). For any prompt edit:

- Quote the before and after text.
- State the behavioral shift that motivates it (e.g. *"Opus ${NUM} calibrates response length to task complexity, so I added an explicit length instruction"*, or *"${NUM} follows instructions more literally, so 'CRITICAL: YOU MUST use the search tool' will now overtrigger — softened to 'Use the search tool when…'"*).
- Make clear which prompt edits are **optional tuning** (tone, length, subagent guidance) versus which code edits are **required to avoid a ${NUM}** (sampling params, `budget_tokens`, prefills). Never present an optional prompt change as mandatory.

If you're applying several prompt-tuning edits at once, offer them as a short list the user can accept or decline item-by-item rather than silently rewriting their system prompt.

---

## Before You Migrate

${NUM}. **Confirm the target model ID.** Use only the exact strings from `shared${PATH}` — do not append date suffixes to aliases (`claude-opus-${NUM}-${NUM}`, not `claude-opus-${NUM}-${NUM}-${NUM}`). Guessing an ID will ${NUM}.
${NUM}. **Check which features your code uses** with this checklist:
   - `thinking: {type: "enabled", budget_tokens: N}` → migrate to adaptive thinking on Opus ${NUM} / Sonnet ${NUM} (still functional but deprecated)
   - Assistant-turn prefills (`messages` ending with `role: "assistant"`) → must change on Opus ${NUM} / Sonnet ${NUM} (returns ${NUM})
   - `output_format` parameter on `messages.create()` → must change on all models (deprecated API-wide)
   - `max_tokens > ~${NUM}` → must stream on any model (above ~16K risks SDK HTTP timeouts). When streaming, Sonnet ${NUM} / Haiku ${NUM} cap at 64K and Opus ${NUM} caps at 128K
   - Beta headers `effort-${DATE}`, `fine-grained-tool-streaming-${DATE}`, `interleaved-thinking-${DATE}` → GA on ${NUM}, remove them and switch from `client.beta.messages.create` to `client.messages.create`
   - Moving Sonnet ${NUM} → Sonnet ${NUM} with no `effort` set → ${NUM} defaults to `high`, which may change your latency${PATH} profile
   - System prompts with `CRITICAL`, `MUST`, `If in doubt, use X` language → likely to overtrigger on ${NUM} (see Prompt-Behavior Changes)
   - Coming from ${NUM}.x / ${NUM} / ${NUM}: also check sampling params (`temperature` + `top_p`), tool versions (`text_editor_20250728`), `refusal` + `model_context_window_exceeded` stop reasons, trailing-newline tool-param handling
${NUM}. **Test on a single request first.** Run one call against the new model, inspect the response, then roll out.

---

## Destination Models (recommended targets)

| If you're on…                         | Migrate to         | Why                                               |
| ------------------------------------- | ------------------ | ------------------------------------------------- |
| Opus ${NUM}                              | `claude-opus-${NUM}-${NUM}`  | Most capable model; adaptive thinking only; high-res vision; see Migrating to Opus ${NUM} |
| Opus ${NUM} / ${NUM} / ${NUM} / Opus ${NUM}         | `claude-opus-${NUM}-${NUM}`  | Most intelligent ${NUM}.x before ${NUM}; adaptive thinking; 128K output |
| Sonnet ${NUM} / ${NUM} / ${NUM} / ${NUM}          | `claude-sonnet-${NUM}-${NUM}`| Best speed / intelligence balance; adaptive thinking; 64K output |
| Haiku ${NUM} / ${NUM}                         | `claude-haiku-${NUM}-${NUM}` | Fastest and most cost-effective                   |

Default to the latest Opus for the caller's tier unless they explicitly chose otherwise. If you're moving from Opus ${NUM} or older directly to Opus ${NUM}, apply the ${NUM} migration first, then layer the Opus ${NUM} changes on top (see Migrating to Opus ${NUM} below).

---

## Retired Model Replacements

These models return ${NUM} — update immediately:

| Retired model                 | Retired       | Drop-in replacement  |
| ----------------------------- | ------------- | -------------------- |
| `claude-${NUM}-${NUM}-sonnet-${NUM}`  | Feb ${NUM}, ${NUM}  | `claude-sonnet-${NUM}-${NUM}`  |
| `claude-${NUM}-${NUM}-haiku-${NUM}`   | Feb ${NUM}, ${NUM}  | `claude-haiku-${NUM}-${NUM}`   |
| `claude-${NUM}-opus-${NUM}`      | Jan ${NUM}, ${NUM}   | `claude-opus-${NUM}-${NUM}`    |
| `claude-${NUM}-${NUM}-sonnet-${NUM}`  | Oct ${NUM}, ${NUM}  | `claude-sonnet-${NUM}-${NUM}`  |
| `claude-${NUM}-${NUM}-sonnet-${NUM}`  | Oct ${NUM}, ${NUM}  | `claude-sonnet-${NUM}-${NUM}`  |
| `claude-${NUM}-sonnet-${NUM}`    | Jul ${NUM}, ${NUM}  | `claude-sonnet-${NUM}-${NUM}`  |
| `claude-${NUM}`, `claude-${NUM}`    | Jul ${NUM}, ${NUM}  | `claude-sonnet-${NUM}-${NUM}`  |

## Deprecated Models (retiring soon)

| Model                         | Retires       | Replacement          |
| ----------------------------- | ------------- | -------------------- |
| `claude-${NUM}-haiku-${NUM}`     | Apr ${NUM}, ${NUM}  | `claude-haiku-${NUM}-${NUM}`   |
| `claude-opus-${NUM}-${NUM}`      | June ${NUM}, ${NUM} | `claude-opus-${NUM}-${NUM}`    |
| `claude-sonnet-${NUM}-${NUM}`    | June ${NUM}, ${NUM} | `claude-sonnet-${NUM}-${NUM}`  |

---

## Breaking Changes by Source Model

### Migrating from Sonnet ${NUM} to Sonnet ${NUM} (effort default change)

Sonnet ${NUM} had no `effort` parameter; Sonnet ${NUM} defaults to `high`. If you just switch the model string and do nothing else, you may see noticeably higher latency and token usage. Set `effort` explicitly.

**Recommended starting points:**

| Workload                                          | Start at       | Notes                                                                                                    |
| ------------------------------------------------- | -------------- | -------------------------------------------------------------------------------------------------------- |
| Chat, classification, content generation          | `low`          | With `thinking: {"type": "disabled"}` you'll see similar or better performance vs. Sonnet ${NUM} no-thinking |
| Most applications (balanced)                      | `medium`       | The default sweet spot for quality vs. cost                                                              |
| Agentic coding, tool-heavy workflows              | `medium`       | Pair with adaptive thinking and a generous `max_tokens` (up to 64K with streaming — Sonnet ${NUM}'s ceiling) |
| Autonomous multi-step agents, long-horizon loops  | `high`         | Scale down to `medium` if latency${PATH} become a concern                                                 |
| Computer-use agents                               | `high` + adaptive | Sonnet ${NUM}'s best computer-use accuracy is on adaptive + high                                          |

For non-thinking chat workloads specifically:

```python
client.messages.create(
    model="claude-sonnet-${NUM}-${NUM}",
    max_tokens=${NUM},
    thinking={"type": "disabled"},
    output_config={"effort": "low"},
    messages=[{"role": "user", "content": "..."}],
)
```

**When to use Opus ${NUM} instead:** hardest and longest-horizon problems — large code migrations, deep research, extended autonomous work. Sonnet ${NUM} wins on fast turnaround and cost efficiency.

### Migrating to Opus ${NUM} / Sonnet ${NUM} (from any older model)

**${NUM}. Manual extended thinking is deprecated — use adaptive thinking.**

`thinking: {type: "enabled", budget_tokens: N}` (manual extended thinking with a fixed token budget) is deprecated on Opus ${NUM} and Sonnet ${NUM}. Replace it with `thinking: {type: "adaptive"}`, which lets Claude decide when and how much to think. Adaptive thinking also enables interleaved thinking automatically (no beta header needed).

```python
# Old (still works on older models, deprecated on ${NUM})
response = client.messages.create(
    model="claude-sonnet-${NUM}-${NUM}",
    max_tokens=${NUM},
    thinking={"type": "enabled", "budget_tokens": ${NUM}},
    messages=[...]
)

# New (Opus ${NUM} / Sonnet ${NUM})
response = client.messages.create(
    model="claude-opus-${NUM}-${NUM}",  # or "claude-sonnet-${NUM}-${NUM}"
    max_tokens=${NUM},
    thinking={"type": "adaptive"},
    output_config={"effort": "high"},  # optional: low | medium | high | max
    messages=[...]
)
```

Adaptive thinking is the long-term target, and on internal evaluations it outperforms manual extended thinking. Move when you can.

**Transitional escape hatch:** manual extended thinking is still *functional* on Opus ${NUM} and Sonnet ${NUM} (deprecated, will be removed in a future release). If you need a hard ceiling while migrating — for example, to bound token spend on a runaway workload before you've tuned `effort` — you can keep `budget_tokens` around alongside an explicit `effort` value, then remove it in a follow-up. `budget_tokens` must be strictly less than `max_tokens`:

```python
# Transitional only — deprecated, plan to remove
client.messages.create(
    model="claude-sonnet-${NUM}-${NUM}",
    max_tokens=${NUM},
    thinking={"type": "enabled", "budget_tokens": ${NUM}},  # must be < max_tokens
    output_config={"effort": "medium"},
    messages=[...],
)
```

If the user asks for a "thinking budget" on ${NUM}, the preferred answer is `effort` — use `low`, `medium`, `high`, or `max` (Opus-tier only — not Sonnet or Haiku) rather than a token count.

**${NUM}. Effort parameter (Opus ${NUM}, Opus ${NUM}, Sonnet ${NUM} only).**

Controls thinking depth and overall token spend. Goes inside `output_config`, not top-level. Default is `high`. `max` is Opus-tier only (Opus ${NUM} and later — not Sonnet or Haiku). Errors on Sonnet ${NUM} and Haiku ${NUM}.

```python
output_config={"effort": "medium"}  # often the best cost / quality balance
```

### Migrating to the ${NUM} family (Opus ${NUM} and Sonnet ${NUM})

**${NUM}. Assistant-turn prefills return ${NUM} (Opus ${NUM} and Sonnet ${NUM}).**

Prefilled responses on the final assistant turn are no longer supported on either Opus ${NUM} or Sonnet ${NUM} — both return a ${NUM}. Adding assistant messages *elsewhere* in the conversation (e.g., for few-shot examples) still works. Pick the replacement that matches what the prefill was doing:

| Prefill was used for                               | Replacement                                                                                                                               |
| -------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| Forcing JSON / YAML / schema output                | `output_config.format` with a `json_schema` — see example below                                                                           |
| Forcing a classification label                     | Tool with an enum field containing valid labels, or structured outputs                                                                    |
| Skipping preambles (`Here is the summary:\n`)      | System prompt instruction: *"Respond directly without preamble. Do not start with phrases like 'Here is...' or 'Based on...'."*           |
| Steering around bad refusals                       | Usually no longer needed — ${NUM} refuses far more appropriately. Plain user-turn prompting is sufficient.                                   |
| Continuing an interrupted response                 | Move continuation into the user turn: *"Your previous response was interrupted and ended with `[last text]`. Continue from there."*     |
| Injecting reminders / context hydration            | Inject into the user turn instead. For complex agent harnesses, expose context via a tool call or during compaction.                      |

```python
# Old (fails on Opus ${NUM} / Sonnet ${NUM}) — prefill forcing JSON shape
messages=[
    {"role": "user", "content": "Extract the name."},
    {"role": "assistant", "content": "{\"name\": \""},
]

# New — structured outputs replace the prefill
response = client.messages.create(
    model="claude-opus-${NUM}-${NUM}",
    max_tokens=${NUM},
    output_config={"format": {"type": "json_schema", "schema": {...}}},
    messages=[{"role": "user", "content": "Extract the name."}],
)
```

**${NUM}. Stream for `max_tokens > ~16K` (all models); Opus ${NUM} alone reaches 128K.**

Non-streaming requests hit SDK HTTP timeouts at high `max_tokens`, regardless of model — stream for anything above ~16K output. The streamable ceiling differs by model: Sonnet ${NUM} and Haiku ${NUM} cap at 64K, and Opus ${NUM} alone goes up to 128K.

```python
with client.messages.stream(model="claude-opus-${NUM}-${NUM}", max_tokens=${NUM}, ...) as stream:
    message = stream.get_final_message()
```

**${NUM}. Tool-call JSON escaping may differ (Opus ${NUM} and Sonnet ${NUM}).**

Both ${NUM} models can produce tool call `input` fields with Unicode or forward-slash escaping. Always parse with `json.loads()` / `JSON.parse()` — never raw-string-match the serialized input.

### All models

**${NUM}. `output_format` → `output_config.format` (API-wide).**

The old top-level `output_format` parameter on `messages.create()` is deprecated. Use `output_config.format` instead. This is not ${NUM}-specific — applies to every model.

---

## Beta Headers to Remove on ${NUM}

Several beta headers that were required on ${NUM} are now GA on ${NUM} and should be removed. Leaving them in is harmless but misleading; removing them also lets you move from `client.beta.messages.create(...)` back to `client.messages.create(...)`.

| Header                                    | Status on ${NUM}                                              | Action                                                  |
| ----------------------------------------- | ---------------------------------------------------------- | ------------------------------------------------------- |
| `effort-${DATE}`                       | Effort parameter is GA                                     | Remove                                                  |
| `fine-grained-tool-streaming-${DATE}`  | GA                                                         | Remove                                                  |
| `interleaved-thinking-${DATE}`         | Adaptive thinking enables interleaved thinking automatically | Remove when using adaptive thinking; still functional on Sonnet ${NUM} *with* manual extended thinking, but that path is deprecated |
| `token-efficient-tools-${DATE}`        | Built in to all Claude ${NUM}+ models                           | Remove (no effect)                                      |
| `output-128k-${DATE}`                  | Built in to Claude ${NUM}+ models                               | Remove (no effect)                                      |

Once you remove all of these and finish moving to adaptive thinking, you can switch the SDK call site from the beta namespace back to the regular one:

```python
# Before
response = client.beta.messages.create(
    model="claude-opus-${NUM}-${NUM}",
    betas=["interleaved-thinking-${DATE}", "effort-${DATE}"],
    ...
)

# After
response = client.messages.create(
    model="claude-opus-${NUM}-${NUM}",
    thinking={"type": "adaptive"},
    output_config={"effort": "high"},
    ...
)
```

---

## Additional Changes When Coming from ${NUM}.x / ${NUM} / ${NUM} → ${NUM}

If you're jumping from Opus ${NUM}, Sonnet ${NUM}, Sonnet ${NUM}, or an older Claude ${NUM}.x model directly to ${NUM}, apply everything above *plus* the items in this section. Users already on Opus ${NUM} / Sonnet ${NUM} can skip this.

**${NUM}. Sampling parameters: `temperature` OR `top_p`, not both.**

Passing both will error on every Claude ${NUM}+ model:

```python
# Old (${NUM}.x only — errors on ${NUM}+)
client.messages.create(temperature=${NUM}, top_p=${NUM}, ...)

# New
client.messages.create(temperature=${NUM}, ...)  # or top_p, not both
```

**${NUM}. Update tool versions.**

Legacy tool versions are not supported on ${NUM}+. **Both the `type` and the `name` field change** — `text_editor_20250728` and `str_replace_based_edit_tool` are a pair; updating one without the other 400s. Also remove the `undo_edit` command from your text-editor integration:

| Old                                               | New                                                     |
| ------------------------------------------------- | ------------------------------------------------------- |
| `text_editor_20250124` + `str_replace_editor`     | `text_editor_20250728` + `str_replace_based_edit_tool`  |
| `code_execution_*` (earlier versions)             | `code_execution_20250825`                               |
| `undo_edit` command                               | *(no longer supported — delete call sites)*             |

```python
# Before
tools = [{"type": "text_editor_20250124", "name": "str_replace_editor"}]

# After — BOTH fields change
tools = [{"type": "text_editor_20250728", "name": "str_replace_based_edit_tool"}]
```

**${NUM}. Handle the `refusal` stop reason.**

Claude ${NUM}+ can return `stop_reason: "refusal"` on the response. If your code only handles `end_turn` / `tool_use` / `max_tokens`, add a branch:

```python
if response.stop_reason == "refusal":
    # Surface the refusal to the user; do not retry with the same prompt
    ...
```

**${NUM}. Handle the `model_context_window_exceeded` stop reason (${NUM}+).**

Distinct from `max_tokens`: it means the model hit the *context window* limit, not the requested output cap. Handle both:

```python
if response.stop_reason == "model_context_window_exceeded":
    # Context window exhausted — compact or split the conversation
    ...
elif response.stop_reason == "max_tokens":
    # Requested output cap hit — retry with higher max_tokens or stream
    ...
```

**${NUM}. Trailing newlines preserved in tool call string parameters (${NUM}+).**

${NUM} and ${NUM} preserve trailing newlines that older models stripped. If your tool implementations do exact string matching against tool-call `input` values (e.g., `if name == "foo"`), verify they still match when the model sends `"foo\n"`. Normalizing with `.rstrip()` on the receiving side is usually the simplest fix.

**${NUM}. Haiku: rate limits reset between generations.**

Haiku ${NUM} has its own rate-limit pool separate from Haiku ${NUM} / ${NUM}. If you're ramping traffic as you migrate, check your tier's Haiku ${NUM} limits at [API rate limits](${URL}) — a quota that comfortably served Haiku ${NUM} traffic may need a tier bump for the same volume on ${NUM}.

---

## Prompt-Behavior Changes (Opus ${NUM} / ${NUM}, Sonnet ${NUM})

These don't break your code, but prompts that worked on ${NUM}-and-earlier may over- or under-trigger on ${NUM}. Tune as needed.

**${NUM}. Aggressive instructions cause overtriggering.** Opus ${NUM} and ${NUM} follow the system prompt much more closely than earlier models. Prompts written to *overcome* the old reluctance are now too aggressive:

| Before (worked on ${NUM} / ${NUM})                | After (use on ${NUM})                        |
| ------------------------------------------- | ----------------------------------------- |
| `CRITICAL: You MUST use this tool when...`  | `Use this tool when...`                   |
| `Default to using [tool]`                   | `Use [tool] when it would improve X`      |
| `If in doubt, use [tool]`                   | *(delete — no longer needed)*             |

If the model is now overtriggering a tool or skill, the fix is almost always to dial back the language, not to add more guardrails.

**${NUM}. Overthinking and excessive exploration (Opus ${NUM}).** At higher `effort` settings, Opus ${NUM} explores more before answering. If that burns too many thinking tokens, lower `effort` first (`medium` is often the sweet spot) before adding prose instructions to constrain reasoning.

**${NUM}. Overeager subagent spawning (Opus ${NUM}).** Opus ${NUM} has a strong preference for delegating to subagents. If you see it spawning a subagent for something a direct `grep` or `read` would solve, add guidance: *"Use subagents only for parallel or independent workstreams. For single-file reads or sequential operations, work directly."*

**${NUM}. Overengineering (Opus ${NUM} / ${NUM}).** Both models may add extra files, abstractions, or defensive error handling beyond what was asked. If you want minimal changes, prompt for it explicitly: *"Only make changes directly requested. Don't add helpers, abstractions, or error handling for scenarios that can't happen."*

**${NUM}. LaTeX math output (Opus ${NUM}).** Opus ${NUM} defaults to LaTeX (`\frac{}{}`, `$...$`) for math and technical content. If you need plain text, instruct it explicitly: *"Format all math as plain text — no LaTeX, no `$`, no `\frac{}{}`. Use `/` for division and `^` for exponents."*

**${NUM}. Skipped verbal summaries (${NUM} family).** The ${NUM} models are more concise and may skip the summary paragraph after a tool call, jumping straight to the next action. If you rely on those summaries for visibility, add: *"After completing a task that involves tool use, provide a brief summary of what you did."*

**${NUM}. "Think" as a trigger word (Opus ${NUM} with thinking disabled).** When `thinking` is off, Opus ${NUM} is particularly sensitive to the word *think* and may reason more than you want. Use `consider`, `evaluate`, or `reason through` instead.

---

## Model-ID Rename Quick Reference

| Old string (migration source)  | New string         |
| ------------------------------ | ------------------ |
| `claude-opus-${NUM}-${NUM}`              | `claude-opus-${NUM}-${NUM}`  |
| `claude-opus-${NUM}-${NUM}`              | `claude-opus-${NUM}-${NUM}`  |
| `claude-opus-${NUM}-${NUM}`              | `claude-opus-${NUM}-${NUM}`  |
| `claude-opus-${NUM}-${NUM}`              | `claude-opus-${NUM}-${NUM}`  |
| `claude-sonnet-${NUM}-${NUM}`            | `claude-sonnet-${NUM}-${NUM}`|
| `claude-sonnet-${NUM}-${NUM}`            | `claude-sonnet-${NUM}-${NUM}`|

Older aliases (`claude-opus-${NUM}-${NUM}`, `claude-sonnet-${NUM}-${NUM}`, `claude-opus-${NUM}-${NUM}`, etc.) are still active and can be pinned if you need time before upgrading — see `shared${PATH}` for the full legacy list.

---

## Migration Checklist

Every item is tagged: **`[BLOCKS]`** items cause a ${NUM} error, infinite loop, silent timeout, or wrong tool selection if missed — apply these as code edits, not as suggestions. **`[TUNE]`** items are quality${PATH} adjustments.

For each file that calls `messages.create()` / equivalent SDK method:

- [ ] **[BLOCKS]** Update the `model=` string to the new alias
- [ ] **[BLOCKS]** Replace `budget_tokens` with `thinking={"type": "adaptive"}` (deprecated on Opus ${NUM} / Sonnet ${NUM})
- [ ] **[BLOCKS]** Move `format` from top-level `output_format` into `output_config.format`
- [ ] **[BLOCKS]** Remove any assistant-turn prefills if targeting Opus ${NUM} or Sonnet ${NUM} (see the prefill replacement table)
- [ ] **[BLOCKS]** Switch to streaming if `max_tokens > ~${NUM}` (otherwise SDK HTTP timeout)
- [ ] **[TUNE]** Set `output_config={"effort": "..."}` explicitly — especially when moving Sonnet ${NUM} → Sonnet ${NUM} (${NUM} defaults to `high`)
- [ ] **[TUNE]** Remove GA beta headers: `effort-${DATE}`, `fine-grained-tool-streaming-${DATE}`, `token-efficient-tools-${DATE}`, `output-128k-${DATE}`; remove `interleaved-thinking-${DATE}` once on adaptive thinking
- [ ] **[TUNE]** Switch `client.beta.messages.create(...)` → `client.messages.create(...)` once all betas are removed
- [ ] **[TUNE]** Review system prompt for aggressive tool language (`CRITICAL:`, `MUST`, `If in doubt`) and dial it back

**Extra items when coming from ${NUM}.x / ${NUM} / ${NUM}:**
- [ ] **[BLOCKS]** Remove either `temperature` or `top_p` (passing both 400s on Claude ${NUM}+)
- [ ] **[BLOCKS]** Update text-editor tool `type` to `text_editor_20250728`
- [ ] **[BLOCKS]** Update text-editor tool `name` to `str_replace_based_edit_tool` — **changing only the `type` and keeping `name: "str_replace_editor"` returns a ${NUM}**
- [ ] **[BLOCKS]** Update code-execution tool to `code_execution_20250825`
- [ ] **[BLOCKS]** Delete any `undo_edit` command call sites
- [ ] **[TUNE]** Add handling for `stop_reason == "refusal"`
- [ ] **[TUNE]** Add handling for `stop_reason == "model_context_window_exceeded"` (${NUM}+)
- [ ] **[TUNE]** Verify tool-param string matching tolerates trailing newlines (preserved on ${NUM}+)
- [ ] **[TUNE]** If moving to Haiku ${NUM}: review rate-limit tier (separate pool from Haiku ${NUM}.x)

**Verification:**
- [ ] Run one test request and inspect `response.stop_reason`, `response.usage`, and whether tool-use / thinking behavior matches expectations

For cached prompts: the render order and hash inputs did not change, so existing `cache_control` breakpoints keep working. However, **changing the model string invalidates the existing cache** — the first request on the new model will write the cache fresh.

---

## Migrating to Opus ${NUM}

> **Model ID `claude-opus-${NUM}-${NUM}` is authoritative as written here.** When the user asks to migrate to Opus ${NUM}, write `model="claude-opus-${NUM}-${NUM}"` exactly. Do **not** WebFetch to verify — this guide is the source of truth for migration target IDs. The corresponding entry exists in `shared${PATH}`.

Claude Opus ${NUM} is our most capable generally available model to date. It is highly autonomous and performs exceptionally well on long-horizon agentic work, knowledge work, vision tasks, and memory tasks. This section summarizes everything new at launch. It is layered on top of the ${NUM} migration above — if the caller is jumping from Opus ${NUM} or older, apply the ${NUM} changes first, then apply this section.

**TL;DR for someone already on Opus ${NUM}:** update the model ID to `claude-opus-${NUM}-${NUM}`, strip any remaining `budget_tokens` and sampling parameters (both ${NUM} on Opus ${NUM}), give `max_tokens` extra headroom and re-baseline with `count_tokens()` against the new model, opt back into `thinking.display: "summarized"` if reasoning is surfaced to users, and re-tune `effort` — it matters more on ${NUM} than on any prior Opus.

### Breaking changes (will ${NUM} on Opus ${NUM})

**Extended thinking removed.**

`thinking: {type: "enabled", budget_tokens: N}` is no longer supported on Claude Opus ${NUM} or later models and returns a ${NUM} error. Switch to adaptive thinking (`thinking: {type: "adaptive"}`) and use the effort parameter to control thinking depth. Adaptive thinking is **off by default** on Claude Opus ${NUM}: requests with no `thinking` field run without thinking, matching Opus ${NUM} behavior. Set `thinking: {type: "adaptive"}` explicitly to enable it.

```python
# Before (Opus ${NUM})
client.messages.create(
    model="claude-opus-${NUM}-${NUM}",
    max_tokens=${NUM},
    thinking={"type": "enabled", "budget_tokens": ${NUM}},
    messages=[{"role": "user", "content": "..."}],
)

# After (Opus ${NUM})
client.messages.create(
    model="claude-opus-${NUM}-${NUM}",
    max_tokens=${NUM},
    thinking={"type": "adaptive"},
    output_config={"effort": "high"},  # or "max", "xhigh", "medium", "low"
    messages=[{"role": "user", "content": "..."}],
)
```

If the caller wasn't using extended thinking, no change is required — thinking is off by default, or can be set explicitly with `thinking={"type": "disabled"}`.

Delete `budget_tokens` plumbing entirely. For the replacement `effort` value, see **Choosing an effort level on Opus ${NUM}** below — there is no exact ${NUM}:${NUM} mapping from `budget_tokens`.

**Sampling parameters removed.**

The `temperature`, `top_p`, and `top_k` parameters are no longer accepted on Claude Opus ${NUM}. Requests that include them return a ${NUM} error. Remove these fields from your request payloads. Prompting is the recommended way to guide model behavior on Claude Opus ${NUM}. If you were using `temperature = ${NUM}` for determinism, note that it never guaranteed identical outputs on prior models.

```python
# Before — errors on Opus ${NUM}
client.messages.create(temperature=${NUM}, top_p=${NUM}, ...)

# After
client.messages.create(...)  # no sampling params
```

- **If the intent was determinism** — use `effort: "low"` with a tighter prompt.
- **If the intent was creative variance** — the prompt replacement depends on the use case; **ask the user** how they want variance elicited. If you can't ask, add a use-case-appropriate instruction along the lines of *"choose something off-distribution and interesting"* — e.g. for text generation, *"Vary your phrasing and structure across responses"*; for frontend${PATH}, use the propose-${NUM}-directions approach under **Design and frontend coding** below.

### Choosing an effort level on Opus ${NUM}

`budget_tokens` controlled how much to *think*; `effort` controls how much to think *and* act, so there is no exact ${NUM}:${NUM} mapping. **Use `xhigh` for best results in coding and agentic use cases, and a minimum of `high` for most intelligence-sensitive use cases.** Experiment with other levels to further tune token usage and intelligence:

| Level | Use when | Notes |
| --- | --- | --- |
| `max` | Intelligence-demanding tasks worth testing at the ceiling | Can deliver gains in some use cases but may show diminishing returns from increased token usage; can be prone to overthinking |
| `xhigh` | **Most coding and agentic use cases** | The best setting for these; used as the default in Claude Code |
| `high` | Intelligence-sensitive use cases generally | Balances token usage and intelligence; recommended minimum for most intelligence-sensitive work |
| `medium` | Cost-sensitive use cases that need to reduce token usage while trading off intelligence | |
| `low` | Short, scoped tasks and latency-sensitive workloads that are not intelligence-sensitive | |

### Silent default changes (no error, but behavior differs)

**Thinking content omitted by default.**

Thinking blocks still appear in the response stream on Claude Opus ${NUM}, but their `thinking` field is empty unless you explicitly opt in. This is a silent change from Claude Opus ${NUM}, where the default was to return summarized thinking text. To restore summarized thinking content on Claude Opus ${NUM}, set `thinking.display` to `"summarized"`. **The block-field name is unchanged** — it is still `block.thinking` on a `thinking`-type block; do not rename it.

**Detect this:** any code that reads `block.thinking` (or equivalent) from a `thinking`-type block and renders it in a UI, log, or trace. **The fix is the request parameter, not the response handling** — add `display: "summarized"` to the `thinking` parameter:

```python
thinking={"type": "adaptive", "display": "summarized"}  # "display" is new on Opus ${NUM}; values: "omitted" (default) | "summarized"
```

The default is `"omitted"` on Claude Opus ${NUM}. If thinking content was never surfaced anywhere, no change needed. If your product streams reasoning to users, the new default appears as a long pause before output begins; set `display: "summarized"` to restore visible progress during thinking.

**Updated token counting.**

Claude Opus ${NUM} and Claude Opus ${NUM} count tokens differently. The same input text produces a higher token count on Claude Opus ${NUM} than on Claude Opus ${NUM}, and `${PATH}` will return a different number of tokens for Claude Opus ${NUM} than it did for Claude Opus ${NUM}. The token efficiency of Claude Opus ${NUM} can vary by workload shape. Prompting interventions, `task_budget`, and `effort` can help control costs and ensure appropriate token usage. Keep in mind that these controls may trade off model intelligence. **Update your `max_tokens` parameters to give additional headroom, including compaction triggers.** Claude Opus ${NUM} provides a 1M context window at standard API pricing with no long-context premium.

What else to check:

- Client-side token estimators (tiktoken-style approximations) calibrated against ${NUM}
- Cost calculators that multiply tokens by a fixed per-token rate
- Rate-limit retry thresholds keyed to measured token counts

Re-baseline by re-running `client.messages.count_tokens()` against `claude-opus-${NUM}-${NUM}` on a representative sample of the caller's prompts. Do not apply a blanket multiplier. For cost-sensitive workloads, consider reducing `effort` by one level (e.g. `high` → `medium`). For agentic loops, consider adopting Task Budgets (below).

### New feature: Task Budgets (beta)

Opus ${NUM} introduces **task budgets** — tell Claude how many tokens it has for a full agentic loop (thinking + tool calls + final output). The model sees a running countdown and uses it to prioritize work and wrap up gracefully as the budget is consumed.

This is a **suggestion the model is aware of**, not a hard cap. It is distinct from `max_tokens`, which remains the enforced per-response limit and is *not* surfaced to the model. Use `task_budget` when you want the model to self-moderate; use `max_tokens` as a hard ceiling to cap usage.

Requires beta header `task-budgets-${DATE}`:

```python
client.beta.messages.create(
    betas=["task-budgets-${DATE}"],
    model="claude-opus-${NUM}-${NUM}",
    max_tokens=${NUM},
    thinking={"type": "adaptive"},
    output_config={
        "effort": "high",
        "task_budget": {"type": "tokens", "total": ${NUM}},
    },
    messages=[...],
)
```

Set a generous budget for open-ended agentic tasks and tighten it for latency-sensitive ones. **Minimum `task_budget.total` is ${NUM},${NUM} tokens.** If the budget is too restrictive for the task, the model may complete it less thoroughly, referencing its budget as the constraint. **Do not add `task_budget` during a migration unless you are sure the budget value is right** — if you can run the workload and measure, do so; otherwise ask the user for the value rather than guessing. This is the primary lever for offsetting the token-counting shift on agentic workloads.

### Capability improvements

**High-resolution vision.** Opus ${NUM} is the first Claude model with high-resolution image support. Maximum image resolution is **${NUM} pixels on the long edge** (up from 1568px on Opus ${NUM} and prior). This unlocks gains on vision-heavy workloads, especially computer use and screenshot${PATH} understanding. Coordinates returned by the model now map ${NUM}:${NUM} to actual image pixels, so no scale-factor math is needed.

High-res support is **automatic on Opus ${NUM}** — no beta header, no client-side opt-in required. The model accepts larger inputs and returns pixel-accurate coordinates out of the box.

**Token cost.** Full-resolution images on Opus ${NUM} can use up to ~${NUM}× more image tokens than on prior models (up to ~${NUM} tokens per image, vs. the previous ~${NUM},${NUM}-token cap). If the extra fidelity isn't needed, downsample client-side before sending to control cost — but **do not add downsampling by default during a migration**. If you're not sure whether the pipeline needs the fidelity, ask the user rather than guessing. Use `count_tokens()` on representative images on Opus ${NUM} to re-baseline before reacting to any measured cost shift.

Beyond resolution, Opus ${NUM} also improves on low-level perception (pointing, measuring, counting) and natural-image bounding-box localization and detection.

**Knowledge work.** Meaningful gains on tasks where the model visually verifies its own output — `.docx` redlining, `.pptx` editing, and programmatic chart${PATH} analysis (e.g. pixel-level data transcription via image-processing libraries). If prompts have scaffolding like *"double-check the slide layout before returning"*, try removing it and re-baselining.

**Memory.** Opus ${NUM} is better at writing and using file-system-based memory. If an agent maintains a scratchpad, notes file, or structured memory store across turns, that agent should improve at jotting down notes to itself and leveraging its notes in future tasks.

**User-facing progress updates.** Opus ${NUM} provides more regular, higher-quality interim updates during long agentic traces. If the system prompt has scaffolding like *"After every ${NUM} tool calls, summarize progress"*, try removing it to avoid excessive user-facing text. If the length or contents of Opus ${NUM}'s updates are not well-calibrated to your use case, explicitly describe what these updates should look like in the prompt and provide examples.

### Real-time cybersecurity safeguards

Requests that involve prohibited or high-risk topics may lead to refusals.

### Fast Mode: not available on Opus ${NUM}

Opus ${NUM} does not have a Fast Mode variant. **Opus ${NUM} Fast remains supported**. Only surface this if the caller's code actually uses a Fast Mode model string (e.g. `claude-opus-${NUM}-${NUM}-fast`); if the word "fast" does not appear in the code, say nothing about Fast Mode.

When you see `model="claude-opus-${NUM}-${NUM}-fast"` (or similar), **the migration edit is**:

```python
# Opus ${NUM} has no Fast Mode — keeping on ${NUM} Fast (caller's choice to switch to standard Opus ${NUM}).
model="claude-opus-${NUM}-${NUM}-fast",
```

That is: leave the model string **unchanged**, add the comment above it, and tell the user their two options — (a) stay on Opus ${NUM} Fast, which remains supported, or (b) move latency-tolerant traffic to standard Opus ${NUM} for the intelligence gain. Do **not** rewrite the model string to `claude-opus-${NUM}-${NUM}` yourself; that silently trades latency for intelligence, which is the caller's decision.

### Behavioral shifts (prompt-tunable)

These don't break anything, but prompts tuned for Opus ${NUM} may land differently. Opus ${NUM} is more steerable than ${NUM}, so small prompt nudges usually close the gap.

**More literal instruction following.** Claude Opus ${NUM} interprets prompts more literally and explicitly than Claude Opus ${NUM}, particularly at lower effort levels. It will not silently generalize an instruction from one item to another, and it will not infer requests you didn't make. The upside of this literalism is precision and less thrash. It generally performs better for API use cases with carefully tuned prompts, structured extraction, and pipelines where you want predictable behavior. A prompt and harness review may be especially helpful for migration to Claude Opus ${NUM}.

**Verbosity calibrates to task complexity.** Opus ${NUM} scales response length to how complex it judges the task to be, rather than defaulting to a fixed verbosity — shorter answers on simple lookups, much longer on open-ended analysis. If the product depends on a particular length or style, tune the prompt explicitly. To reduce verbosity:

> *"Provide concise, focused responses. Skip non-essential context, and keep examples minimal."*

If you see specific kinds of over-verbosity (e.g. over-explaining), add instructions targeting those. Positive examples showing the desired level of concision tend to be more effective than negative examples or instructions telling the model what not to do. Do **not** assume existing "be concise" instructions should be removed — test first.

**Tone and writing style.** Opus ${NUM} is more direct and opinionated, with less validation-forward phrasing and fewer emoji than Opus ${NUM}'s warmer style. As with any new model, prose style on long-form writing may shift. If the product relies on a specific voice, re-evaluate style prompts against the new baseline. If a warmer or more conversational voice is wanted, specify it:

> *"Use a warm, collaborative tone. Acknowledge the user's framing before answering."*

**`effort` matters more than on any prior Opus.** Opus ${NUM} respects `effort` levels more strictly, especially at the low end. At `low` and `medium` it scopes work to what was asked rather than going above and beyond — good for latency and cost, but on moderate tasks at `low` there is some risk of under-thinking.

- If shallow reasoning shows up on complex problems, raise `effort` to `high` or `xhigh` rather than prompting around it.
- If `effort` must stay `low` for latency, add targeted guidance: *"This task involves multi-step reasoning. Think carefully through the problem before responding."*
- **At `xhigh` or `max`, set a large `max_tokens`** so the model has room to think and act across tool calls and subagents. Start at 64K and tune from there. (`xhigh` is a new effort level on Opus ${NUM}, between `high` and `max`.)

Adaptive-thinking triggering is also steerable. If the model thinks more often than wanted — which can happen with large or complex system prompts — add: *"Thinking adds latency and should only be used when it will meaningfully improve answer quality — typically for problems that require multi-step reasoning. When in doubt, respond directly."*

**Uses tools less often by default.** Opus ${NUM} tends to use tools less often than ${NUM} and to use reasoning more. This produces better results in most cases, but for products that rely on tools (search${PATH}, function-calling, computer-use steps), it can drop tool-use rate. Two levers:

- **Raise `effort`** — `high` or `xhigh` show substantially more tool usage in agentic search and coding, and are especially useful for knowledge work.
- **Prompt for it** — be explicit in tool descriptions or the system prompt about when and how to use the tool, and encourage the model to err on the side of using it more often:

> *"When the answer depends on information not present in the conversation, you MUST call the `search` tool before answering — do not answer from prior knowledge."*

**Fewer subagents by default.** Opus ${NUM} tends to spawn fewer subagents than ${NUM}. This is steerable — give explicit guidance on when delegation is desirable. For a coding agent, for example:

> *"Do NOT spawn a subagent for work you can complete directly in a single response (e.g. refactoring a function you can already see). Spawn multiple subagents in the same turn when fanning out across items or reading multiple files."*

**Design and frontend coding.** Opus ${NUM} has stronger design instincts than ${NUM}, with a consistent default house style: warm cream${PATH} backgrounds (around `#F4F1EA`), serif display type (Georgia, Fraunces, Playfair), italic word-accents, and a terracotta${PATH} accent. This reads well for editorial, hospitality, and portfolio briefs, but will feel off for dashboards, dev tools, fintech, healthcare, or enterprise apps — and it appears in slide decks as well as web UIs.

The default is persistent. Generic instructions ("don't use cream," "make it clean and minimal") tend to shift the model to a different fixed palette rather than producing variety. Two approaches work reliably:

${NUM}. **Specify a concrete alternative.** The model follows explicit specs precisely — give exact hex values, typefaces, and layout constraints.
${NUM}. **Have the model propose options before building.** This breaks the default and gives the user control:

   > *"Before building, propose ${NUM} distinct visual directions tailored to this brief (each as: bg hex / accent hex / typeface — one-line rationale). Ask the user to pick one, then implement only that direction."*

If the caller previously relied on `temperature` for design variety, use approach (${NUM}) — it produces meaningfully different directions across runs.

Opus ${NUM} also requires less frontend-design prompting than previous models to avoid generic "AI slop" aesthetics. Where earlier models needed a lengthy anti-slop snippet, Opus ${NUM} generates distinctive, creative frontends with a much shorter nudge. This snippet works well alongside the variety approaches above:

> *"NEVER use generic AI-generated aesthetics like overused font families (Inter, Roboto, Arial, system fonts), cliched color schemes (particularly purple gradients on white or dark backgrounds), predictable layouts and component patterns, and cookie-cutter design that lacks context-specific character. Use unique fonts, cohesive colors and themes, and animations for effects and micro-interactions."*

**Interactive coding products.** Opus ${NUM}'s token usage and behavior can differ between autonomous, asynchronous coding agents with a single user turn and interactive, synchronous coding agents with multiple user turns. Specifically, it tends to use more tokens in interactive settings, primarily because it reasons more after user turns. This can improve long-horizon coherence, instruction following, and coding capabilities in long interactive coding sessions, but also comes with more token usage. To maximize both performance and token efficiency in coding products, use `effort: "xhigh"` or `"high"`, add autonomous features (like an auto mode), and reduce the number of human interactions required from users.

When limiting required user interactions, specify the task, intent, and relevant constraints upfront in the first human turn. Well-specified, clear, and accurate task descriptions upfront help maximize autonomy and intelligence while minimizing extra token usage after user turns — because Opus ${NUM} is more autonomous than prior models, this usage pattern helps to maximize performance. In contrast, ambiguous or underspecified prompts conveyed progressively over multiple user turns tend to reduce token efficiency and sometimes performance.

**Code review.** Opus ${NUM} is meaningfully better at finding bugs than prior models, with both higher recall and precision. However, if a code-review harness was tuned for an earlier model, it may initially show *lower* recall — this is likely a harness effect, not a capability regression. When a review prompt says "only report high-severity issues," "be conservative," or "don't nitpick," Opus ${NUM} follows that instruction more faithfully than earlier models did: it investigates just as thoroughly, identifies the bugs, and then declines to report findings it judges to be below the stated bar. Precision rises, but measured recall can fall even though underlying bug-finding has improved.

Recommended prompt language:

> *"Report every issue you find, including ones you are uncertain about or consider low-severity. Do not filter for importance or confidence at this stage — a separate verification step will do that. Your goal here is coverage: it is better to surface a finding that later gets filtered out than to silently drop a bug. For each finding, include your confidence level and an estimated severity so a downstream filter can rank them."*

This can be used without an actual second step, but moving confidence filtering out of the finding step often helps. If the harness has a separate verification${PATH} stage, tell the model explicitly that its job at the finding stage is coverage, not filtering. If single-pass self-filtering is wanted, be concrete about the bar rather than using qualitative terms like "important" — e.g. *"report any bugs that could cause incorrect behavior, a test failure, or a misleading result; only omit nits like pure style or naming preferences."* Iterate on prompts against a subset of evals to validate recall or F1 gains.

**Computer use.** Computer use works across resolutions up to the new 2576px / ${NUM}.75MP maximum. Sending images at **1080p** provides a good balance of performance and cost. For particularly cost-sensitive workloads, **720p** or **${NUM}×${NUM}** are lower-cost options with strong performance. Test to find the ideal settings for the use case; experimenting with `effort` can also help tune behavior.

---

## Opus ${NUM} Migration Checklist

Every item is tagged: **`[BLOCKS]`** items cause a ${NUM} error, infinite loop, silent truncation, or empty output if missed — apply these as code edits, not as suggestions. **`[TUNE]`** items are quality${PATH} adjustments — surface them to the user as recommendations.

`[BLOCKS]` items prefixed with **"If…"** or **"At…"** are conditional. Before working through the list, **scan the file** for the conditions: does it surface thinking text to a UI${PATH}? Does it set `output_config.effort` to `"x-high"` or `"max"`? Is it a security workload? Is it a multi-turn agentic loop? Apply only the items whose condition matches.

- [ ] **[BLOCKS]** Replace `thinking: {type: "enabled", budget_tokens: N}` with `thinking: {type: "adaptive"}` + `output_config.effort`; delete `budget_tokens` plumbing entirely
- [ ] **[BLOCKS]** Strip `temperature`, `top_p`, `top_k` from request construction
- [ ] **[BLOCKS]** If thinking content is surfaced to users or stored in logs: add `thinking.display: "summarized"` (otherwise the rendered text is empty)
- [ ] **[BLOCKS]** At `output_config.effort` of `xhigh` or `max`: set `max_tokens` ≥ ${NUM} (otherwise output truncates mid-thought)
- [ ] **[TUNE]** Give `max_tokens` and compaction triggers extra headroom; re-run `count_tokens()` against `claude-opus-${NUM}-${NUM}` on representative prompts to re-baseline (no blanket multiplier)
- [ ] **[TUNE]** Re-baseline cost and rate-limit dashboards *before* reacting to measured shifts
- [ ] **[TUNE]** Re-evaluate `effort` per route — use `xhigh` for coding${PATH} and a minimum of `high` for most intelligence-sensitive work; it matters more on ${NUM} than any prior Opus
- [ ] **[TUNE]** Multi-turn agentic loops: adopt the API-native Task Budgets (`output_config.task_budget`, beta `task-budgets-${DATE}`, minimum 20k tokens) — this is for capping *cumulative* spend across a loop; per-turn depth is `effort`
- [ ] **[TUNE]** Check for ambiguous or underspecified instructions that relied on ${NUM} generalizing intent, and update them to be clearer or more precise — ${NUM} follows them literally
- [ ] **[TUNE]** Tool-use workloads: add explicit when${PATH} guidance to tool descriptions (${NUM} reaches for tools less often)
- [ ] **[TUNE]** Verbosity: test existing length instructions before changing them — ${NUM} calibrates length to task complexity, so tune for the desired output rather than assuming a direction
- [ ] **[TUNE]** Remove forced-progress-update scaffolding (*"after every N tool calls…"*)
- [ ] **[TUNE]** Remove knowledge-work verification scaffolding (*"double-check the slide layout…"*) and re-baseline
- [ ] **[TUNE]** Add tone instruction if a warmer / more conversational voice is needed; re-evaluate style prompts on writing-heavy routes
- [ ] **[TUNE]** Subagent tool present: add explicit spawn / don't-spawn guidance
- [ ] **[TUNE]** Frontend${PATH} output: specify a concrete palette${PATH}, or have the model propose ${NUM} visual directions before building (the default cream${PATH} house style is persistent)
- [ ] **[TUNE]** Interactive coding products: use `effort: "xhigh"` or `"high"`, add autonomous features (e.g. an auto mode) to reduce human interactions, and specify task${PATH} upfront in the first turn
- [ ] **[TUNE]** Code-review harnesses: remove or loosen "only report high-severity" / "be conservative" filters and have the model report every finding with confidence + severity; move filtering to a downstream step (${NUM} follows severity filters more literally, which can depress measured recall)
- [ ] **[TUNE]** Vision-heavy pipelines (screenshots, charts, document understanding): leave images at native resolution up to 2576px long edge for the accuracy gain; remove any scale-factor math from coordinate handling (coords are now ${NUM}:${NUM} with pixels). No beta header / opt-in needed — high-res is automatic on Opus ${NUM}.
- [ ] **[TUNE]** Computer-use pipelines: send screenshots at 1080p for a good performance${PATH} balance (720p or ${NUM}×${NUM} for cost-sensitive workloads); experiment with `effort` to tune behavior
- [ ] **[TUNE]** Cost-sensitive image pipelines: full-res images on ${NUM} use up to ~${NUM} tokens vs ~${NUM},${NUM} on prior models (~${NUM}×). Downsampling client-side before upload avoids the increase, but **do not downsample by default** — if you're unsure whether fidelity is needed, ask the user. Re-baseline with `count_tokens()` on representative images before reacting to cost shifts.

---

## Verify the Migration

After updating, spot-check that the new model is actually being used. Replace `YOUR_TARGET_MODEL` with the model string you migrated to (e.g. `claude-opus-${NUM}-${NUM}`, `claude-opus-${NUM}-${NUM}`, `claude-sonnet-${NUM}-${NUM}`, `claude-haiku-${NUM}-${NUM}`) and keep the assertion prefix in sync:

```python
YOUR_TARGET_MODEL = "{{OPUS_ID}}"  # or "claude-opus-${NUM}-${NUM}", "claude-sonnet-${NUM}-${NUM}", "claude-haiku-${NUM}-${NUM}"
response = client.messages.create(model=YOUR_TARGET_MODEL, max_tokens=${NUM}, messages=[...])
assert response.model.startswith(YOUR_TARGET_MODEL), response.model
```

For rate-limit headroom changes, pricing, or capability deltas (vision, structured outputs, effort support), query the Models API:

```python
m = client.models.retrieve(YOUR_TARGET_MODEL)
m.max_input_tokens, m.max_tokens
m.capabilities["effort"]["max"]["supported"]
```

See `shared${PATH}` for the full capability lookup pattern.
