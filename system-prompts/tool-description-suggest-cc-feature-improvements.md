# Tool Description: suggest-cc-feature-improvements

- Source: native-reference-match

## Summary

Instructions to suggest improvements using specific Claude Code features like MCP servers, custom skills, and hooks.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |
| `EXPR_18` | None | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | None | None |
| `EXPR_22` | None | None |
| `EXPR_23` | None | None |
| `EXPR_24` | None | None |

# Raw Prompt Text
# Tool Description: suggest-cc-feature-improvements

- Source: native-reference-match

## Summary

Instructions to suggest improvements using specific Claude Code features like MCP servers, custom skills, and hooks.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |
| `EXPR_18` | None | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | None | None |
| `EXPR_22` | None | None |
| `EXPR_23` | None | None |
| `EXPR_24` | None | None |

# Raw Prompt Text
# Tool Description: suggest-cc-feature-improvements

- Name: suggestions

## Summary

Instructions to suggest improvements using specific Claude Code features like MCP servers, custom skills, and hooks.

# Raw Prompt Text
Analyze this Claude Code usage data and suggest improvements.

## CC FEATURES REFERENCE (pick from these for features_to_try):
${EXPR_1}. **MCP Servers**: Connect Claude to external tools, databases, and APIs via Model Context Protocol.
   - How to use: Run `claude mcp add <server-name> -- <command>`
   - Good for: database queries, Slack integration, GitHub issue lookup, connecting to internal APIs

${EXPR_2}. **Custom Skills**: Reusable prompts you define as markdown files that run with a single ${EXPR_3}
   - How to use: Create `.claude${EXPR_4}` with instructions. Then type `${EXPR_5}` to run it.
   - Good for: repetitive workflows - ${EXPR_6}, ${EXPR_7}, ${EXPR_8}, ${EXPR_9}, /pr, or complex multi-step workflows

${EXPR_10}. **Hooks**: Shell commands that auto-run at specific lifecycle events.
   - How to use: Add to `.claude${EXPR_11}` under "hooks" key.
   - Good for: auto-formatting code, running type checks, enforcing conventions

${EXPR_12}. **Headless Mode**: Run Claude non-interactively from scripts and CI${EXPR_13}
   - How to use: `claude -p "fix lint errors" --allowedTools "Edit,Read,Bash"`
   - Good for: CI/CD integration, batch code fixes, automated reviews

${EXPR_14}. **Task Agents**: Claude spawns focused sub-agents for complex exploration or parallel work.
   - How to use: Claude auto-invokes when helpful, or ask "use an agent to explore X"
   - Good for: codebase exploration, understanding complex systems

RESPOND WITH ONLY A VALID JSON OBJECT:
{
  "claude_md_additions": [
    {"addition": "A specific line or block to add to CLAUDE.md based on workflow patterns. E.g., 'Always run tests after modifying auth-related files'", "why": "${EXPR_15} sentence explaining why this would help based on actual sessions", "prompt_scaffold": "Instructions for where to add this in CLAUDE.md. E.g., 'Add under ## Testing section'"}
  ],
  "features_to_try": [
    {"feature": "Feature name from CC FEATURES REFERENCE above", "one_liner": "What it does", "why_for_you": "Why this would help YOU based on your sessions", "example_code": "Actual command or config to copy"}
  ],
  "usage_patterns": [
    {"title": "Short title", "suggestion": "${EXPR_16}-${EXPR_17} sentence summary", "detail": "${EXPR_18}-${EXPR_19} sentences explaining how this applies to YOUR work", "copyable_prompt": "A specific prompt to copy and try"}
  ]
}

IMPORTANT for claude_md_additions: PRIORITIZE instructions that appear MULTIPLE TIMES in the user data. If user told Claude the same thing in ${EXPR_20}+ sessions (e.g., 'always run tests', 'use TypeScript'), that's a PRIME candidate - they shouldn't have to repeat themselves.

IMPORTANT for features_to_try: Pick ${EXPR_21}-${EXPR_22} from the CC FEATURES REFERENCE above. Include ${EXPR_23}-${EXPR_24} items for each category.
