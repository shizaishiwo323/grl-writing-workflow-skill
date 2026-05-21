# workflow_router

## Skill Objective

Diagnose the manuscript's current editing stage before choosing any writing skill. This is Skill 0 and should be called before all other writing skills.

## Input

- Manuscript section, full draft, or user request.
- Optional target journal, usually GRL or a similar short high-impact geoscience journal.
- Optional diagnosis from the user, such as "帮我润色" or "帮我看逻辑".

## Output

- Manuscript stage diagnosis: `Storyline`, `OCAR`, `Methods Evidence`, `Mechanism Results`, `Paragraph`, or `Sentence`.
- Primary skill to call next.
- Secondary skill if needed.
- One-sentence reason for routing.
- What not to do yet.
- Do not rewrite prose unless explicitly asked after routing.

## When to Call / When Not to Call

**When to call:**

- At the beginning of any substantial manuscript editing request.
- When the user asks vaguely for polishing, logic checking, or improvement.
- When it is unclear whether the problem is story, section, paragraph, or sentence level.

**When not to call:**

- When the user explicitly asks for one known skill and already provides the target section.
- When the task is a narrow formatting or citation cleanup.
- After a route has already been chosen and the next skill is actively being applied.

## Core Principles

- Meta Principle 0: Diagnose The Manuscript Stage Before Editing.
- P2: Keep One Storyline Across OCAR.
- P7: Start Paragraphs With Their Function.
- P12: Calibrate Claims To The Evidence.

## Detection Logic

Use this order:

1. If the paper cannot be summarized in one mechanism-centered sentence, route to `story_architect`.
2. If the paper has a central claim but Opening, Challenge, Action, or Resolution is weak, route to `ocar_funnel`.
3. If Methods do not show input-output coupling, parameter controls, validation, or processing consistency, route to `methods_evidence_chain`.
4. If Results describe figures but do not explain mechanisms, route to `mechanism_results`.
5. If paragraph functions are unclear, route to `paragraph_engineering`.
6. If logic is stable but wording is clumsy, route to `sentence_hierarchy`.

## Rewrite Logic

Do not rewrite. Produce routing only:

```text
Stage:
Primary skill:
Secondary skill:
Reason:
What to inspect next:
Do not do yet:
```

## Forbidden Patterns

- Do not polish sentences before diagnosing storyline and OCAR.
- Do not route every request to `sentence_hierarchy`.
- Do not treat missing evidence as a wording problem.
- Do not call a method problem a "style" problem.

## Example Cases

Case ID: I-001 / I-009

Source Principle: Meta Principle 0, P3, P4

Before: User asks, "帮我润色 Introduction."

Diagnosis: The Introduction opens with examples but does not narrow to a process-based gap.

Route: `ocar_funnel`, then `paragraph_engineering`.

Do not do yet: sentence polishing.

Reason: The issue is section logic, not sentence polish.
