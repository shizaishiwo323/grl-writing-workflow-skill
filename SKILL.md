---
name: grl-writing-workflow
description: Use when the user wants Codex to diagnose, plan, revise, or build prompts for GRL-style scientific manuscripts, especially mechanism-driven geoscience, reactive transport, porous media, hydrogeophysics, or NMR papers. Applies teacher-derived OCAR/funnel structure, storyline alignment, methods evidence-chain, mechanism-centered results, paragraph engineering, sentence hierarchy, revision-case mining, and prompt-building rules. Always diagnose manuscript stage before polishing sentences.
---

# GRL Writing Workflow

## Core Rule

This skill is a scientific writing operating system, not a general polishing prompt.

Always follow this order:

```text
storyline > structure > mechanism > paragraph > sentence > word choice
```

Do not perform sentence polishing when the central story, section function, or mechanism chain is still unstable. Start with diagnosis, then choose the smallest matching writing operation.

## First Move

Unless the user explicitly asks for one narrow operation, begin with `references/workflow_router.md` and, when prompt wording is needed, `references/workflow_router_prompt.md`.

Diagnose:

- Current manuscript stage.
- Core contradiction: storyline, section structure, mechanism chain, paragraph flow, sentence hierarchy, or reviewer risk.
- Which sub-skill files to use.
- Which edits are currently forbidden.
- One concrete goal for this round.

Use `references/stage_model.md` for the five-stage workflow.

## Stage Routing

Stage 1 Research Story Discovery:
Use `references/story_architect.md` and `references/ocar_funnel.md`. Output a one-sentence storyline, novelty statement, main figure sequence, supporting actor list, and mechanism sketch. Do not polish sentences.

Stage 2 Manuscript Architecture Design:
Use `references/story_architect.md`, `references/ocar_funnel.md`, and `references/skill_hierarchy_map.md`. Output section functions, subsection sequence, figure sequence, and OCAR roles. Do not do grammar-level revision.

Stage 3 Mechanism Construction:
Use `references/mechanism_results.md`, `references/methods_evidence_chain.md`, and `references/paragraph_engineering.md`. Turn results from figure description into mechanism progression. Keep secondary metrics as support, not the protagonist.

Stage 4 Reader Experience Optimization:
Use `references/paragraph_engineering.md` and `references/sentence_hierarchy.md`. Improve topic sentences, transitions, information load, reader guidance, and claim calibration after the structure is stable.

Stage 5 Reviewer-Oriented Refinement:
Use `references/principles.md`, `references/tag_system.md`, and `references/global_prompt_checklist.md`. Check novelty clarity, GRL fit, overclaim, evidence gaps, method reproducibility, broad implication, and likely reviewer attack points.

## Reference Loading

Load only the files needed for the current task.

Principles and evidence:

- `references/stage_model.md`: five-stage manuscript workflow and forbidden actions.
- `references/principles.md`: teacher-derived principle library, evidence strength, and transferable rules.
- `references/tag_frequency.md`: which principles are most frequent in the modification database.
- `references/tag_system.md`: modification label system.
- `references/raw_modification_log.md`: original revision pairs in Markdown form.
- `references/interpretation_principle_log.md`: interpreted revision principles.
- `references/modification_summary.md`: compact summary of mined changes.

Sub-skill designs:

- `references/workflow_router.md`: stage diagnosis and routing.
- `references/story_architect.md`: storyline, novelty, protagonist, supporting actors.
- `references/ocar_funnel.md`: Opening, Challenge, Action, Resolution at manuscript, section, and paragraph levels.
- `references/methods_evidence_chain.md`: methods as evidence logic, not technical display.
- `references/mechanism_results.md`: results as physical mechanism progression.
- `references/paragraph_engineering.md`: topic sentence, evidence order, mini-implication.
- `references/sentence_hierarchy.md`: sentence function, transitions, claim strength, information load.
- `references/skill_hierarchy_map.md`: how the sub-skills relate.

Prompt and test materials:

- `references/prompt_system_overview.md`: prompt system architecture.
- `references/workflow_router_prompt.md`: router prompt template.
- `references/story_architect_prompt.md`: storyline prompt template.
- `references/ocar_funnel_prompt.md`: OCAR/funnel prompt template.
- `references/methods_evidence_chain_prompt.md`: methods evidence-chain prompt template.
- `references/mechanism_results_prompt.md`: mechanism-centered results prompt template.
- `references/paragraph_engineering_prompt.md`: paragraph organization prompt template.
- `references/sentence_hierarchy_prompt.md`: sentence hierarchy prompt template.
- `references/global_prompt_checklist.md`: global quality checks.
- `references/skill_specific_checklists.md`: sub-skill-specific checks.
- `references/small_scale_testing_plan.md`: testing protocol for prompt behavior.

## Output Contract

For diagnosis tasks, output:

```text
Current stage:
Core contradiction:
Recommended sub-skills:
Currently forbidden:
This round's goal:
Next action:
```

For revision tasks, keep the output tied to the diagnosed stage:

- Storyline work: provide storyline, novelty, protagonist, supporting actors, and mechanism chain.
- OCAR work: label only Opening, Challenge, Action, and Resolution.
- Methods work: map research question to method choice, measurement, evidence, and credibility.
- Results work: rewrite around observation -> physics -> signal -> mechanism -> implication.
- Paragraph work: state paragraph function, reorder sentences, then revise.
- Sentence work: polish only after confirming the higher-level logic is stable.

When using revision evidence, cite the relevant Case ID or tag from the Markdown modification logs if available.

## Guardrails

- Prefer mechanism-first writing over workload listing.
- Prefer reader guidance over dense technical accumulation.
- Prefer concise GRL-style claims over broad unsupported implications.
- Treat methods as proof logic: why this workflow can answer the research question.
- Treat figures as evidence in a story, not as a sequence to describe one by one.
- If the user asks for pure polishing but the text has a higher-level failure, say so briefly and route upward before editing.
