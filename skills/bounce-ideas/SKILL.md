---
name: bounce-ideas
description: >
  Facilitates concise, goal-directed idea-bouncing sessions by reflecting each
  idea and asking one short "Yes, and..." or "Yes, but..." question. Use when
  the user asks to bounce ideas, use the agent as a sounding board, or brainstorm
  interactively one step at a time.
---

# Bounce Ideas

## Purpose

Help users develop a larger concept or plan incrementally by asking targeted questions that move each idea forward and close relevant gaps.

This helps users organize their thoughts, work through writer's block, and maintain consistency among their ideas.

## Initial Context Collection

When the session starts, determine the central goal from the user's message. If it cannot be inferred confidently, ask one short clarification question. Do not require the user to restate an already clear goal. Briefly confirm the goal before beginning. If the initial message already contains an idea, process it immediately as the first loop iteration; otherwise, ask for the first idea.

Keep questions relevant to the central goal. Allow a promising tangent briefly when it may reveal a useful implication or alternative. If its relevance becomes unclear, ask how it contributes to the goal and then return to the goal.

## Working Loop

1. **User states idea**

Interpret direct answers, decisions, constraints, and new proposals as ideas. Treat questions, corrections, changes to the goal, and process requests according to their intent. When the user changes the central goal, briefly confirm the new goal and evaluate subsequent ideas against it. If the user has no further idea, offer two or three brief candidates and ask which they want to adopt, modify, or reject. Do not treat an agent-proposed candidate as accepted until the user adopts it.

2. **Ask follow-up question**

As soon as the user has stated an idea, briefly restate the idea only when doing so clarifies its meaning, confirms an interpretation, or exposes a tension. Then ask exactly one follow-up question.

Treat fictional, speculative, and counterfactual premises as intentional creative choices rather than factual errors. Do not affirm an idea when it contradicts accepted ideas, established world rules, the stated goal, or declared constraints. Challenge a real-world factual claim only when its accuracy materially affects the goal or the user has requested realism. Briefly identify the tension and ask one question that helps resolve it.

The follow-up question has the following properties:

* Except when identifying a tension under the rule above, it begins with "Yes, and..." or "Yes, but...".
* Use "Yes, and..." to expand or clarify an idea. Use "Yes, but..." to examine a constraint, trade-off, or edge case. Do not manufacture an objection merely to use "but".
* It can be answered with a brief response, possibly with a single word up to a few sentences.
* It advances the stated goal or clarifies a relevant constraint, implication, or gap.

Example follow-up questions:

* Goal: Design affordable long-term client logging. User idea: "A MySQL table records every client log entry." Agent: "Yes, but what retention policy keeps storage within the available budget?"
* Goal: Make the dynasty's naming system work over centuries. User idea: "Each generation is named with the next letter of the alphabet." Agent: "Yes, but what naming rule applies after Z?"
* Goal: Design an incorporeal monster that characters can investigate. User idea: "A Shadow has no physical body." Agent: "Yes, and what evidence of its presence can living characters observe?"
* Accepted idea: "Shadows cannot interact with physical matter." Later idea: "A normal sword can wound a Shadow." Agent: "That conflicts with the accepted rule that Shadows cannot interact with matter. Which rule should change?"

The follow-up question is answered by another idea from the user, i.e., proceed with step 1.

Track whether ideas are accepted, tentative, superseded, discarded, unresolved, or agent-proposed. When a new idea conflicts with an earlier one, ask whether it replaces the earlier idea or remains an alternative. Treat a user-stated assertion or decision as accepted unless they frame it as tentative or as one possible alternative. Reclassify it if the user later revises, supersedes, or discards it.

Proceed to consolidation when the user says they are finished, asks for a summary, indicates that the goal has been resolved, or asks to pause or leave the brainstorming mode.

Remain in brainstorming mode throughout the loop. Do not implement ideas, edit files, or produce finished artifacts unless the user explicitly requests that action or leaves brainstorming mode.

3. **Session consolidation**

Consolidate the material accepted ideas into concise prose organized around the session goal. Exclude discarded or superseded ideas and agent-proposed candidates that the user did not adopt. Present unresolved alternatives as alternatives rather than combining them. Do not introduce new substantive claims or silently resolve missing details, but you may paraphrase, reorder, and connect ideas for clarity. If material questions remain unanswered, add a short Open Questions list.
