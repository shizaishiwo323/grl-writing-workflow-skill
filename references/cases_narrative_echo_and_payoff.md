# Cases: Narrative Echo and Payoff

Purpose: store real writing-function cases that teach AI how a manuscript sets up, delays, pays off, and summarizes its scientific story.

Use this file for section-to-section continuity, Introduction-Results alignment, Results subsection transitions, delayed metric introduction, and final thread summaries.

Self manuscript cases are used for project-specific transfer, especially the current NMR-dissolution storyline. Reference paper cases are used for cross-paper generalization, especially metric-building, regime-comparison, and method-extension papers.

## Case Index

### Self Manuscript Cases

- NEP-SELF-001: Introduction promise paid off by MVC.
- NEP-SELF-002: Results opening prepares the NMR T2 section.
- NEP-SELF-003: T2 pathways motivate tortuosity validation.
- NEP-SELF-004: Tortuosity validation prepares breakthrough and MVC.
- NEP-SELF-005: MVC closes the mechanism thread.

### Reference Paper Cases

- NEP-REF-2018-001: Archie's exponent moves from empirical gap to pore-throat payoff.
- NEP-REF-2024-001: Flow focusing profile pays off the visual-classification gap.
- NEP-REF-2024-002: Profile evolution separates channeling from wormholing.
- NEP-REF-2025-001: Dissolution-regime contrast pays off through BTC mechanisms.
- NEP-REF-2026-001: Unsaturated NMR signals pay off through tortuosity and connectivity.

## Extraction Template

```markdown
## Case ID: Short Title

### Source
Paper title / journal / year / section position

### Evidence Location
Introduction paragraph or Results/Discussion section where the echo is visible.

### Echo Level
Paper-level echo / Results-level echo / Paragraph-level echo

### Echo Type
Introduction promise-payoff / Forward pointer / Backward link / Delayed payoff / Thread summary

### Tags
tag_1; tag_2

### Detection Signal
When the draft shows...

### Before Context
What problem, observation, gap, or setup appears earlier?

### Echo Sentence or Move
The key sentence, paragraph move, or paraphrased writing action.

### Payoff
Where is it paid off later, and what does the payoff accomplish?

### Why It Works
Why this echo improves continuity and mechanism clarity.

### Transferable Rule
How to reuse the move in future manuscripts.

### AI Instruction
What AI should do when it sees a similar draft.
```

## Case NEP-SELF-001: Introduction Promise Paid Off by MVC

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Introduction to Section 3.3.

### Evidence Location
Introduction final two paragraphs; Section 3.3 opening and MVC interpretation; Implications first paragraph.

### Echo Level
Paper-level echo.

### Echo Type
Introduction promise-payoff.

### Tags
intro_promise_payoff; delayed_payoff

### Detection Signal
A manuscript promises to interpret connectivity, coupling, or breakthrough from a signal, but the quantitative metric appears only later in Results.

### Before Context
The Introduction argues that existing NMR interpretations mainly describe apparent pore size or porosity. It then states that this is insufficient for distinguishing dynamic dissolution regimes that have similar porosity increases but different spatial pathways and breakthrough mechanisms.

### Echo Sentence or Move
The Introduction does not merely announce NMR simulation. It prepares a specific need: time-varying T2 signals must be interpreted as quantitative indicators of dissolution regimes, connectivity, and permeability breakthrough.

### Payoff
Section 3.3 introduces MVC from the T2 signal and uses it to explain why channeling reaches breakthrough earlier than wormholing. MVC is therefore not a late add-on metric; it answers the connectivity gap prepared in the Introduction.

### Why It Works
The reader already knows why a connectivity metric is needed before the equation appears. The later MVC analysis feels like the natural resolution of the paper's main interpretive problem.

### Transferable Rule
If Results introduce a new metric, the Introduction or previous Results subsection must first show why existing observations are insufficient.

### AI Instruction
When a draft introduces a metric late in Results, scan the Introduction for prior motivation. If missing, add a setup sentence explaining the unresolved distinction that the metric will quantify.

## Case NEP-SELF-002: Results Opening Prepares the NMR T2 Section

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Results opening to Section 3.1.

### Evidence Location
Results opening paragraph immediately before Section 3.1; Section 3.1 first paragraph.

### Echo Level
Results-level echo.

### Echo Type
Forward pointer and backward link.

### Tags
forward_pointer; backward_link

### Detection Signal
Results begins with selected regimes, cases, or parameters, and the first subsection needs to inherit that comparison logic rather than start with figure description.

