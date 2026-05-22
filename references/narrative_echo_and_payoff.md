# Narrative Echo and Payoff

## Purpose

This module checks whether the manuscript builds clear promise-payoff relationships across the paper and within Results and Discussion.

It ensures that:

1. Introduction prepares the questions, concepts, and method rationale that Results/Discussion later resolve.
2. Results subsections form a continuous mechanism chain through forward pointers, backward links, delayed payoffs, and thread summaries.

## Part A: Paper-Level Echo

Check whether the Introduction's promises are paid off later.

Core questions:

- What problem does the Introduction promise to solve?
- What gap does it define?
- What concept, metric, or method rationale does it prepare?
- Does Results/Discussion answer these promises?
- Are there Introduction details that never return later?
- Are there major Results findings that appear without prior motivation?
- Does the Discussion return to the original gap and broaden the implication without drifting away from the evidence?

## Part B: Results-Level Echo

Check whether Results and Discussion subsections are connected as a mechanism chain.

### Core Echo Types

#### 1. Forward Pointer

A sentence near the end of a subsection that prepares the reader for the next analytical step.

Purpose: tell the reader why the next section is needed.

Example pattern:

```text
These regime-specific spectral pathways motivate an independent hydraulic test of whether NMR-inferred coupling corresponds to flow-path optimization.
```

#### 2. Backward Link

A sentence at the beginning of a subsection that explicitly inherits the previous finding.

Purpose: prevent each subsection from reading as an isolated result block.

Example pattern:

```text
Building on the regime-specific T2 pathways identified above, we next examine whether these spectral differences correspond to hydraulic reorganization.
```

#### 3. Delayed Payoff

A result or concept introduced briefly earlier and explained or quantified later.

Purpose: maintain reader curiosity and show that later metrics are logically necessary.

Example pattern:

```text
This early spectral merging is quantified below using the MVC metric.
```

#### 4. Thread Summary

A short synthesis sentence that summarizes several preceding findings and turns them into the next mechanistic step.

Purpose: help readers see the continuous storyline.

Example pattern:

```text
Together, the T2 spectra and tortuosity trends show that the regimes differ not only in geometry, but also in the timing of matrix-vug coupling and flow-path optimization.
```

## Rules Derived from Cases

### Rule 1: New metrics need prior motivation

If a metric appears for the first time in Results, the Introduction or the preceding Results subsection should already explain why existing observations are insufficient and why the new metric is needed.

### Rule 2: Each Results subsection should inherit or prepare

A Results subsection should either inherit a question from the previous subsection or prepare the next analytical step. If it does neither, it will read as an isolated result block.

### Rule 3: Validate signal interpretation with an independent metric

When a subsection interprets a signal or pattern, the next subsection should test whether that interpretation corresponds to an independent physical, hydraulic, structural, or mechanistic measure.

### Rule 4: Use delayed payoff when a partial explanation leaves a residual question

If one metric explains part of a contrast but cannot explain the whole outcome, explicitly state the remaining question before introducing the next metric or mechanism.

### Rule 5: Use thread summaries after multiple result blocks

After several related results, insert a short synthesis that converts them into one mechanism chain. The summary should name the main process, not only repeat figure observations.

### Rule 6: Do not leave Introduction promises unpaid

Any concept introduced as central in the Introduction must return in Results, Discussion, Implications, or Conclusions. If it does not return, remove it, downgrade it, or add a real payoff.

## Diagnostic Checklist

- Does each major Introduction promise receive a later payoff?
- Does every major Results concept have enough prior motivation?
- Does each Results subsection inherit something from the previous one?
- Does each subsection prepare the next step when needed?
- Are important later results briefly foreshadowed earlier?
- Are earlier observations later quantified, tested, or mechanistically explained?
- Are there isolated result blocks with no forward or backward connection?
- Does the final subsection synthesize earlier findings into the central mechanism?

## Common Problems

1. Results subsections are arranged side by side, not as a mechanism chain.
2. A new metric appears suddenly without earlier motivation.
3. A subsection ends with data, but not with a forward-looking interpretation.
4. A later subsection does not explicitly return to earlier observations.
5. The Discussion claims broad significance without returning to the Introduction gap.

## Failure Symptoms by Echo Type

### Missing Forward Pointer

Symptom: A subsection ends with a value, figure description, or local observation, and the next subsection starts a new metric or topic without motivation.

Minimal fix: Add one sentence explaining why the next analytical step is needed.

### Missing Backward Link

Symptom: A subsection begins with a new topic, metric, or figure but does not inherit the previous subsection's unresolved question or mechanism claim.

Minimal fix: Start the subsection by naming the previous finding and stating what will now be tested, quantified, or explained.

### Missing Delayed Payoff

Symptom: A metric appears only when it is defined, with no earlier signal that such a metric is needed.

Minimal fix: Add a setup sentence in the Introduction or preceding Results subsection that identifies the remaining distinction the metric will resolve.

### Missing Thread Summary

Symptom: Several Results subsections are individually correct, but the reader must infer the mechanism chain alone.

Minimal fix: Add a 1-2 sentence synthesis that names the shared mechanism and links the main evidence types.

### Orphan Introduction Promise

Symptom: The Introduction emphasizes a central concept, method rationale, or application payoff that never returns in Results, Discussion, Implications, or Conclusions.

Minimal fix: Remove or downgrade the orphan content, or add a real payoff where the later evidence answers it.

## Recommended Actions

- Add one forward pointer at the end of a subsection.
- Add one backward link at the beginning of the next subsection.
- Add one thread-summary sentence before introducing a new metric.
- Delete or downgrade Introduction content that is never used later.
- Add a brief foreshadowing phrase in Introduction or the preceding Results subsection if a major Results concept appears suddenly.

## Boundary Rule

Do not treat narrative echo as decorative transition polishing. It is a structure-level test of whether the paper sets up, delays, pays off, and summarizes the scientific story.
