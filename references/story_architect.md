# story_architect

## Skill Objective

Determine the central scientific story before any section-level or sentence-level revision. This skill builds or repairs the whole-paper storyline so the title, abstract, introduction, methods, results, discussion, conclusions, and figure sequence all point to one mechanism-centered claim.

Use `references/cases_story_architect.md` for concrete examples from high-quality papers and the current manuscript.

## Input

- Title, key points, abstract, introduction, or whole manuscript.
- Figure sequence, figure captions, and main results.
- Optional target journal constraints, usually GRL.

## Output

- One-sentence Core Story.
- Central Scientific Question.
- Main Character and Supporting Actors.
- Potential Distractions that should be downgraded or moved to SI.
- Section-Level Storyline table.
- Figure Sequence Logic table.
- Transferable Rule for similar manuscripts.

## When to Call / When Not to Call

**When to call:**

- The user is unsure what the manuscript is really about.
- The manuscript contains many results but no clear central claim.
- Figures, methods, and metrics feel like parallel work packages.
- Introduction, Results, and Discussion appear to emphasize different things.
- The user asks whether the manuscript is suitable for GRL.
- The central claim cannot be stated in one mechanism-centered sentence.
- The manuscript reads like a list of work done rather than a coherent scientific argument.

**When not to call:**

- The storyline is stable and only paragraph order or sentence clarity is weak.
- The user only provides a single mature sentence for polishing.
- The immediate issue is method reproducibility after the central story is already clear.

## Core Principles

### Rule 1: Identify the main character

Every paper should have one main scientific object: a mechanism, process, contrast, diagnostic relationship, or controlling variable. The main character is what readers should remember after forgetting most details.

### Rule 2: Separate main story from supporting actors

Methods, metrics, figures, validation checks, and comparison cases should support the main story rather than become parallel stories.

### Rule 3: Define the central question before improving wording

Do not polish sentences before the paper can be summarized as one central scientific question and one core story.

### Rule 4: Align section functions with the story

Introduction defines the problem; Methods justify how the problem can be answered; Results build the evidence chain; Discussion explains significance; Conclusions state the durable take-home message.

### Rule 5: Use figure sequence as storyline evidence

A strong figure sequence should move from framework or concept, to core observation, to mechanism, quantification, or implication. If figures only list outputs, the paper likely lacks story architecture.

### Rule 6: Protect GRL concision

Move technical details to SI when they support credibility but do not advance the main story. The main text should tell the story; SI should carry reproducibility, parameters, validation details, and secondary checks.

## Do Not Confuse

- Main character is not necessarily the method.
- Main character is not necessarily the newest metric.
- Supporting actor is not unimportant; it is important because it serves the main character.
- A paper can contain several results, but it should not contain several competing stories.
- A strong story is not a slogan; it must be supported by section sequence and figure sequence.

## Extraction Checklist

For each manuscript or reference paper, answer only these questions:

1. What is the one-sentence Core Story?
2. What Central Scientific Question does the paper answer?
3. What is the Main Character?
4. Which methods, metrics, and figures are Supporting Actors?
5. Which content could become a Potential Distraction?
6. How do Abstract, Introduction, Methods, Results, Discussion, and Conclusion serve the same story?
7. Does the figure sequence show framework -> phenomenon -> mechanism -> implication?
8. What transferable writing rule can be learned?

## Detection Logic

Look for:

- Title starts with a tool rather than the physical process or diagnostic relationship.
- Abstract lists work done but does not state a testable scientific action.
- Introduction gap differs from the Results mechanism.
- Methods, metrics, and validation outputs appear as separate products rather than one evidence chain.
- Figures are ordered by workflow convenience rather than argument function.
- Final claim is broader than the evidence or target journal allows.
- SI-worthy technical details compete with the main-text story.

## Failure Signals

The manuscript likely needs Story Architect if:

- Abstract emphasizes a method, but Discussion emphasizes an application.
- Introduction gap is about one problem, but Results mainly answer another.
- Each figure can be explained alone, but the figure sequence has no cumulative logic.
- A new metric appears as a product, not as the answer to a defined problem.
- Results contain many values but no controlling mechanism.
- SI-level method details are needed to understand the main claim.

## Rewrite Logic

1. Identify the main physical process, diagnostic relationship, or controlling contrast.
2. Identify the central question the manuscript answers.
3. Identify the main character and supporting actors.
4. Convert methods and metrics into evidence roles: reveal, validate, quantify, or explain.
5. Rewrite the central storyline in one sentence.
6. Align title, abstract, section openings, and figure sequence around that sentence.
7. Downgrade technical details that support credibility but do not advance the story.

Preferred storyline forms:

```text
We show/test how [measurable signal] tracks [physical process] by revealing [mechanism], which explains [scientific or practical consequence].
```

```text
[Process or regime] changes [controlling variable], which produces [observable behavior] and explains [broader implication].
```

## Output Template

```markdown
## Core Story

## Central Scientific Question

## Main Character

## Supporting Actors

## Potential Distractions

## Section-Level Storyline

## Figure Sequence Logic

## Transferable Rule

## Next Writing Operation
```

## Forbidden Patterns

- "This paper studies..." without mechanism.
- Method-first title when the result is process-first.
- Multiple central claims competing for attention.
- Treating a new metric as the story rather than evidence for the story.
- Polishing sentences while the main character is still unclear.
- Letting SI-level method details dominate a GRL main text.

## Reference Cases

See `references/cases_story_architect.md`.

Most reusable case patterns:

- NMR dissolution manuscript: signal -> pore coupling -> breakthrough efficiency.
- Niu and Zhang 2018: empirical parameter -> pore-throat electric-field mechanism -> universal correlation.
- Szawello et al. 2024: visual classification failure -> dynamic flow focusing profile -> regime distinction.
- Deng et al. 2025: dissolution regime -> flow heterogeneity -> Fickian/non-Fickian transport transition.
- Zhou et al. 2026: saturation -> water-pathway tortuosity/connectivity -> NMR-visible pore coupling.