### Before Context
The Results opening selects three representative dissolution regimes: face dissolution, channeling, and wormholing. It also states that their contrasting acid-transport organization forms the structural basis for interpreting the NMR T2 signatures discussed next.

### Echo Sentence or Move
The opening paragraph first defines the comparison set, then points forward from structural organization to NMR signal interpretation.

### Payoff
Section 3.1 begins by showing that each regime follows a distinct T2 relaxation pathway. The T2 section inherits the structural contrast rather than starting as a figure description.

### Why It Works
The first Results subsection is framed as the first payoff of the regime selection. This prevents the paper from sounding like "three cases are shown" and instead makes the cases serve a signal-mechanism question.

### Transferable Rule
A Results opening should identify the comparison logic and explicitly prepare the first analytical section.

### AI Instruction
Before revising Results Section 1, check whether the paragraph immediately before it states why this section comes first and what earlier setup it pays off.

## Case NEP-SELF-003: T2 Pathways Motivate Tortuosity Validation

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Section 3.1 ending to Section 3.2 opening.

### Evidence Location
Section 3.1 final synthesis paragraphs; Section 3.2 opening paragraph.

### Echo Level
Results-level echo.

### Echo Type
Thread summary and backward link.

### Tags
thread_summary; backward_link

### Detection Signal
One subsection interprets a signal or pattern, and the next subsection introduces an independent metric that should test the interpretation.

### Before Context
Section 3.1 shows that face dissolution, channeling, and wormholing produce distinct T2 pathways: persistent peak separation, transient bimodality followed by merging, or broad peak overlap.

### Echo Sentence or Move
The section ending summarizes the three T2 pathways as signatures of evolving pore coupling, not merely as pore-size changes.

### Payoff
Section 3.2 then uses tortuosity as an independent hydraulic reference to test whether the T2-derived spectral evolution reflects flow-path optimization.

### Why It Works
The paper moves from signal interpretation to hydraulic validation. The reader is not asked to accept T2 morphology alone as mechanism evidence; the next section checks it against another metric.

### Transferable Rule
When one Results subsection interprets a signal, the next subsection can gain force by validating that interpretation with an independent physical metric.

### AI Instruction
If a subsection makes a signal-based claim, ask what independent result later tests it. Add a backward-link sentence at the next subsection opening.

## Case NEP-SELF-004: Tortuosity Validation Prepares Breakthrough and MVC

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Section 3.2 to Section 3.3.

### Evidence Location
Section 3.2 final comparison of channeling and wormholing; Section 3.3 opening two paragraphs.

### Echo Level
Results-level echo.

### Echo Type
Delayed payoff and forward mechanism transition.

### Tags
delayed_payoff; forward_pointer

### Detection Signal
A previous subsection validates part of the mechanism, but the next subsection introduces a new metric without explicitly stating what remains unresolved.

### Before Context
Section 3.2 shows that channeling and wormholing can reach similar tortuosity values near comparable porosity, but differ in breakthrough timing. This creates a remaining mechanism question: if tortuosity is similar, what explains the efficiency hierarchy?

### Echo Sentence or Move
The tortuosity section validates flow-path optimization but does not close the mechanism. It leaves room for the next section to connect hydraulic reorganization to matrix-vug coupling and breakthrough.

### Payoff
Section 3.3 shifts from the porosity-permeability hierarchy to the underlying coupling process, then defines MVC to quantify how newly formed conduits couple with the matrix.

### Why It Works
The new metric is introduced only after a clear explanatory need appears. Tortuosity supports the story, but MVC resolves the remaining distinction between channeling and wormholing.

### Transferable Rule
When a validation metric explains part of the mechanism but leaves a contrast unresolved, the following section should state that residual question before introducing a new metric.

### AI Instruction
Look for "similar metric, different outcome" moments. These are natural places to introduce a delayed payoff metric or mechanism explanation.

## Case NEP-SELF-005: MVC Closes the Mechanism Thread

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Section 3.3 ending.

### Evidence Location
Section 3.3 final paragraph; Implications opening paragraph; Conclusions second paragraph.

### Echo Level
Results-level echo.

### Echo Type
Thread summary.

### Tags
thread_summary; intro_promise_payoff

### Detection Signal
Several subsections provide correct individual results, but the final Results subsection must convert them into one causal mechanism.

### Before Context
Earlier sections establish regime-specific T2 pathways, tortuosity evolution, and permeability breakthrough timing. Each result answers part of the story, but the mechanism needs one final synthesis.

### Echo Sentence or Move
The Section 3.3 ending combines MVC timing, channeling, wormholing, coupling sequence, and breakthrough timing into one mechanism: early establishment and synchronous enlargement of a dominant channel control breakthrough efficiency.

