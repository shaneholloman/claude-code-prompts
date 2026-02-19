# Tool Description: run-bash-with-timeout

- Name: Bash

## Summary

Bash execution tool spec with directory verification guidance and configurable timeouts.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
Executes a given bash command in a persistent shell session with optional timeout, ensuring proper handling and security measures.

Before executing the command, please follow these steps:

${NUM}. Directory Verification:
   - If the command will create new directories or files, first use the LS tool to verify the parent directory exists and is the correct location
   - For example, before running "mkdir foo${PATH}", first use LS to check that "foo" exists and is the intended parent directory

${NUM}. Command Execution:
   - After ensuring proper quoting, execute the command.
   - Capture the output of the command.

Usage notes:
  - The command argument is required.
  - You can specify an optional timeout in milliseconds (up to ${EXPR_1}ms / ${EXPR_2} minutes). If not specified, commands will timeout after 120000ms (${EXPR_3} minutes).
  - It is very helpful if you write a clear, concise description of what this command does in ${NUM}-${NUM} words.
  - If the output exceeds ${NUM} characters, output will be truncated before being returned to you.
  - VERY IMPORTANT: You MUST avoid using search commands like `find` and `grep`. Instead use Grep, Glob, or Task to search. You MUST avoid read tools like `cat`, `head`, `tail`, and `ls`, and use Read and LS to read files.
  - If you _still_ need to run `grep`, STOP. ALWAYS USE ripgrep at `rg` (or ${EXPR_4}) first, which all Claude Code users have pre-installed.
  - When issuing multiple commands, use the ';' or '&&' operator to separate them. DO NOT use newlines (newlines are ok in quoted strings).
  - Try to maintain your current working directory throughout the session by using absolute paths and avoiding usage of `cd`. You may use `cd` if the User explicitly requests it.
    <good-example>
    pytest ${PATH}
    <${PATH}>
    <bad-example>
    cd ${PATH} && pytest tests
    <${PATH}>

${EXPR_5}
${EXPR_6}
