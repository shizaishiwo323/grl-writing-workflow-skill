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
3. If Introduction promises are not paid off in Results/Discussion, or major Results concepts appear without setup, route to `narrative_echo_and_payoff`.
4. If Methods do not show input-output coupling, parameter controls, validation, or processing consistency, route to `methods_evidence_chain`.
5. If Results describe figures but do not explain mechanisms, route to `mechanism_results`.
6. If Results subsections read as parallel blocks without forward pointers, backward links, delayed payoffs, or thread summaries, route to `narrative_echo_and_payoff`, usually with `mechanism_results` or `paragraph_engineering`.
7. If paragraph functions are unclear, route to `paragraph_engineering`.
8. If logic is stable but wording is clumsy, route to `sentence_hierarchy`.

## Trigger: Scientific Story Architect

Use `references/story_architect.md` before all structure, mechanism, paragraph, or sentence skills when:

- the user is unsure about the manuscript's main story;
- the manuscript contains many results but no clear central claim;
- figures and metrics feel like parallel work packages;
- Introduction, Results, and Discussion appear to emphasize different things;
- the user asks whether the manuscript is suitable for GRL.

Routing logic:

- If the main character and supporting actors are unclear, route to `story_architect` only.
- If the main character is clear but the Introduction does not funnel toward it, route to `ocar_funnel`.
- If the main character is clear but Results subsections do not pay off earlier promises, route to `narrative_echo_and_payoff` with `mechanism_results`.
- Do not polish or reorganize prose until `story_architect` has produced a Core Story, Central Scientific Question, and Supporting Actors.

## Trigger: Narrative Echo And Payoff

Use `references/narrative_echo_and_payoff.md` when the user asks about:

- 前后呼应
- 铺垫与兑现
- 提前引入
- 后文再讨论
- 承上启下
- Results 小节之间的衔接
- 小节结尾总结
- 把几个结果串成一条线
- Introduction 是否为 Results 做铺垫
- Results 是否回应 Introduction 的 gap
- 某个指标是否出现得太突然

Routing logic:

- If the issue occurs across Introduction, Results, and Discussion, route to `story_architect`, `ocar_funnel`, and `narrative_echo_and_payoff`.
- If the issue occurs within Results and Discussion subsections, route to `mechanism_results`, `narrative_echo_and_payoff`, and `paragraph_engineering`.
- Do not treat intra-Results echo as only sentence polishing.

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
- Do not treat missing promise-payoff structure as a request for decorative transition sentences.

## Example Cases

Case ID: I-001 / I-009

Source Principle: Meta Principle 0, P3, P4

Before: User asks, "帮我润色 Introduction."

Diagnosis: The Introduction opens with examples but does not narrow to a process-based gap.

Route: `ocar_funnel`, then `paragraph_engineering`.

Do not do yet: sentence polishing.

Reason: The issue is section logic, not sentence polish.
