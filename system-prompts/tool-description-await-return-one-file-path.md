# Tool Description: await-return-one-file-path

- Name: REPL

## Summary

Script to await and return a single file path.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
REPL is your **only way** to investigate — shell, file reads, and code search all happen here via the shorthands below. Edit, Write, and Agent are still available as top-level tools for direct use.

**Aim for ${NUM}-${NUM} REPL calls per turn** — over-fetch and batch.

## Dense scripts — every char is an output token

```javascript
o.git=sh('git status')
for(const f of (await rgf('X','src')).slice(${NUM},${NUM})) o[f]=cat(f,${NUM},${NUM})
o
```

`o` is pre-declared `{}`; assign results directly to `o.key` (no `const x=` then repack). Promise values on `o` are auto-awaited — drop `await` unless you branch on the value. **End the script with bare `o`** (or a statement) to return the full object; ending on `o.x=...` returns just that one value. Relative paths resolve against cwd. No `//` comments — the `description` param is your comment. No blank lines, single-char vars.

## API
- `sh(cmd,ms?)` → stdout+stderr (merged — never write `${NUM}>&${NUM}` or `${NUM}>${PATH}`)
- `cat(path,off?,lim?)` → file content
- `rg(pat,path?,{A,B,C,glob,head,type,i}?)` → match text
- `rgf(pat,path?,glob?)` → matching file paths[]
- `gl(pat,path?)` → glob file paths[]
- `put(path,content)` → write file
- `gh(args)` → `sh('gh '+args)` with `-R ${EXPR_1}` injected
- `chdir(path)` — set cwd for this REPL call
- `haiku(prompt,schema?)` — one-turn model sampling
- `registerTool(name,desc,schema,handler)` / `unregisterTool` / `listTools` / `getTool`
- `log` (console.log) · `str` (JSON.stringify) · `shQuote(s)` · `REPO` ('owner${PATH}')
- `await Edit({…})` / `await NotebookEdit({…})` / `await mcp__server__tool({…})` (MCP tools by full name)

Shorthands never throw — `sh`/`cat`/`rg` return the error text on failure, `rgf`/`gl` return `[]`, never `undefined`. Permission-denied is a hard no — don't retry the same call; pivot or stop.

## Rules
- One investigation = one call. Put the next step in the code; grep→read→grep in one script. A failing inner call degrades the result, not the whole script.
- No `import`/`require`/`process`${PATH} globals — the VM context is sealed. ≥${NUM} ops per call. Over-fetch (${NUM}-${NUM} files, ${NUM}-${NUM} patterns).
- Variables persist across calls. Last expression (or `o`) = return value. No top-level `return` — end with `o` and branch with `if${PATH}` above it.
- Never re-invoke a stateful op (`sh`/`Edit`/`put`) to grab another field — `git reset`, `rm`, migrations run twice.
