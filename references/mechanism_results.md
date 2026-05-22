# mechanism_results

## Skill Objective

Turn Results and Discussion from figure description into mechanism interpretation.

Story Architect Gate: Before applying this skill, confirm that `story_architect` has identified the main character and supporting actors. Do not polish or reorganize Results if the manuscript's central story is still unclear.

## Input

- Results paragraph, figure caption, figure observations, or discussion draft.
- Optional central claim and relevant method outputs.

## Output

- Observation-mechanism map.
- Weak result paragraphs that only describe figures.
- Suggested mechanism-centered rewrites.
- Literature comparison placement if needed.

## When to Call / When Not to Call

**When to call:**

- Results describe figures, trends, or numbers without explaining mechanism.
- Regime comparisons are visual or chronological rather than physical.
- Literature needs to clarify the new contribution of a result.

**When not to call:**

- The issue is missing method validation or parameter reproducibility.
- The user only needs sentence polish after mechanism logic is stable.
- The section lacks a central claim and needs `story_architect` first.

## Core Principles

- P6: Results Must Translate Patterns Into Mechanisms.
- P7: Start Paragraphs With Their Function.
- P9: Let Literature Serve The Current Result.
- P11: Prefer Physical Verbs Over Generic Reporting Verbs.

## Detection Logic

Look for:

- Sentences beginning with "Figure shows" but not explaining why it matters.
- Numbers reported without a process interpretation.
- Regime comparisons based on appearance rather than mechanism.
- Literature inserted broadly instead of clarifying the current result's contribution.
- Paragraphs ending with a measurement instead of a scientific judgment.

## Rewrite Logic

For each result paragraph:

1. Name the result pattern.
2. State the physical mechanism.
3. Connect the mechanism to the main claim.
4. Use quantitative values only where they support the mechanism.
5. End with a takeaway sentence.

Preferred form:

```text
[Observed signal/pathway] indicates [mechanism], because [physical reason], leading to [consequence].
```

## Results Echo Requirement

Results subsections should not read as independent result blocks.

Each subsection should do at least one of the following:

1. inherit a question from the previous subsection;
2. prepare a later mechanism;
3. test a previous interpretation;
4. quantify a previously described pattern;
5. synthesize earlier findings into the next step of the mechanism chain.

Before revising a Results subsection, check:

- What previous result does this subsection build on?
- What later result does this subsection prepare?
- Does the opening sentence include a backward link when needed?
- Does the ending sentence include a forward pointer when needed?
- Does the subsection end with a mechanism-oriented mini-summary rather than only data?

## Case-Derived Rules

Use `references/cases_mechanism_centered_results.md` when a Results task needs concrete examples of mechanism-centered writing.

1. Results paragraphs should convert observations into mechanisms, not merely describe figures.
2. A metric should be introduced only after the mechanism question requiring that metric is clear.
3. Secondary metrics should validate or constrain the main interpretation, not compete with the central storyline.
4. Regime comparisons should be organized around the physical process that causes divergence among regimes.
5. Transient signal behavior should be written as a transition between physical states, not as a time-series description alone.
6. Bulk geophysical metrics should be connected to pore-scale redistribution of flux, exchange, coupling, or connectivity.
7. Breakthrough curves, spectra, and profile shapes should be mapped to physical pathways, storage zones, exchange processes, or flow structures.
8. Each Results subsection should end with a mechanism-oriented mini-synthesis when it prepares the next step.

## Reference Case Library

Load the case library especially for these patterns:

- Observation to mechanism: `MCR-SELF-002`, `MCR-REF-2018-003`, `MCR-REF-2025-001`, `MCR-REF-2026-001`.
- Structure to signal: `MCR-SELF-002`, `MCR-SELF-003`, `MCR-REF-2026-001`, `MCR-REF-2026-002`.
- Metric validation: `MCR-SELF-004`, `MCR-SELF-005`, `MCR-REF-2024-001`, `MCR-REF-2026-002`.
- Regime comparison: `MCR-SELF-001`, `MCR-REF-2024-002`, `MCR-REF-2025-003`.
- Breakthrough or transition mechanism: `MCR-SELF-003`, `MCR-SELF-005`, `MCR-REF-2025-001`.
- Mini synthesis: `MCR-SELF-005`, `MCR-REF-2025-003`, `MCR-REF-2026-002`.

## Forbidden Patterns

- Pure chronological figure description.
- Listing peak shifts without saying what they mean.
- Saying "consistent with" without explaining the connection.
- Adding literature that does not sharpen the paper's contribution.

## Example Cases

Case ID: R-008

Source Principle: P6

Before: `This transient bimodality indicates that channeling achieves early permeability breakthrough with limited matrix dissolution.`

After: `This transient bimodality followed by rapid peak merging indicates that channeling achieves early permeability breakthrough through efficient conduit formation with limited matrix dissolution.`

Use: The revised sentence connects spectral evolution to conduit formation and breakthrough.
