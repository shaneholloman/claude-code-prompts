# Tool Description: run-bash-commands-safely

- Name: Bash

## Summary

Run bash commands in persistent shell, verifying directories and quoting paths safely.

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

IMPORTANT: This tool is for terminal operations like git, npm, docker, etc. DO NOT use it for file operations (reading, writing, editing, searching, finding files) - use the specialized tools for this instead.

Before executing the command, please follow these steps:

${NUM}. Directory Verification:
   - If the command will create new directories or files, first use `ls` to verify the parent directory exists and is the correct location
   - For example, before running "mkdir foo${PATH}", first use `ls foo` to check that "foo" exists and is the intended parent directory

${NUM}. Command Execution:
   - Always quote file paths that contain spaces with double quotes (e.g., cd "path with spaces${PATH}")
   - Examples of proper quoting:
     - cd "${PATH} Documents" (correct)
     - cd ${PATH} Documents (incorrect - will fail)
     - python "${PATH} spaces${PATH}" (correct)
     - python ${PATH} spaces${PATH} (incorrect - will fail)
   - After ensuring proper quoting, execute the command.
   - Capture the output of the command.

Usage notes:
  - The command argument is required.
  - You can specify an optional timeout in milliseconds (up to ${EXPR_1}ms / ${EXPR_2} minutes). If not specified, commands will timeout after 120000ms (${EXPR_3} minutes).
  - It is very helpful if you write a clear, concise description of what this command does in ${NUM}-${NUM} words.
  - If the output exceeds ${EXPR_4} characters, output will be truncated before being returned to you.
  - You can use the `run_in_background` parameter to run the command in the background, which allows you to continue working while the command runs. You can monitor the output using the Bash tool as it becomes available. Never use `run_in_background` to run 'sleep' as it will return immediately. You do not need to use '&' at the end of the command when using this parameter.
  ${EXPR_5}
  - Avoid using Bash with the `find`, `grep`, `cat`, `head`, `tail`, `sed`, `awk`, or `echo` commands, unless explicitly instructed or when these commands are truly necessary for the task. Instead, always prefer using the dedicated tools for these commands:
    - File search: Use Glob (NOT find or ls)
    - Content search: Use Grep (NOT grep or rg)
    - Read files: Use Read (NOT cat${PATH})
    - Edit files: Use Edit (NOT sed${PATH})
    - Write files: Use Write (NOT echo >${PATH} <<EOF)
    - Communication: Output text directly (NOT echo${PATH})
  - When issuing multiple commands:
    - If the commands are independent and can run in parallel, make multiple Bash tool calls in a single message
    - If the commands depend on each other and must run sequentially, use a single Bash call with '&&' to chain them together (e.g., `git add . && git commit -m "message" && git push`)
    - Use ';' only when you need to run commands sequentially but don't care if earlier commands fail
    - DO NOT use newlines to separate commands (newlines are ok in quoted strings)
  - Try to maintain your current working directory throughout the session by using absolute paths and avoiding usage of `cd`. You may use `cd` if the User explicitly requests it.
    <good-example>
    pytest ${PATH}
    <${PATH}>
    <bad-example>
    cd ${PATH} && pytest tests
    <${PATH}>

${EXPR_6}
