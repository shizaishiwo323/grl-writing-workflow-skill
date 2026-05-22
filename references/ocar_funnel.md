# ocar_funnel

## Skill Objective

Repair section-level OCAR movement: Opening, Challenge, Action, Resolution. Use this especially for Abstract and Introduction.

OCAR can operate at multiple scales: Abstract, Introduction, Methods opening, Results opening, subsection opening, and paragraph. Do not restrict OCAR to the Introduction only.

## Input

- Abstract, Introduction, section opening, or paragraph sequence.
- Optional target journal and central claim.

## Output

- OCAR diagnosis.
- Missing or weak OCAR component.
- Suggested section-level structure.
- Rewritten topic sentences for each OCAR move.

## When to Call / When Not to Call

**When to call:**

- Abstract or Introduction lacks a clear Opening, Challenge, Action, or Resolution.
- The text jumps from broad background to methods without a process-based gap.
- Details appear before readers know the section's problem.

**When not to call:**

- The OCAR movement is already clear and only sentence flow is weak.
- The target text is a Methods workflow paragraph.
- The user asks to interpret a specific result figure.

## Core Principles

- P3: Open With A Process, Not A List.
- P4: Define The Challenge As A Process-Based Link.
- P2: Keep One Storyline Across OCAR.
- P10: Remove Detail That Arrives Before Its Function.

## Detection Logic

Check whether:

- Opening begins with a physical process and consequence.
- Challenge identifies a missing process-based link, not a generic research gap.
- Action states what the study tests, builds, or compares.
- Resolution states what the results reveal and how readers can use it.
- Details appear before readers know why they matter.

## Rewrite Logic

1. Compress broad background to one process-first sentence.
2. Add why the process matters for flow, transport, signal, or risk.
3. State what current methods cannot translate or diagnose.
4. Introduce the study as an action that resolves that missing link.
5. Remove regime-specific or technical detail that arrives before its function.

## Forbidden Patterns

- Opening with a list of applications before naming the process.
- "Few studies..." as the main gap.
- Introducing detailed mechanisms before the Challenge is established.
- Ending the Introduction with a method list but no contribution sentence.

## Example Cases

For reference-paper examples, see `references/cases_ocar_funnel.md`.

Case ID: I-001

Source Principle: P3

Before: `Mineral dissolution widely occurs in natural and engineering processes...`

After: `Mineral dissolution reshapes pore networks through spatiotemporally variable pathways, influencing flow and transport evolution...`

Use: The revised Opening starts with the process and its consequence before examples.
