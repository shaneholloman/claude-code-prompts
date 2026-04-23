# Skill: customize-keyboard-shortcuts

- Source: native-reference-match

## Summary

Skill: customize-keyboard-shortcuts - Source: inline Summary Guides safe creation or editing of keybindings with required schema fields and keystroke syntax.

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

# Raw Prompt Text
# Skill: customize-keyboard-shortcuts

- Source: inline

## Summary

Guides safe creation or editing of keybindings with required schema fields and keystroke syntax.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# Keybindings Skill
Create or modify `~${EXPR_1}` to customize keyboard shortcuts.
## CRITICAL: Read Before Write
**Always read `~${EXPR_2}` first** (it may not exist yet). Merge changes with existing bindings — never replace the entire file.
- Use **Edit** tool for modifications to existing files
- Use **Write** tool only if the file does not exist yet

## File Format
```json
```
Always include the `$schema` and `$docs` fields.

## Keystroke Syntax
**Modifiers** (combine with `+`):
- `ctrl` (alias: `control`)
- `alt` (aliases: `opt`, `option`) — note: `alt` and `meta` are identical in terminals
- `shift`
- `meta` (aliases: `cmd`, `command`)
**Special keys**: `escape`/`esc`, `enter`/`return`, `tab`, `space`, `backspace`, `delete`, `up`, `down`, `left`, `right`
**Chords**: Space-separated keystrokes, e.g. `ctrl+k ctrl+s` (${EXPR_3}-second timeout between keystrokes)
**Examples**: `ctrl+shift+p`, `alt+enter`, `ctrl+k ctrl+n`

## Unbinding Default Shortcuts
Set a key to `null` to remove its default binding:
```json
```

## How User Bindings Interact with Defaults
- User bindings are **additive** — they are appended after the default bindings
- To **move** a binding to a different key: unbind the old key (`null`) AND add the new binding
- A context only needs to appear in the user's file if they want to change something in that context

## Common Patterns
### Rebind a key
To change the external editor shortcut from `ctrl+g` to `ctrl+e`:
```json
```
### Add a chord binding
```json
```

## Behavioral Rules
${EXPR_4}. Only include contexts the user wants to change (minimal overrides)
${EXPR_5}. Validate that actions and contexts are from the known lists below
${EXPR_6}. Warn the user proactively if they choose a key that conflicts with reserved shortcuts or common tools like tmux (`ctrl+b`) and screen (`ctrl+a`)
${EXPR_7}. When adding a new binding for an existing action, the new binding is additive (existing default still works unless explicitly unbound)
${EXPR_8}. To fully replace a default binding, unbind the old key AND add the new one

## Validation with ${EXPR_9}
The `${EXPR_10}` command includes a "Keybinding Configuration Issues" section that validates `~${EXPR_11}`.
### Common Issues and Fixes
| ${EXPR_12} |
| ${EXPR_13} |
### Example ${EXPR_14} Output
```
Keybinding Configuration Issues
Location: ~${EXPR_15}
  └ [Error] Unknown context "chat"
    → Valid contexts: Global, Chat, Autocomplete, ...
  └ [Warning] "ctrl+c" may not work: Terminal interrupt (SIGINT)
```
**Errors** prevent bindings from working and must be fixed. **Warnings** indicate potential conflicts but the binding may still work.

## Reserved Shortcuts

${EXPR_16}

## Available Contexts

${EXPR_17}

## Available Actions

${EXPR_18}
