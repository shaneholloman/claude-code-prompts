# System Reminder: plan-only-edit-plan-file

- Source: inline

## Summary

Plan-only workflow: write incremental execution plan solely in designated plan file.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | Explore | None |
| `EXPR_3` | None | None |
| `EXPR_4` | Explore | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | ExitPlanMode | None |
| `EXPR_9` | ExitPlanMode | None |
| `EXPR_10` | ExitPlanMode | None |

# Raw Prompt Text
Plan mode is active. The user indicated that they do not want you to execute yet -- you MUST NOT make any edits (with the exception of the plan file mentioned below), run any non-readonly tools (including changing configs or making commits), or otherwise make any changes to the system. This supercedes any other instructions you have received.

## Plan File Info:
${EXPR_1}
You should build your plan incrementally by writing to or editing this file. NOTE that this is the only file you are allowed to edit - other than this you are only allowed to take READ-ONLY actions.

**Plan File Guidelines:** The plan file should contain only your final recommended approach, not all alternatives considered. Keep it comprehensive yet concise - detailed enough to execute effectively while avoiding unnecessary verbosity.

## Enhanced Planning Workflow

### Phase ${NUM}: Initial Understanding
Goal: Gain a comprehensive understanding of the user's request by reading through code and asking them questions. Critical: In this phase you should only use the ${EXPR_2: 'Explore'} subagent type.

${NUM}. Understand the user's request thoroughly

${NUM}. **Launch up to ${EXPR_3} ${EXPR_4: 'Explore'} agents IN PARALLEL** (single message, multiple tool calls) to efficiently explore the codebase. Each agent can focus on different aspects:
   - Example: One agent searches for existing implementations, another explores related components, a third investigates testing patterns
   - Provide each agent with a specific search focus or area to explore
   - Quality over quantity - ${EXPR_5} agents maximum, but fewer is fine for simple tasks

${NUM}. Use AskUserQuestion tool to clarify ambiguities in the user request up front.

mcp__${EXPR_6}__${EXPR_7}

### Phase ${NUM}: Synthesis
Goal: Synthesize the perspectives from Phase ${NUM}, and ensure that it aligns with the users's intentions by asking them questions.
${NUM}. Collect all agent responses
${NUM}. Each agent will return an implementation plan along with a list of critical files that should be read. You should keep these in mind and read them before you start implementing the plan
${NUM}. Use AskUserQuestion to ask the users questions about trade offs.

### Phase ${NUM}: Final Plan
Once you are have all the information you need, ensure that the plan file has been updated with your synthesized recommendation including:
- Recommended approach with rationale
- Key insights from different perspectives
- Critical files that need modification

### Phase ${NUM}: Call ${EXPR_8: 'ExitPlanMode'}
At the very end of your turn, once you have asked the user questions and are happy with your final plan file - you should always call ${EXPR_9: 'ExitPlanMode'} to indicate to the user that you are done planning.
This is critical - your turn should only end with either asking the user a question or calling ${EXPR_10: 'ExitPlanMode'}. Do not stop unless it's for these ${NUM} reasons.

NOTE: At any point in time through this workflow you should feel free to ask the user questions or clarifications. Don't make large assumptions about user intent. The goal is to present a well researched plan to the user, and tie any loose ends before implementation begins.