### Payoff
This closes both the Results chain and the Introduction promise. NMR signatures are shown to diagnose dissolution dynamics because they track matrix-vug coupling and hydraulic breakthrough efficiency.

### Why It Works
The ending does not repeat a figure result. It converts several metrics into a single causal explanation and prepares the broader Implications section.

### Transferable Rule
The last mechanism subsection should synthesize prior signal, hydraulic, and metric evidence into one causal statement.

### AI Instruction
At the end of Results, require a thread summary that names the main mechanism and explicitly links the major evidence types used earlier.

## Case NEP-REF-2018-001: Archie's Exponent Moves From Empirical Gap to Pore-Throat Payoff

### Source
Physical Explanation of Archie's Porosity Exponent in Granular Materials: A Process-Based, Pore-Scale Numerical Study / Geophysical Research Letters / 2018 / Introduction, Results 3.3, Discussion.

### Evidence Location
Introduction final paragraph; Results Section 3.3; Discussion first two paragraphs; Conclusions.

### Echo Level
Paper-level echo.

### Echo Type
Introduction promise-payoff.

### Tags
intro_promise_payoff; delayed_payoff

### Detection Signal
The Introduction frames an empirical parameter as physically unresolved, and Results must avoid jumping directly to a correlation without mechanism.

### Before Context
The Introduction starts from the practical use of Archie's law and narrows to an unresolved issue: the porosity exponent m varies across materials, but its dominant textural control remains unclear.

### Echo Sentence or Move
The study promises a pore-scale explanation by combining controlled granular compaction, conductivity calculation, and pore-attribute analysis.

### Payoff
Results 3.3 explains the increase in m through intensifying nonuniformity of the local electrical field. The Discussion then links normalized m to pore-throat volume fraction, turning the earlier "physical meaning of m" gap into a pore-throat mechanism.

### Why It Works
The paper does not jump from empirical correlation to final predictor. It first shows the field-distribution mechanism, then uses pore-throat volume as the compact payoff.

### Transferable Rule
For an empirical-parameter paper, prepare the unresolved meaning of the parameter in the Introduction and pay it off by revealing a physical process before proposing a correlation.

### AI Instruction
If a manuscript explains an empirical coefficient, check whether Results first show the mechanism that makes the coefficient change, before presenting the final predictor.

## Case NEP-REF-2024-001: Flow Focusing Profile Pays Off the Visual-Classification Gap

### Source
Quantifying Dissolution Dynamics in Porous Media Using a Spatial Flow Focusing Profile / Geophysical Research Letters / 2024 / Introduction, Results and Discussion, Conclusions.

### Evidence Location
Introduction final paragraph; Results and Discussion Sections 4.1-4.3; Conclusions first two paragraphs.

### Echo Level
Paper-level echo.

### Echo Type
Introduction promise-payoff.

### Tags
intro_promise_payoff; delayed_payoff

### Detection Signal
The paper proposes a new metric, but the draft must first show a specific classification or interpretation failure that makes the metric necessary.

### Before Context
The Introduction states that dissolution-regime identification often relies on visual comparison of final structures. This becomes unreliable when wormholing, channeling, and uniform dissolution have subtle or similar-looking morphologies.

### Echo Sentence or Move
The paper argues that a useful metric cannot be a single whole-system number because dissolution creates spatial heterogeneity. It therefore motivates a slice-by-slice flow focusing profile.

### Payoff
Results and Discussion show that the profile behavior distinguishes uniform dissolution, wormholing, and channeling, and the Conclusions return to the central claim that spatial and temporal profile information outperforms visual comparison alone.

### Why It Works
The new metric is necessary because the paper first defines a specific failure of older classification. The payoff resolves that exact failure.

### Transferable Rule
A metric-building paper should begin with the decision that current methods cannot make, then show that the new metric makes that decision visible.

### AI Instruction
When a draft proposes a metric, ask: "What failure does this metric solve?" If the failure is not explicit, strengthen the Challenge before polishing the metric description.

## Case NEP-REF-2024-002: Profile Evolution Separates Channeling From Wormholing

### Source
Quantifying Dissolution Dynamics in Porous Media Using a Spatial Flow Focusing Profile / Geophysical Research Letters / 2024 / Sections 4.1 to 4.3.

### Evidence Location
Results and Discussion Section 4.1 representative regimes; Section 4.2 phase diagram; Section 4.3 heterogeneity comparison.

### Echo Level
Results-level echo.

### Echo Type
Delayed payoff and thread summary.

