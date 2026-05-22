# Skill Hierarchy Map

Source principles: `../02_principle_extraction/principles.md`

This is the Phase 3 skill architecture. It translates the principle library into modular, AI-callable writing skills, but it does not yet provide final prompt templates. Prompt engineering belongs to Phase 4.

## Default Maturity Pipeline / Recommended Escalation Order

Actual routing is determined by `workflow_router.md`; skills do not need to be called linearly for every task. The pipeline below describes the recommended escalation order when revising a full manuscript from an unstable draft toward final prose.

```text
0. workflow_router
   diagnose manuscript stage and choose next skill
        |
        v
1. story_architect
   define central claim and paper-wide storyline
        |
        v
2. ocar_funnel
   repair Opening, Challenge, Action, Resolution movement
        |
        v
3. narrative_echo_and_payoff
   check promise-payoff links across the paper and within Results
        |
        v
3.5. methods_evidence_chain
   align workflow, parameters, processing, validation
        |
        v
4. mechanism_results
   turn figures, trends, and numbers into mechanism claims
        |
        v
5. paragraph_engineering
   fix topic sentence, evidence order, paragraph function
        |
        v
6. sentence_hierarchy
   polish physical verbs, transitions, claim strength
```

## Skill Responsibility Boundaries

| Skill | Primary Problem | Do Not Use For |
|---|---|---|
| `workflow_router.md` | Manuscript-stage diagnosis and task routing | Rewriting actual prose |
| `story_architect.md` | Whole-paper storyline and central claim | Sentence polishing |
| `ocar_funnel.md` | Section-level OCAR structure | Detailed method reproducibility |
| `narrative_echo_and_payoff.md` | Introduction-Results payoff and Results subsection echo | Decorative transition polishing |
| `methods_evidence_chain.md` | Method workflow, parameters, validation, processing control | Results interpretation |
| `mechanism_results.md` | Result-to-mechanism interpretation | General background writing |
| `paragraph_engineering.md` | Paragraph topic sentence, evidence order, local coherence | Whole-paper architecture |
| `sentence_hierarchy.md` | Sentence-level clarity, verbs, claim calibration | Fixing missing evidence |

## Evidence Strength Priority

Skills based on high-frequency principles should be prioritized:

1. `mechanism_results.md`: `mechanism_emphasis`, `physics_first`, `result_interpretation`
2. `paragraph_engineering.md`: `topic_sentence_insertion`, `reader_guidance`
3. `story_architect.md` and `ocar_funnel.md`: `storyline_alignment`, `funnel_narrowing`
4. `methods_evidence_chain.md`: `method_reproducibility`

Use `narrative_echo_and_payoff.md` as a conservative Skill 3 between OCAR and mechanism construction: it is broader than a paragraph transition, but should not become a standalone claim-making skill.

Emerging principles should be used carefully:

- `claim_calibration` and `metric_grounding` are important but currently supported by fewer cases.
- Do not make them standalone skills yet; keep them inside `sentence_hierarchy.md` and `methods_evidence_chain.md`.
