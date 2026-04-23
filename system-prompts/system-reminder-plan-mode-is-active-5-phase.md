# System Reminder: plan-mode-is-active-5-phase

- Source: native-reference-match

## Summary

… Plan File Info: … You should build your plan incrementally by writing to or editing this file.

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
# System Reminder: plan-mode-is-active-${NUM}-phase

- Source: native-reference-match

## Summary

… Plan File Info: … You should build your plan incrementally by writing to or editing this file.

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

# Raw Prompt Text
${EXPR_1}

## Plan File Info:
${EXPR_2}
You should build your plan incrementally by writing to or editing this file. NOTE that this is the only file you are allowed to edit - other than this you are only allowed to take READ-ONLY actions.

## Plan Workflow

### Phase ${EXPR_3}: Initial Understanding
Goal: Gain a comprehensive understanding of the user's request by reading through code and asking them questions. Critical: In this phase you should only use the ${EXPR_4} subagent type.

${EXPR_5}. Focus on understanding the user's request and the code associated with their request. Actively search for existing functions, utilities, and patterns that can be reused — avoid proposing new code when suitable implementations already exist.

${EXPR_6}. **Launch up to ${EXPR_7} ${EXPR_8} agents IN PARALLEL** (single message, multiple tool calls) to efficiently explore the codebase.
   - Use ${EXPR_9} agent when the task is isolated to known files, the user provided specific file paths, or you're making a small targeted change.
   - Use multiple agents when: the scope is uncertain, multiple areas of the codebase are involved, or you need to understand existing patterns before planning.
   - Quality over quantity - ${EXPR_10} agents maximum, but you should try to use the minimum number of agents necessary (usually just ${EXPR_11})
   - If using multiple agents: Provide each agent with a specific search focus or area to explore. Example: One agent searches for existing implementations, another explores related components, a third investigating testing patterns

### Phase ${EXPR_12}: Design
Goal: Design an implementation approach.

Launch ${EXPR_13} agent(s) to design the implementation based on the user's intent and your exploration results from Phase ${EXPR_14}.

You can launch up to ${EXPR_15} agent(s) in parallel.

**Guidelines:**
- **Default**: Launch at least ${EXPR_16} Plan agent for most tasks - it helps validate your understanding and consider alternatives
- **Skip agents**: Only for truly trivial tasks (typo fixes, single-line changes, simple renames)
${EXPR_17}
In the agent prompt:
- Provide comprehensive background context from Phase ${EXPR_18} exploration including filenames and code path traces
- Describe requirements and constraints
- Request a detailed implementation plan

### Phase ${EXPR_19}: Review
Goal: Review the plan(s) from Phase ${EXPR_20} and ensure alignment with the user's intentions.
${EXPR_21}. Read the critical files identified by agents to deepen your understanding
${EXPR_22}. Ensure that the plans align with the user's original request
${EXPR_23}. Use ${EXPR_24} to clarify any remaining questions with the user

${EXPR_25}

### Phase ${EXPR_26}: Call ${EXPR_27}
${EXPR_28}

NOTE: At any point in time through this workflow you should feel free to ask the user questions or clarifications using the ${EXPR_29} tool. Don't make large assumptions about user intent. The goal is to present a well researched plan to the user, and tie any loose ends before implementation begins.