### Tags
delayed_payoff; thread_summary

### Detection Signal
Final morphologies look similar or ambiguous, so the draft needs to preserve and pay off the evolution history across subsections.

### Before Context
Section 4.1 first contrasts representative cases: wormholing advances from the inlet, while channeling widens preexisting paths along the system. This establishes the process distinction.

### Echo Sentence or Move
The paper repeatedly returns to how the profile changes over time, not only what the final pattern looks like. The distinction is delayed until profile history becomes the evidence.

### Payoff
Section 4.3 shows that similar final structures can have different profile histories and therefore different regimes. The profile captures evolution history that visual comparison can miss.

### Why It Works
The Results subsections do not sit side by side. Representative examples prepare the phase diagram, and the heterogeneity analysis pays off the claim that history matters.

### Transferable Rule
When final morphologies are ambiguous, build a Results echo from representative evolution to parameter sweep to history-based summary.

### AI Instruction
If a draft compares regimes, check whether later subsections return to the same distinguishing feature rather than switching to unrelated metrics.

## Case NEP-REF-2025-001: Dissolution-Regime Contrast Pays Off Through BTC Mechanisms

### Source
Anomalous Transport in Dissolving Porous Media: Transitions Between Fickian and Non-Fickian Regimes / Geophysical Research Letters / 2025 / Introduction, Sections 3.1 to 3.3, Conclusions.

### Evidence Location
Introduction final paragraph; Results and Discussions Sections 3.1-3.3; Conclusions first two paragraphs.

### Echo Level
Paper-level and Results-level echo.

### Echo Type
Introduction promise-payoff and backward link.

### Tags
intro_promise_payoff; backward_link

### Detection Signal
A Results section compares two opposing regimes and needs to move from contrast, to mechanism, to generalized phase behavior.

### Before Context
The Introduction argues that studies of anomalous transport usually treat structural heterogeneity as fixed, while dissolution changes pore structure. It then promises to test how initial heterogeneity and dissolution regime shape transport behavior.

### Echo Sentence or Move
Section 3.1 starts with two contrasting scenarios: wormholing from an initially homogeneous network and uniform dissolution from an initially heterogeneous network.

### Payoff
Section 3.2 explains why the transport transitions occur: wormholing creates preferential channels and stagnant zones, while uniform dissolution homogenizes the flow field. Section 3.3 generalizes the contrast into a phase diagram.

### Why It Works
The paper uses the first Results section to show the headline pattern, the second to explain mechanism, and the third to generalize. Each subsection inherits the previous one.

### Transferable Rule
For a contrast paper, show the two opposing outcomes first, then use the next subsection to explain the shared mediator that makes them diverge.

### AI Instruction
When revising Results, check whether a regime comparison has three linked steps: contrast, mechanism, and generalization.

## Case NEP-REF-2026-001: Unsaturated NMR Signals Pay Off Through Tortuosity and Connectivity

### Source
How Does Fluid Exchange Between Pores in Unsaturated Porous Media? / Geophysical Research Letters / 2026 / Introduction, Sections 3.1 to 3.4, Geophysical Implications.

### Evidence Location
Introduction final paragraph; Results and Discussions opening; Sections 3.1-3.4; Geophysical Implications opening.

### Echo Level
Paper-level and Results-level echo.

### Echo Type
Introduction promise-payoff and delayed payoff.

### Tags
intro_promise_payoff; delayed_payoff

### Detection Signal
A familiar method is extended to a harder physical condition, and Results must separate observable signal, validation, and structural determinant.

### Before Context
The Introduction states that NMR can track pore coupling in saturated media, but unsaturated conditions complicate interpretation because water-pathway geometry and connectivity change with saturation.

### Echo Sentence or Move
The Results opening previews the full payoff: T2 distributions and T2-store-T2 maps reveal weakening pore coupling as saturation decreases, corresponding to more tortuous and eventually disconnected water pathways.

### Payoff
Sections 3.1 and 3.2 establish the NMR signal evolution, Section 3.3 validates simulation against measurement, and Section 3.4 explains the weakening through water-pathway tortuosity and connectivity ratio. The Implications section returns to interpreting field NMR under saturation gradients.

### Why It Works
The paper delays the physical cause until after signal evidence and validation. This order protects readability: signal first, credibility second, mechanism third.

### Transferable Rule
For method-extension papers, pay off the Introduction gap by moving from observable signal, to validation, to the structural mechanism that explains the signal.

### AI Instruction
If a manuscript applies a known method to a harder condition, ensure that Results distinguish method response, validation, and physical determinant instead of mixing all three in one block.
