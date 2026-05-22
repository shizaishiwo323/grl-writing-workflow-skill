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
2. Test `mechanism_results_prompt.md` on one Results paragraph that originally described spectra or tortuosity.
3. Test `paragraph_engineering_prompt.md` on one paragraph with mixed function.
4. Test `sentence_hierarchy_prompt.md` only after the same paragraph's logic is stable.
5. Test `ocar_funnel_prompt.md` on Abstract or Introduction.
6. Test `methods_evidence_chain_prompt.md` on the RTM or NMR Methods paragraph.
7. Test `story_architect_prompt.md` on title + abstract + introduction.

## Narrative Echo Tests

Test 1: Introduction promise without payoff

Input:
An Introduction emphasizes a concept that never appears in Results.

Expected output:
Identify the orphan promise and suggest deletion, merging, or adding a Results payoff.

Test 2: Result without foreshadowing

Input:
A Results section introduces a major metric suddenly.

Expected output:
Suggest a short foreshadowing sentence in Introduction or the previous Results subsection.

Test 3: Weak Results subsection transition

Input:
Section 3.1 ends abruptly and Section 3.2 begins as an unrelated result.

Expected output:
Suggest one forward pointer at the end of 3.1 and one backward link at the beginning of 3.2.

Test 4: Missing thread summary

Input:
Several Results subsections each describe useful findings, but no sentence connects them.

Expected output:
Suggest a 1-2 sentence thread summary that turns the results into a mechanism chain.

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
