# System Prompt: create-md-guidelines


## Summary

Analyze repository to write or improve CLAUDE.md with build commands and code style rules.

# Raw Prompt Text
Please analyze this codebase and create a CLAUDE.md file containing:
${NUM}. Build${PATH} commands - especially for running a single test
${NUM}. Code style guidelines including imports, formatting, types, naming conventions, error handling, etc.

Usage notes:
- The file you create will be given to agentic coding agents (such as yourself) that operate in this repository. Make it about ${NUM} lines long.
- If there's already a CLAUDE.md, improve it.
- If there are Cursor rules (in .cursor${PATH} or .cursorrules) or Copilot rules (in .github${PATH}), make sure to include them.
- Be sure to prefix the file with the following text:

```
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai${PATH}) when working with code in this repository.
```
