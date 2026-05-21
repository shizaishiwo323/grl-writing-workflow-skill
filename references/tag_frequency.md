# Tag Frequency Summary

Source: `../01_modification_mining/modification_database.xlsx`

Scope: current modification database with 60 records covering Title, Abstract, Introduction, Methods, and Results and Discussion.

## Overall Tag Counts

| Rank | Tag | Count |
|---:|---|---:|
| 1 | `mechanism_emphasis` | 38 |
| 2 | `topic_sentence_insertion` | 27 |
| 3 | `reader_guidance` | 26 |
| 4 | `physics_first` | 21 |
| 5 | `storyline_alignment` | 18 |
| 6 | `funnel_narrowing` | 14 |
| 7 | `result_interpretation` | 13 |
| 8 | `method_reproducibility` | 10 |
| 9 | `redundancy_removal` | 2 |
| 10 | `evidence_chain` | 1 |
| 11 | `supporting_actor_reposition` | 1 |
| 12 | `overclaim_softening` | 1 |
| 13 | `sentence_flow` | 1 |
| 14 | `metric_grounding` | 1 |

## OCAR Distribution

| OCAR Position | Count |
|---|---:|
| Opening | 7 |
| Challenge | 8 |
| Action | 24 |
| Resolution | 21 |

## Section Distribution

| Section | Count |
|---|---:|
| Title | 1 |
| Abstract | 9 |
| Introduction | 17 |
| Methods | 18 |
| Results and Discussion | 15 |

## Initial Reading

The dominant pattern is not sentence-level polishing. The most frequent tags show that the teacher repeatedly pushes the paper toward mechanism-centered storytelling:

1. `mechanism_emphasis`, `physics_first`, and `result_interpretation` dominate the Results and Discussion logic.
2. `topic_sentence_insertion` and `reader_guidance` appear across all sections, showing that each paragraph needs an explicit reader-facing function.
3. `storyline_alignment` and `funnel_narrowing` are concentrated in Title, Abstract, and Introduction, showing that the front matter is being reshaped around the main scientific question rather than around a list of work done.
4. `method_reproducibility` appears in Methods, where the teacher strengthens parameter definitions, model validation, module coupling, and processing consistency.

## Evidence Strength Tiers

| Tier | Tags | Use In Principle Extraction |
|---|---|---|
| Strong | `mechanism_emphasis`, `topic_sentence_insertion`, `reader_guidance`, `physics_first`, `storyline_alignment`, `funnel_narrowing`, `result_interpretation`, `method_reproducibility` | Can support core principles and future high-priority skills. |
| Medium | `redundancy_removal` | Keep as a principle, but gather more examples before making it a standalone skill. |
| Emerging | `evidence_chain`, `supporting_actor_reposition`, `overclaim_softening`, `sentence_flow`, `metric_grounding` | Treat as important hypotheses. Mark principles based on these tags as Emerging unless supported by other high-frequency tags. |

## Phase 2 Revision Notes

- `principles_v2.md` adds `Evidence Strength`, `Primary Level`, and `Secondary Level` to each principle.
- Method-related evidence is split under Principle 5 into workflow coupling, parameter reproducibility, and processing consistency.
- A workflow-level Meta Principle was added: diagnose manuscript stage before editing.
