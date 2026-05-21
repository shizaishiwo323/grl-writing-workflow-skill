# GRL Scientific Writing Principle Library

Source: `../01_modification_mining/modification_database.xlsx`

This library is abstracted from the current 60-record modification database. It should be treated as the first principle layer, not the final skill implementation.

Revision note: this file keeps the original 12 principles, then applies later refinements: evidence strength, method sub-principles, and a workflow-level meta principle before Phase 3.

## Contents

- Frequency Signal
- Evidence Strength Guide
- Principle Evidence Matrix
- Meta Principle
- Macro-Level Principles
- Section-Level Principles
- Paragraph-Level Principles
- Sentence-Level Principles
- Layer Map
- How To Use This Library In The Next Phase

## Frequency Signal

| Tag | Count | What It Suggests |
|---|---:|---|
| `mechanism_emphasis` | 38 | The paper must explain physical mechanisms, not only report patterns. |
| `topic_sentence_insertion` | 27 | Paragraphs need clear functional openings. |
| `reader_guidance` | 26 | The reader must be guided through figures, variables, and logic. |
| `physics_first` | 21 | Physical variables and process links should lead the prose. |
| `storyline_alignment` | 18 | Title, abstract, introduction, and results must point to one story. |
| `funnel_narrowing` | 14 | The introduction must move from broad relevance to a specific unresolved gap. |
| `result_interpretation` | 13 | Results must be translated into scientific meaning. |
| `method_reproducibility` | 10 | Methods must explain enough for trust and reproducibility. |

## Evidence Strength Guide

| Strength | Meaning |
|---|---|
| Strong | Repeated across many records and/or multiple sections. Safe to use as a core writing principle. |
| Medium | Clearly present, but supported by fewer records or concentrated in one section. Keep, but continue collecting cases. |
| Emerging | Important and plausible, but current evidence comes from only a few records. Treat as a hypothesis for later validation. |

## Principle Evidence Matrix

| Principle | Primary Level | Secondary Level | Evidence Strength |
|---|---|---|---|
| P1 Make The Title Carry The Main Scientific Action | Macro | Sentence | Medium |
| P2 Keep One Storyline Across OCAR | Macro | Section | Strong |
| P3 Open With A Process, Not A List | Section | Sentence | Strong |
| P4 Define The Challenge As A Process-Based Link | Section | Paragraph | Strong |
| P5 Make Methods Answer "Why This Workflow Can Prove The Claim" | Section | Paragraph | Strong |
| P6 Results Must Translate Patterns Into Mechanisms | Section | Paragraph | Strong |
| P7 Start Paragraphs With Their Function | Paragraph | Sentence | Strong |
| P8 Use Independent Evidence To Support The Main Signal | Paragraph | Section | Emerging |
| P9 Let Literature Serve The Current Result | Paragraph | Section | Medium |
| P10 Remove Detail That Arrives Before Its Function | Paragraph | Section | Medium |
| P11 Prefer Physical Verbs Over Generic Reporting Verbs | Sentence | Paragraph | Strong |
| P12 Calibrate Claims To The Evidence | Sentence | Macro | Emerging |

## Meta Principle

### Meta Principle 0: Diagnose The Manuscript Stage Before Editing

**Description:** Before editing, identify whether the manuscript problem is storyline, section logic, paragraph architecture, or sentence expression.

**Why:** Many weak edits happen when sentence polishing is applied before the paper's OCAR structure and mechanism storyline are stable.

**Editing Order:**

1. If the central claim is unclear, work on story architecture first.
2. If the OCAR movement is weak, repair Opening, Challenge, Action, and Resolution before polishing.
3. If sections are stable but paragraphs drift, revise topic sentences, evidence order, and paragraph function.
4. If the logic is stable, then polish sentence hierarchy, verbs, transitions, and claim strength.
5. Before submission, run a reviewer-oriented pass: scope, evidence boundaries, method reproducibility, and overclaim checks.

**Applicable Sections:** Whole manuscript and all future skill routing.

