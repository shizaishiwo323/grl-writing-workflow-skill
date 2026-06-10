# Journal Profile

Use this file before applying concision, Supporting Information, or reviewer-fit rules. The core workflow stays the same across journals:

```text
storyline > structure > narrative echo > mechanism > paragraph > sentence > word choice
```

The journal profile only changes how much evidence, method detail, validation, uncertainty, and discussion should remain in the main text.

## Default Rule

- If the user gives a target journal, apply that profile.
- If the target journal is unspecified, infer from the user's goal only when it is obvious.
- If the target journal is unclear and the edit depends on article length, ask or state the assumption before enforcing GRL-style concision.
- Do not move technical detail to Supporting Information merely because it is detailed. Move it only when it does not help the main claim, target journal, or reader trust.

## GRL

- Short, high-impact, mechanism-centered.
- Strongly prioritize one central claim and one clean evidence chain.
- Keep the main text focused on the result, mechanism, and broad implication.
- Move secondary parameter sweeps, implementation details, extended validation, and side analyses to Supporting Information when they support credibility but do not advance the main story.
- Avoid long literature inventories, extended method exposition, and diffuse multi-claim Discussion sections.

## JGR / JGR: Solid Earth

- Full-length AGU Research Article.
- Preserve detailed methods, parameter definitions, validation logic, uncertainty analysis, and mechanism discussion when they are needed for reproducibility or reader trust.
- Do not over-compress Results and Discussion into only a GRL-style mechanism sketch.
- The storyline should remain clear and mechanism-centered, but supporting evidence can be developed more fully than in GRL.
- Use Supporting Information for exhaustive derivations, supplementary cases, or implementation details, not for evidence that the main claim needs in order to be credible.

## WRR

- Full-length hydrology and water-resources research article.
- Emphasize process understanding, model/data credibility, reproducibility, uncertainty, and broader water-resources implications.
- Methods, validation, and uncertainty usually need more main-text space than in GRL.
- Maintain a clear process-centered storyline, but allow fuller explanation of assumptions, parameter choices, boundary conditions, and practical implications.
- Do not reduce hydrologic significance to a single broad implication if the paper requires a careful link to water-resources context.

## Generic AGU Research Article

- Use when the target is AGU but not clearly GRL, JGR, or WRR.
- Preserve the GRL-derived strengths: strong central story, OCAR funnel, mechanism chain, paragraph function, and calibrated claims.
- Avoid GRL-specific compression unless the user wants a short-format article.
- Keep enough method, evidence, validation, uncertainty, and discussion in the main text for a full research article.

## Output Requirement

When a request could be affected by journal type, include:

```text
Target journal profile:
Concision strategy:
Main-text evidence to preserve:
Details that can move to Supporting Information:
```
