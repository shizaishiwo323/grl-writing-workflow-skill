# sentence_hierarchy

## Skill Objective

Polish sentence-level hierarchy after storyline, section logic, and paragraph function are stable.

## Input

- Sentence, paragraph, or marked-up draft.
- Optional desired tone: GRL concise, mechanism-forward, or claim-calibrated.

## Output

- Sentence-level problems.
- Revised sentence options.
- Explanation of what changed: physical verb, sequence, claim strength, or information order.

## When to Call / When Not to Call

**When to call:**

- Storyline, section logic, and paragraph function are stable.
- The sentence is clumsy, static, overclaimed, or physically vague.
- The user explicitly asks for sentence-level polishing after logic review.

**When not to call:**

- Central claim is unclear.
- Paragraph lacks evidence or has no topic function.
- Section OCAR is broken.

## Core Principles

- P11: Prefer Physical Verbs Over Generic Reporting Verbs.
- P12: Calibrate Claims To The Evidence.
- P7: Start Paragraphs With Their Function.

## Detection Logic

Look for:

- Generic verbs: occurs, provides, shows, is used, has, demonstrates.
- Long noun stacks that hide the physical action.
- Multiple mechanisms in one sentence without order.
- Claims broader than the data.
- Weak temporal or causal connectors.

## Rewrite Logic

1. Put the physical actor near the subject position.
2. Replace generic verbs with process verbs when accurate.
3. Use temporal connectors for evolution: initially, as, then, thereafter.
4. Use causal connectors for mechanism: because, therefore, indicating, reflecting.
5. Soften claims when evidence is representative or model-bound.

## Forbidden Patterns

- Polishing sentences before fixing missing evidence.
- Making claims stronger just to sound confident.
- Hiding the mechanism behind abstract nouns.
- Using elegant phrasing that reduces physical precision.

## Example Cases

Case ID: I-001

Source Principle: P11

Before: `Mineral dissolution widely occurs in natural and engineering processes...`

After: `Mineral dissolution reshapes pore networks through spatiotemporally variable pathways...`

Use: The revised sentence uses a physical verb and makes the process visible.