**Common Failure Modes:**

- Polishing grammar while the paper still lacks a central mechanism.
- Asking a sentence-level skill to fix a section-level gap.
- Designing too many skills before knowing which editing stage the manuscript is in.

**Primary Level:** Macro

**Secondary Level:** Workflow

**Evidence Strength:** Workflow principle, not counted as a normal writing principle.

## Macro-Level Principles

### Principle 1: Make The Title Carry The Main Scientific Action

**Description:** The title should foreground the scientific process and diagnostic contribution, not merely name the tool.

**Why:** In a GRL-style paper, the title is the first storyline filter. It should tell readers what is being tracked, by what kind of evidence, and why the result is not just an application of a method.

**Before/After Example:**

Before: `Nuclear Magnetic Resonance for Spatiotemporal Tracking of Pore Coupling During Mineral Dissolution`

After: `Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures`

**Applicable Sections:** Title, Abstract, Introduction.

**Common Failure Modes:**

- Starting with the instrument instead of the physical process.
- Making the title sound like a method application rather than a science result.
- Hiding the quantitative signal or diagnostic contribution.

**Source Tags:** `storyline_alignment`, `mechanism_emphasis`, `physics_first`

**Primary Level:** Macro

**Secondary Level:** Sentence

**Evidence Strength:** Medium

### Principle 2: Keep One Storyline Across OCAR

**Description:** The paper should move through one continuous logic: why the problem matters, what gap blocks understanding, what action the study takes, and what mechanism the results reveal.

**Why:** The teacher's edits repeatedly align title, abstract, introduction, methods, and results around the same spine: NMR signatures track dissolution dynamics by revealing matrix-vug exchange and hydraulic pathway reorganization.

**Before/After Example:**

Before: `Here, we interpret transient nuclear magnetic resonance (NMR) $T_2$ distributions as signatures of dissolution-driven pore coupling.`

After: `Here, we test whether quantitative nuclear magnetic resonance (NMR) signatures can diagnose carbonate dissolution dynamics.`

**Applicable Sections:** Title, Abstract, Introduction, Results and Discussion.

**Common Failure Modes:**

- Describing the work done without framing a testable scientific question.
- Letting different sections emphasize different main stories.
- Treating NMR, MVC, tortuosity, and permeability as separate outputs instead of linked evidence.

**Source Tags:** `storyline_alignment`, `topic_sentence_insertion`, `reader_guidance`

**Primary Level:** Macro

**Secondary Level:** Section

**Evidence Strength:** Strong

## Section-Level Principles

### Principle 3: Open With A Process, Not A List

**Description:** The opening should begin with the physical process and its consequence before listing examples or regimes.

**Why:** A list of applications tells readers the topic is broad; a process sentence tells them what the paper is scientifically about.

**Before/After Example:**

Before: `Mineral dissolution widely occurs in natural and engineering processes, including calcite dissolution in karst erosion...`

After: `Mineral dissolution reshapes pore networks through spatiotemporally variable pathways, influencing flow and transport evolution in many natural and engineering processes...`

**Applicable Sections:** Introduction Opening, Abstract Opening.

**Common Failure Modes:**

- Opening with examples before the controlling physical process.
- Listing regimes before explaining why regimes matter.
- Treating background as a literature inventory rather than a funnel.

**Source Tags:** `funnel_narrowing`, `topic_sentence_insertion`, `mechanism_emphasis`

**Primary Level:** Section

**Secondary Level:** Sentence

**Evidence Strength:** Strong

### Principle 4: Define The Challenge As A Process-Based Link

**Description:** The gap should identify the missing link between measurable signals and evolving physical processes.

**Why:** The strongest challenge is not "few people have studied this." It is "current measurements do not yet translate into the process we need to understand."

**Before/After Example:**

Before: `Thus, despite substantial progress in classifying dissolution patterns, a field-applicable framework that continuously translates geophysical responses into specific dissolution regimes remains lacking.`

