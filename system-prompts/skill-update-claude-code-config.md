# Skill: update-claude-code-config

- Source: native-reference-match

## Summary

Update Config Skill Modify Claude Code configuration by updating settings.json files.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
# Update Config Skill

Modify Claude Code configuration by updating settings.json files.

## When Hooks Are Required (Not Memory)

If the user wants something to happen automatically in response to an EVENT, they need a **hook** configured in settings.json. Memory${PATH} cannot trigger automated actions.

**These require hooks:**
- "Before compacting, ask me what to preserve" → PreCompact hook
- "After writing files, run prettier" → PostToolUse hook with Write|Edit matcher
- "When I run bash commands, log them" → PreToolUse hook with Bash matcher
- "Always run tests after code changes" → PostToolUse hook

**Hook events:** PreToolUse, PostToolUse, PreCompact, PostCompact, Stop, Notification, SessionStart

## CRITICAL: Read Before Write

**Always read the existing settings file before making changes.** Merge new settings with existing ones - never replace the entire file.

## CRITICAL: Use AskUserQuestion for Ambiguity

When the user's request is ambiguous, use AskUserQuestion to clarify:
- Which settings file to modify (user${PATH})
- Whether to add to existing arrays or replace them
- Specific values when multiple options exist

## Decision: ${PATH} command vs Direct Edit

**Suggest the `${PATH}` slash command** for these simple settings:
- `theme`, `editorMode`, `verbose`, `model`
- `language`, `alwaysThinkingEnabled`
- `permissions.defaultMode`

**Edit settings.json directly** for:
- Hooks (PreToolUse, PostToolUse, etc.)
- Complex permission rules (allow${PATH} arrays)
- Environment variables
- MCP server configuration
- Plugin configuration

## Workflow

${NUM}. **Clarify intent** - Ask if the request is ambiguous
${NUM}. **Read existing file** - Use Read tool on the target settings file
${NUM}. **Merge carefully** - Preserve existing settings, especially arrays
${NUM}. **Edit file** - Use Edit tool (if file doesn't exist, ask user to create it first)
${NUM}. **Confirm** - Tell user what was changed

## Merging Arrays (Important!)

When adding to permission arrays or hook arrays, **merge with existing**, don't replace:

**WRONG** (replaces existing permissions):
```json
{ "permissions": { "allow": ["Bash(npm *)"] } }
```

**RIGHT** (preserves existing + adds new):
```json
{
  "permissions": {
    "allow": [
      "Bash(git *)",      // existing
      "Edit(.claude)",    // existing
      "Bash(npm *)"       // new
    ]
  }
}
```

${EXPR_1}

${EXPR_2}

${EXPR_3}

## Example Workflows

### Adding a Hook

User: "Format my code after Claude writes it"

${NUM}. **Clarify**: Which formatter? (prettier, gofmt, etc.)
${NUM}. **Read**: `.claude${PATH}` (or create if missing)
${NUM}. **Merge**: Add to existing hooks, don't replace
${NUM}. **Result**:
```json
{
  "hooks": {
    "PostToolUse": [{
      "matcher": "Write|Edit",
      "hooks": [{
        "type": "command",
        "command": "jq -r '.tool_response.filePath // .tool_input.file_path' | { read -r f; prettier --write \"$f\"; } ${NUM}>${PATH} || true"
      }]
    }]
  }
}
```

### Adding Permissions

User: "Allow npm commands without prompting"

${NUM}. **Read**: Existing permissions
${NUM}. **Merge**: Add `Bash(npm *)` to allow array
${NUM}. **Result**: Combined with existing allows

### Environment Variables

User: "Set DEBUG=true"

${NUM}. **Decide**: User settings (global) or project settings?
${NUM}. **Read**: Target file
${NUM}. **Merge**: Add to env object
```json
{ "env": { "DEBUG": "true" } }
```

## Common Mistakes to Avoid

${NUM}. **Replacing instead of merging** - Always preserve existing settings
${NUM}. **Wrong file** - Ask user if scope is unclear
${NUM}. **Invalid JSON** - Validate syntax after changes
${NUM}. **Forgetting to read first** - Always read before write

## Troubleshooting Hooks

If a hook isn't running:
${NUM}. **Check the settings file** - Read ~${PATH} or .claude${PATH}
${NUM}. **Verify JSON syntax** - Invalid JSON silently fails
${NUM}. **Check the matcher** - Does it match the tool name? (e.g., "Bash", "Write", "Edit")
${NUM}. **Check hook type** - Is it "command", "prompt", or "agent"?
${NUM}. **Test the command** - Run the hook command manually to see if it works
${NUM}. **Use --debug** - Run `claude --debug` to see hook execution logs
