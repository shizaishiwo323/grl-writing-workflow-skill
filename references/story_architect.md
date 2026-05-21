# story_architect

## Skill Objective

Build or repair the whole-paper scientific storyline so that the title, abstract, introduction, methods, and results point to one mechanism-centered claim.

## Input

- Title, abstract, introduction, or whole manuscript.
- Optional figures and key results.
- Optional target journal constraints.

## Output

- One-sentence central claim.
- Storyline spine: `Problem -> Gap -> Action -> Evidence -> Mechanism -> Implication`.
- Drift points where sections pursue side stories.
- Suggested high-level rewrites for title, abstract, and section openings.

## When to Call / When Not to Call

**When to call:**

- The central claim cannot be stated in one mechanism-centered sentence.
- Title, abstract, introduction, and results emphasize different stories.
- The manuscript reads like a list of work done rather than a coherent scientific argument.

**When not to call:**

- The storyline is stable and only paragraph order or sentence clarity is weak.
- The user only provides a single mature sentence for polishing.
- The immediate issue is method reproducibility, not story architecture.

## Core Principles

- P1: Make The Title Carry The Main Scientific Action.
- P2: Keep One Storyline Across OCAR.
- P6: Results Must Translate Patterns Into Mechanisms.
- P12: Calibrate Claims To The Evidence.

## Detection Logic

Look for:

- Title starts with a tool rather than the physical process.
- Abstract lists work done but does not state a testable scientific action.
- Introduction gap differs from the Results mechanism.
- Methods, MVC, tortuosity, and NMR appear as separate products rather than one evidence chain.
- Final claim is broader than the representative cases.

## Rewrite Logic

1. Identify the main physical process.
2. Identify the diagnostic signal or evidence type.
3. Identify the mechanism the paper reveals.
4. Rewrite the central storyline in one sentence.
5. Align title and abstract around that sentence.

Preferred storyline form:

```text
We show/test how [measurable signal] tracks [physical process] by revealing [mechanism], which explains [scientific or practical consequence].
```

## Forbidden Patterns

- "This paper studies..." without mechanism.
- Method-first title when the result is process-first.
- Multiple central claims competing for attention.
- Treating a new metric as the story rather than evidence for the story.

## Example Cases

Case ID: T-001

Source Principle: P1

Before: `Nuclear Magnetic Resonance for Spatiotemporal Tracking of Pore Coupling During Mineral Dissolution`

After: `Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures`

Use: The revised title makes the physical process and diagnostic evidence carry the story.
