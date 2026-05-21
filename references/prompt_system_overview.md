# Phase 4 Prompt Building Overview

Source architecture: `../03_skill_design/`

This phase turns the Phase 3 skill architecture into AI-executable prompt templates. It does not add new skills. The goal is to make each existing skill callable, testable, and evaluable.

## Priority Order

Follow the order suggested in `临时.md`:

1. `workflow_router`
2. `mechanism_results`
3. `paragraph_engineering`
4. `sentence_hierarchy`
5. `ocar_funnel`
6. `methods_evidence_chain`
7. `story_architect`

Reason: `workflow_router` is the entrance; `mechanism_results` and `paragraph_engineering` are the highest-value execution skills for the current manuscript; `sentence_hierarchy` should only be used after logic is stable.

## Prompt Files

| Skill | Prompt Template |
|---|---|
| `workflow_router` | `prompts/workflow_router_prompt.md` |
| `mechanism_results` | `prompts/mechanism_results_prompt.md` |
| `paragraph_engineering` | `prompts/paragraph_engineering_prompt.md` |
| `sentence_hierarchy` | `prompts/sentence_hierarchy_prompt.md` |
| `ocar_funnel` | `prompts/ocar_funnel_prompt.md` |
| `methods_evidence_chain` | `prompts/methods_evidence_chain_prompt.md` |
| `story_architect` | `prompts/story_architect_prompt.md` |

## Evaluation Files

| Scope | Checklist |
|---|---|
| All prompts | `evaluation_checklists/global_prompt_checklist.md` |
| Skill-specific | `evaluation_checklists/skill_specific_checklists.md` |
| Small-scale testing | `test_protocols/small_scale_testing_plan.md` |

## Nonlinear Routing Rule

Do not call all prompts in a fixed line. First run `workflow_router_prompt.md`. Then call only the prompt that matches the diagnosed manuscript stage.

## Routing Table

| Router Stage | Prompt To Call | Main Output |
|---|---|---|
| Storyline | `prompts/story_architect_prompt.md` | Central claim, storyline spine, drift diagnosis |
| OCAR | `prompts/ocar_funnel_prompt.md` | Opening-Challenge-Action-Resolution repair |
| Methods Evidence | `prompts/methods_evidence_chain_prompt.md` | Workflow, parameter, validation, and processing checks |
| Mechanism Results | `prompts/mechanism_results_prompt.md` | Observation-to-mechanism interpretation |
| Paragraph | `prompts/paragraph_engineering_prompt.md` | Topic sentence, evidence order, paragraph function |
| Sentence | `prompts/sentence_hierarchy_prompt.md` | Physical verbs, sentence order, claim calibration |

## Minimum Prompt Contract

Every prompt template must specify:

- Role
- When to use
- Do not use when
- Inputs
- Outputs
- Procedure
- Forbidden actions
- Output format
- Example case
- Self-check