After: `Geophysical methods can monitor mineral dissolution non-invasively over larger spatial and temporal scales... The central challenge is therefore to establish process-based links between measurable geophysical signals and the spatiotemporal evolution of dissolution regimes.`

**Applicable Sections:** Introduction Challenge, Abstract Challenge.

**Common Failure Modes:**

- Writing the gap as a generic lack of studies.
- Jumping from prior work to the new method without explaining the missing link.
- Stating the tool's promise without saying what physical process it must diagnose.

**Source Tags:** `funnel_narrowing`, `reader_guidance`, `storyline_alignment`

**Primary Level:** Section

**Secondary Level:** Paragraph

**Evidence Strength:** Strong

### Principle 5: Make Methods Answer "Why This Workflow Can Prove The Claim"

**Description:** Methods should not only list procedures; they should show how each module produces evidence for the central claim.

**Why:** In this paper, the reactive-transport model, NMR forward model, inversion, permeability, tortuosity, and MVC are not separate technical blocks. They form a proof chain.

**Before/After Example:**

Before: `The NMR simulation module then uses each time-stamped geometry as the forward-simulation domain and converts it into whole-domain and segment-wise $T_2$ distributions...`

After: `At selected dissolution stages, the resulting pore geometries are passed to the NMR forward model to generate whole-domain bulk $T_2$ distributions and spatially resolved $T_2$ profiles... enabling direct comparison among pore-structure evolution, hydraulic properties, and NMR observables.`

**Applicable Sections:** Methods, Results setup.

**Common Failure Modes:**

- Listing modules without explaining how information passes between them.
- Omitting synchronized outputs that let readers trust comparisons.
- Treating methods as procedural background rather than evidence architecture.

**Sub-Principles:**

- **5a. State the workflow as input-output coupling.** Write the method as a chain of inputs, transformations, and outputs, such as geometry snapshots passed into NMR forward modeling.
- **5b. Define parameters with units, controls, and sources.** For key variables such as Pe, Da, reaction constants, and boundary conditions, state what was varied, what was fixed, what the units mean, and where values come from.
- **5c. State processing consistency when interpreting signal changes.** If signal changes support a physical interpretation, explain how inversion settings, processing choices, or numerical procedures were kept consistent.

**Source Tags:** `method_reproducibility`, `reader_guidance`, `evidence_chain`

**Primary Level:** Section

**Secondary Level:** Paragraph

**Evidence Strength:** Strong

### Principle 6: Results Must Translate Patterns Into Mechanisms

**Description:** Every result paragraph should convert observed trends into a physical interpretation.

**Why:** For GRL, reporting that peaks shift, merge, or separate is not enough. The reader needs to know what those changes mean for pore coupling, flow-path development, and breakthrough.

**Before/After Example:**

Before: `This transient bimodality indicates that channeling achieves early permeability breakthrough with limited matrix dissolution.`

After: `This transient bimodality followed by rapid peak merging indicates that channeling achieves early permeability breakthrough through efficient conduit formation with limited matrix dissolution.`

**Applicable Sections:** Results and Discussion, Abstract Resolution.

**Common Failure Modes:**

- Ending a result paragraph with a measurement rather than an interpretation.
- Describing spectral morphology without linking it to hydraulic behavior.
- Comparing regimes by appearance rather than mechanism.

**Source Tags:** `result_interpretation`, `mechanism_emphasis`, `physics_first`

**Primary Level:** Section

**Secondary Level:** Paragraph

**Evidence Strength:** Strong

## Paragraph-Level Principles

### Principle 7: Start Paragraphs With Their Function

**Description:** A paragraph should quickly announce whether it is orienting the reader, defining a variable, reporting a pattern, validating a method, or interpreting a mechanism.

**Why:** Teacher edits often insert or strengthen topic sentences so that readers can follow the purpose of each paragraph before entering details.

**Before/After Example:**

Before: `The evolution of system tortuosity delineates the optimization of flow pathways across dissolution patterns.`

