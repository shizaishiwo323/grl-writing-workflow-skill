# paragraph_engineering

## Skill Objective

Repair paragraph-level function: topic sentence, evidence order, mechanism chain, and paragraph ending.

Story Architect Gate: Before applying this skill, confirm that `story_architect` has identified the main character and supporting actors. Do not repair paragraph flow if the manuscript's central story is still unclear.

## Input

- One paragraph or a short sequence of paragraphs.
- Optional target OCAR role.

## Output

- Paragraph function diagnosis.
- Topic sentence rewrite.
- Evidence order recommendation.
- Sentences to delete, move, compress, or merge.
- Final takeaway sentence.

## When to Call / When Not to Call

**When to call:**

- A paragraph has useful content but no clear function.
- Topic sentence, evidence order, or final takeaway is weak.
- A paragraph mixes background, method, result, and implication.

**When not to call:**

- The whole-paper storyline is still unresolved.
- The section-level OCAR movement is broken.
- The only problem is local word choice or grammar.

## Core Principles

- P7: Start Paragraphs With Their Function.
- P10: Remove Detail That Arrives Before Its Function.
- P8: Use Independent Evidence To Support The Main Signal.
- P4: Define The Challenge As A Process-Based Link.

## Detection Logic

Look for:

- Paragraph starts with detail rather than function.
- More than one topic competes inside the same paragraph.
- The last sentence points to a different topic than the first sentence.
- Technical side-notes interrupt the main logic.
- Evidence is listed before the reader knows why it matters.

## Rewrite Logic

1. Assign the paragraph one function: orient, define, compare, validate, interpret, or conclude.
2. Write a topic sentence that names that function.
3. Order details from most central to most supporting.
4. Move or delete details that belong to another paragraph.
5. End with a sentence that returns to the paragraph function.

## Case-Guided Diagnosis

For full reference cases, see `references/cases_paragraph_engineering.md`. Use those cases before rewriting paragraphs, especially when diagnosing topic sentence failure, evidence-order failure, mechanism-buried paragraphs, paragraph-to-paragraph echo, or weak mini-implication endings.

Match the paragraph to one primary case type:

- `PE-TOPIC`: function-first topic sentence.
- `PE-ORDER`: evidence order.
- `PE-MECH`: observation-to-mechanism paragraph.
- `PE-ECHO`: paragraph-to-paragraph echo.
- `PE-END`: mini-implication ending.
- `PE-COMPRESS`: detail compression / detail repositioning.

Use the case type to decide the first operation:

- If `PE-TOPIC`, repair the opening sentence before editing details.
- If `PE-ORDER`, reorder evidence before polishing sentences.
- If `PE-MECH`, insert or foreground the physical mechanism chain.
- If `PE-ECHO`, inspect previous and next paragraphs before revising the target paragraph.
- If `PE-END`, rewrite the final sentence so it returns to the paragraph function.
- If `PE-COMPRESS`, move or delete details whose function belongs elsewhere.

## Paragraph-to-Paragraph Echo

A strong Results paragraph should not stand alone.

It should:

1. inherit the previous paragraph's unresolved question;
2. advance the mechanism by one clear step;
3. prepare the next paragraph or subsection when the argument continues.

Avoid isolated paragraphs that only describe one figure, one metric, or one phenomenon.

When revising a paragraph, check:

- Does this paragraph connect to the previous paragraph?
- Does it create a logical need for the next paragraph?
- Does it end with a mini-implication?
- Is the paragraph part of a larger mechanism chain?

## Forbidden Patterns

- One paragraph doing background, method, result, and implication at once.
- Long technical explanation before the gap or result is established.
- Ending with a new topic.
- Keeping correct but low-function detail in the main paragraph.

## Example Cases

Full case library: `references/cases_paragraph_engineering.md`.

Case ID: R-011

Source Principle: P7

Before: `The evolution of system tortuosity delineates the optimization of flow pathways across dissolution patterns.`

After: `Flow field tortuosity \\tau is defined based on velocity ratios (Text S3) and provides an independent hydraulic reference to evaluate whether the T2-derived spectral evolution reflects flow path optimization.`

Use: The revised topic sentence assigns tortuosity a function in the argument.
