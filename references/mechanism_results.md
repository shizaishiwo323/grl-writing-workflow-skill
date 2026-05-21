# mechanism_results

## Skill Objective

Turn Results and Discussion from figure description into mechanism interpretation.

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