After: `Flow field tortuosity $\\tau$ is defined based on velocity ratios (Text S3) and provides an independent hydraulic reference to evaluate whether the $T_2$ derived spectral evolution reflects flow path optimization.`

**Applicable Sections:** Methods, Results and Discussion, Introduction Challenge.

**Common Failure Modes:**

- Beginning with a result but not saying why it is being introduced.
- Introducing a metric without assigning it a role in the argument.
- Making readers infer how a paragraph supports the central claim.

**Source Tags:** `topic_sentence_insertion`, `reader_guidance`, `evidence_chain`

**Primary Level:** Paragraph

**Secondary Level:** Sentence

**Evidence Strength:** Strong

### Principle 8: Use Independent Evidence To Support The Main Signal

**Description:** When a new signal or metric is proposed, pair it with an independent physical reference.

**Why:** The teacher strengthens the argument by linking $T_2$ signatures to tortuosity, permeability, and benchmark validation rather than leaving NMR as a standalone interpretation.

**Before/After Example:**

Before: `We further define a matrix--vug connectivity (MVC) index, showing that earlier coupling in channeling enables the most efficient acid breakthrough.`

After: `We further define a matrix--vug connectivity (MVC) index from $T_2$ spectra and compare it with flow-field tortuosity.`

**Applicable Sections:** Abstract, Methods validation, Results and Discussion.

**Common Failure Modes:**

- Presenting a new metric without saying where it comes from.
- Treating agreement with another quantity as implied rather than explicit.
- Using a metric name before establishing its physical meaning.

**Source Tags:** `evidence_chain`, `metric_grounding`, `supporting_actor_reposition`

**Primary Level:** Paragraph

**Secondary Level:** Section

**Evidence Strength:** Emerging. The principle is important, but the current tag counts for `evidence_chain`, `metric_grounding`, and `supporting_actor_reposition` are still low; collect more cases before making this a standalone skill.

### Principle 9: Let Literature Serve The Current Result

**Description:** Literature comparison should clarify what the present result adds, not simply prove familiarity with the field.

**Why:** In Results and Discussion, the teacher adds literature only where it helps distinguish this paper's contribution: time-resolved, regime-specific NMR pathways.

**Before/After Example:**

Before: `Together, the decomposed peaks show that the three regimes reorganize matrix--vug exchange along flow pathways...`

After: `Previous carbonate dissolution NMR studies qualitatively showed that long $T_2$ components increase as large pores, vugs, or wormholes develop... However, those studies did not establish regime specific, time resolved $T_2$ pathways. Our framework addresses this gap...`

**Applicable Sections:** Introduction Challenge, Results and Discussion.

**Common Failure Modes:**

- Adding literature as a broad paragraph disconnected from the result.
- Repeating literature already introduced in the Introduction.
- Comparing with prior work without naming the new contribution.

**Source Tags:** `supporting_actor_reposition`, `storyline_alignment`, `result_interpretation`

**Primary Level:** Paragraph

**Secondary Level:** Section

**Evidence Strength:** Medium

### Principle 10: Remove Detail That Arrives Before Its Function

**Description:** Technical details should be kept only when they serve the paragraph's current function; otherwise they should be compressed, moved, or commented out.

**Why:** Several edits remove detailed explanations that interrupt the funnel or distract from the result's main mechanism.

**Before/After Example:**

Before: `The emergence of this regime requires a highly heterogeneous initial pore architecture... This advection-dominated environment allows unreacted fluids to penetrate the entire macroscopic system before being completely consumed...`

After: `%The emergence of this regime requires a highly heterogeneous initial pore architecture... before being completely consumed...%`

**Applicable Sections:** Introduction Opening, Methods, Results and Discussion.

**Common Failure Modes:**

- Explaining one regime too deeply before the reader knows the problem.
- Letting technical side-notes break paragraph momentum.
- Keeping correct but low-function details in the main text.

**Source Tags:** `redundancy_removal`, `funnel_narrowing`, `reader_guidance`

**Primary Level:** Paragraph

**Secondary Level:** Section

