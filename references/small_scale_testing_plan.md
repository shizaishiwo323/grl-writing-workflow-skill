# Small-Scale Testing Plan

This is the Phase 4 initial testing protocol. Do not run large-scale testing yet.

## Test Sources

Use three kinds of text:

1. Old draft paragraphs from `老师未改版本/main.tex`.
2. Revised teacher-version paragraphs from `当前最新论文情况/main.tex`.
3. Optional literature paper paragraphs later, after the internal tests are stable.

## Test Order

Follow the priority in `临时.md`:

1. Test `workflow_router_prompt.md` on one Introduction paragraph, one Methods paragraph, and one Results paragraph.
2. Test `narrative_echo_and_payoff_prompt.md` on one Introduction-Results promise, one Results subsection boundary, and one sudden-metric case.
3. Test `mechanism_results_prompt.md` on one Results paragraph that originally described spectra or tortuosity.
4. Test `paragraph_engineering_prompt.md` on one paragraph with mixed function.
5. Test `sentence_hierarchy_prompt.md` only after the same paragraph's logic is stable.
6. Test `ocar_funnel_prompt.md` on Abstract or Introduction.
7. Test `methods_evidence_chain_prompt.md` on the RTM or NMR Methods paragraph.
8. Test `story_architect_prompt.md` on title + abstract + introduction.

## Narrative Echo Tests

Use `references/narrative_echo_and_payoff_prompt.md`, `references/narrative_echo_and_payoff.md`, and `references/cases_narrative_echo_and_payoff.md`.

Expected diagnostic output:

```text
Current echo problem:
Echo type:
Missing setup/payoff:
Suggested minimal fix:
Relevant case ID:
Boundary behavior:
```

Test NEP-001: Introduction promise without payoff

Input:
An Introduction emphasizes a concept that never appears in Results.

Expected output:
Identify the orphan promise and suggest deletion, merging, or adding a Results payoff.

Relevant case IDs:
NEP-SELF-001; NEP-REF-2024-001.

Test NEP-002: Result without foreshadowing

Input:
A Results section introduces a major metric suddenly.

Expected output:
Suggest a short foreshadowing sentence in Introduction or the previous Results subsection.

Relevant case IDs:
NEP-SELF-004; NEP-REF-2018-001; NEP-REF-2024-001.

Test NEP-003: Weak Results subsection transition

Input:
Section 3.1 ends abruptly and Section 3.2 begins as an unrelated result.

Expected output:
Suggest one forward pointer at the end of 3.1 and one backward link at the beginning of 3.2.

Relevant case IDs:
NEP-SELF-003; NEP-REF-2025-001.

Optional Test NEP-004: Missing thread summary

Input:
Several Results subsections each describe useful findings, but no sentence connects them.

Expected output:
Suggest a 1-2 sentence thread summary that turns the results into a mechanism chain.

Relevant case IDs:
NEP-SELF-005; NEP-REF-2024-002.

## Minimal Narrative Echo Test Inputs

Use these only as first-round prompt behavior tests. Replace them with real manuscript excerpts after the prompt passes these simple cases.

### NEP Minimal Input 1: Introduction Promise Without Payoff

```text
Introduction excerpt:
This study aims to show that pore-scale wettability controls dissolution efficiency and can be diagnosed from NMR relaxation signals.

Results excerpt:
The Results only report T2 peak migration, tortuosity evolution, permeability breakthrough, and MVC. Wettability is not mentioned again.
```

Expected behavior:
Detect an orphan Introduction promise and recommend deleting, downgrading, or adding a real wettability payoff.

### NEP Minimal Input 2: New Metric Without Foreshadowing

```text
Previous Results excerpt:
The T2 spectra show different peak separation and merging pathways among face dissolution, channeling, and wormholing.

Next Results excerpt:
We define the matrix-vug connectivity index MVC as the valley amplitude divided by the dominant peak amplitude.
```

Expected behavior:
Detect missing delayed payoff and suggest one setup sentence explaining why T2 morphology alone is insufficient and why MVC is needed.

### NEP Minimal Input 3: Weak Results Subsection Transition

```text
Section 3.1 ending:
These spectra show that each dissolution regime has a distinct T2 pathway.

Section 3.2 opening:
Flow-field tortuosity decreases with increasing porosity in all simulations.
```

Expected behavior:
Detect missing backward link and suggest linking regime-specific T2 pathways to independent hydraulic validation by tortuosity.

## Test Record Template

```text
Test ID:
Prompt:
Input source:
Target section:
Expected skill behavior:
Boundary behavior:
Actual output:
Pass/fail:
Failure mode:
Revision needed:
```

## Pass Criteria

- The prompt stays within its assigned skill boundary.
- The test record explicitly states boundary behavior: whether the prompt stayed inside its role or crossed into another skill's work.
- The output is specific to the manuscript text.
- The output uses mechanism, evidence, and reader-navigation logic from the principle library.
- The output avoids generic "academic polishing" advice.
- The output identifies when not to revise yet.

## Failure Modes To Watch

- Router sends everything to sentence polishing.
- Results prompt rewrites style but not mechanism.
- Paragraph prompt keeps too many side details.
- Sentence prompt overclaims.
- Methods prompt ignores validation and processing consistency.
- Story prompt creates a broader claim than the evidence supports.
