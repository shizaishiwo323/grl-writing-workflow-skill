# methods_evidence_chain

## Skill Objective

Make Methods function as an evidence chain: workflow coupling, parameter reproducibility, validation, and processing consistency.

## Input

- Methods section or method paragraph.
- Model workflow, parameter table, figure schematic, or signal-processing description.

## Output

- Method evidence-chain diagnosis.
- Missing input-output links.
- Missing parameter controls, units, or sources.
- Missing validation or processing-consistency statements.
- Suggested method paragraph rewrites.

## When to Call / When Not to Call

**When to call:**

- Methods list modules but do not explain handoff between inputs and outputs.
- Parameters, units, controls, sources, or boundary conditions are underspecified.
- Validation is qualitative or signal processing consistency is missing.

**When not to call:**

- The problem is the paper-wide storyline rather than Methods evidence.
- The user asks to interpret Results figures.
- The Methods are stable and only sentence-level wording is awkward.

## Core Principles

- P5: Make Methods Answer "Why This Workflow Can Prove The Claim".
- P5a: State the workflow as input-output coupling.
- P5b: Define parameters with units, controls, and sources.
- P5c: State processing consistency when interpreting signal changes.
- P8: Use Independent Evidence To Support The Main Signal.

## Detection Logic

Look for:

- Modules listed without handoff: what output from one module becomes input to the next?
- Parameter definitions without units, controls, fixed values, or source references.
- Validation described qualitatively without numerical or observable comparison.
- Signal processing or inversion described without consistency controls.
- SI references that do not say what reproducibility detail they contain.

## Rewrite Logic

Use this sequence:

1. Workflow: `input -> model/process -> output -> comparison`.
2. Parameters: define each important variable with role, unit, control method, and source.
3. Validation: state benchmark target, measured agreement, and what model capacity it supports.
4. Processing: state settings kept constant and what artifacts are excluded.
5. Pairing: explain which outputs are synchronized for direct comparison.

## Forbidden Patterns

- "Details are in Text S1" without saying what details.
- Equations without parameter meaning or units.
- Validation that only says "consistent with" but gives no observable.
- Treating signal changes as physical changes without processing-control statement.

## Example Cases

Case ID: M-009

Source Principle: P5

Before: `The comparison focused on shared observables... and supports the parameter choices...`

After: `After normalizing for different initial porosities, the mean absolute difference... was minimal, and the time for complete dissolution... is comparable (4.26 h experimentally and 4.28 h numerically).`

Use: The revised method gives quantitative validation rather than generic support.