**Evidence Strength:** Medium

## Sentence-Level Principles

### Principle 11: Prefer Physical Verbs Over Generic Reporting Verbs

**Description:** Use verbs that reveal physical action: reshapes, focuses, exchanges, penetrates, merges, controls, reflects.

**Why:** Physical verbs make the mechanism visible at sentence level and reduce vague prose.

**Before/After Example:**

Before: `Mineral dissolution widely occurs in natural and engineering processes...`

After: `Mineral dissolution reshapes pore networks through spatiotemporally variable pathways...`

**Applicable Sections:** Title, Abstract, Introduction, Results and Discussion.

**Common Failure Modes:**

- Relying on "occurs," "shows," "is used," or "provides" when a mechanism verb is available.
- Naming a phenomenon without showing its action.
- Making physical processes sound static.

**Source Tags:** `physics_first`, `mechanism_emphasis`, `sentence_flow`

**Primary Level:** Sentence

**Secondary Level:** Paragraph

**Evidence Strength:** Strong

### Principle 12: Calibrate Claims To The Evidence

**Description:** Strong claims should be bounded by the type of evidence, model scope, and representative cases.

**Why:** Teacher edits sometimes make the claim more useful by making it more precise: representative regimes, potential proxy, diagnostic indicators, and comparison with independent variables.

**Before/After Example:**

Before: `This Pe range is consistent with previous pore-scale dissolution studies. These regimes provide the structural basis for interpreting the following NMR $T_2$ signatures...`

After: `This Pe range is consistent with previous pore-scale dissolution studies..., and the selected regimes serve as representative regime examples rather than a complete regime-boundary analysis.`

**Applicable Sections:** Abstract, Introduction Action, Results and Discussion.

**Common Failure Modes:**

- Treating representative simulations as a complete regime map.
- Claiming a diagnostic framework without naming its validation boundary.
- Letting a useful result sound broader than the evidence supports.

**Source Tags:** `overclaim_softening`, `reader_guidance`, `storyline_alignment`

**Primary Level:** Sentence

**Secondary Level:** Macro

**Evidence Strength:** Emerging. Keep this principle because it is important for GRL writing, but current direct evidence is limited; add more cases from future drafts and reviews.

## Layer Map

### Workflow-Level

- Meta Principle 0: Diagnose The Manuscript Stage Before Editing

### Macro-Level

- Principle 1: Make The Title Carry The Main Scientific Action
- Principle 2: Keep One Storyline Across OCAR

### Section-Level

- Principle 3: Open With A Process, Not A List
- Principle 4: Define The Challenge As A Process-Based Link
- Principle 5: Make Methods Answer "Why This Workflow Can Prove The Claim"
- Principle 6: Results Must Translate Patterns Into Mechanisms

### Paragraph-Level

- Principle 7: Start Paragraphs With Their Function
- Principle 8: Use Independent Evidence To Support The Main Signal
- Principle 9: Let Literature Serve The Current Result
- Principle 10: Remove Detail That Arrives Before Its Function

### Sentence-Level

- Principle 11: Prefer Physical Verbs Over Generic Reporting Verbs
- Principle 12: Calibrate Claims To The Evidence

## How To Use This Library In The Next Phase

In Phase 3, these principles can be converted into separate skills, but this mapping should remain a draft until more cases are collected. The first skill should likely be a workflow router based on Meta Principle 0.

| Future Skill | Principles To Include |
|---|---|
| `workflow_router.md` | Meta Principle 0 |
| `story_architect.md` | Principles 1, 2 |
| `ocar_funnel.md` | Principles 3, 4 |
| `methods_evidence_chain.md` | Principles 5, 8 |
| `mechanism_results.md` | Principles 6, 7, 9 |
| `paragraph_engineering.md` | Principles 7, 10 |
| `sentence_hierarchy.md` | Principles 11, 12 |

Do not lock this skill architecture yet. In particular, Principle 8 and Principle 12 should remain "emerging" until the database contains more examples.
