# GRL Writing Stage Model

Use this file to route manuscript work before editing.

## Operating Order

```text
storyline > structure > mechanism > paragraph > sentence > word choice
```

The system should not move to a lower level until the higher-level problem is stable enough.

## Stage 1: Research Story Discovery

Symptoms: many results, unclear main message, novelty hard to state, too many figures competing for attention, paper feels like workload display.

Core task: find the story.

Use: `story_architect.md`, `ocar_funnel.md`.

Forbidden: sentence polishing, grammar optimization, word-choice tuning, line-by-line rewriting.

Output: one-sentence storyline, novelty statement, protagonist, supporting actors, main figure sequence, mechanism sketch.

## Stage 2: Manuscript Architecture Design

Symptoms: storyline exists, but Introduction narrowing, section order, subsection function, or figure sequence does not fully serve the mechanism chain.

Core task: design the manuscript architecture.

Use: `story_architect.md`, `ocar_funnel.md`, `skill_hierarchy_map.md`.

Forbidden: micro-polishing and treating Results as figure-by-figure description.

Output: section function table, subsection sequence, figure sequence, OCAR roles for each section.

## Stage 3: Mechanism Construction

Symptoms: sections and figures are mostly stable, but Results read like description; data, signal, physics, and mechanism are not connected.

Core task: write results as a mechanism chain.

Use: `mechanism_results.md`, `methods_evidence_chain.md`, `paragraph_engineering.md`.

Forbidden: only writing "Figure shows..." or letting secondary metrics become the protagonist.

Output: observation -> physics -> signal -> mechanism -> implication structure, figure function map, Results/Discussion boundary.

## Stage 4: Reader Experience Optimization

Symptoms: content is complete, but transitions are weak, topic sentences are unclear, sentences are overloaded, or the reader has to infer the logic.

Core task: make the paper easy and pleasant to read.

Use: `paragraph_engineering.md`, `sentence_hierarchy.md`.

Forbidden: elegant wording that hides mechanism logic or sacrifices clarity.

Output: clearer topic sentences, transitions, shorter sentence hierarchy, explicit reader guidance, concise GRL tone.

## Stage 5: Reviewer-Oriented Refinement

Symptoms: the manuscript is near submission and needs risk checking.

Core task: inspect the paper through a GRL reviewer lens.

Use: `principles.md`, `tag_system.md`, `global_prompt_checklist.md`, `skill_specific_checklists.md`.

Forbidden: assuming language polish is enough for submission.

Output: reviewer attack-point list, novelty clarity check, overclaim/underclaim check, mechanism gap check, method credibility check, GRL fit map.
