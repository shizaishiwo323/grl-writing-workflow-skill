# Cases: Mechanism-Centered Results Writer

Purpose: store real writing-function cases that teach AI how Results and Discussion paragraphs convert observations, figures, metrics, and regime comparisons into physical mechanism chains.

Use this file when revising Results paragraphs that describe figures, spectra, breakthrough curves, regimes, or secondary metrics without clearly explaining the mechanism.

Self manuscript cases are used for project-specific transfer, especially the current NMR-dissolution storyline. Reference paper cases are used for cross-paper generalization, especially metric-building, regime-comparison, and structure-to-signal writing.

## Case Index

### Self Manuscript Cases

- MCR-SELF-001: Results opening establishes the mechanism task.
- MCR-SELF-002: Face dissolution converts structure into T2 peak separation.
- MCR-SELF-003: Channeling links transient bimodality to early breakthrough.
- MCR-SELF-004: Tortuosity validates T2-derived flow-path interpretation.
- MCR-SELF-005: MVC turns a macroscopic hierarchy into a coupling mechanism.

### Reference Paper Cases

- MCR-REF-2018-001: Particle shape is tested against dilute-state theory.
- MCR-REF-2018-002: Particle-size effects are explained by sample state.
- MCR-REF-2018-003: Archie's exponent is linked to pore-throat electric-field focusing.
- MCR-REF-2024-001: Flow focusing profile turns visual regimes into a mechanism metric.
- MCR-REF-2024-002: Temporal profile evolution separates channeling from wormholing.
- MCR-REF-2025-001: Wormholing BTC features are mapped to transport zones.
- MCR-REF-2025-002: Uniform dissolution explains non-Fickian to Fickian transition.
- MCR-REF-2025-003: A phase diagram synthesizes heterogeneity and Damkohler controls.
- MCR-REF-2026-001: T2 peak separation is interpreted as weakened pore coupling.
- MCR-REF-2026-002: Off-diagonal exchange and geometry metrics explain coupling loss.

## How to Choose a Case

- If the draft only reports a figure trend, use observation-to-mechanism cases.
- If the draft links geometry to NMR, SIP, CT, BTC, or permeability signals, use structure-to-signal cases.
- If the draft introduces tortuosity, MVC, flow focusing, or another index, use metric-validation cases.
- If the draft compares regimes, use regime-comparison cases.
- If the draft explains breakthrough, transition, plateau, or tailing, use breakthrough-mechanism cases.
- If the draft summarizes several results or a phase diagram, use mini-synthesis cases.

## Extraction Template

```markdown
## Case ID: Short Title

### Source
Paper title / journal / year / section position

### Mechanism-Writing Type
Observation-to-mechanism / Structure-to-signal / Metric validation / Regime comparison / Breakthrough mechanism / Mini synthesis

### Tags
tag_1; tag_2; tag_3

### Context
What question or comparison is being handled before the result appears?

### Typical Failure Pattern
What weak draft pattern this case helps fix.

### Result Observation
What pattern, figure feature, signal change, or metric behavior is observed?

### Mechanism Move
How does the author convert the observation into physics, geometry, transport, signal response, or causal process?

### Evidence Role
What role does the figure, metric, or comparison play in the mechanism chain?

### Why It Works
Why this paragraph is more than figure description or data listing.

### Transferable Rule
One reusable rule for future Results writing.

### AI Instruction
What AI should do when it sees a similar Results problem.
```

## Case MCR-SELF-001: Results Opening Establishes the Mechanism Task

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Results and Discussion opening.

### Mechanism-Writing Type
Mini synthesis; Regime comparison.

### Tags
mechanism_before_data; regime_comparison; evidence_hierarchy

### Context
The Results must introduce three representative dissolution regimes without making the section sound like a parameter survey.

### Typical Failure Pattern
The Results opening lists cases, parameters, or figures before explaining what mechanism question those cases are meant to answer.

### Result Observation
The opening identifies face dissolution, channeling, and wormholing as representative cases and shows their different acid-transport organizations at comparable porosity.

### Mechanism Move
The paragraph states that the spatial organization of acid transport forms the structural basis for interpreting the later NMR T2 signatures and breakthrough efficiency.

### Evidence Role
The concentration maps are not the main conclusion. They define the physical comparison set that later signal and hydraulic evidence must explain.

### Why It Works
The reader receives the mechanism task before the spectra appear: the paper is asking how different dissolution pathways generate different NMR and breakthrough responses.

### Transferable Rule
Open a Results section by naming the mechanism question that the first figures will answer, not by merely listing the figures or parameter cases.

### AI Instruction
When Results begins with several representative cases, require one sentence that explains why those cases are mechanistically diagnostic for the next subsection.

## Case MCR-SELF-002: Face Dissolution Converts Structure Into T2 Peak Separation

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Section 3.1 face dissolution paragraphs.

### Mechanism-Writing Type
Structure-to-signal; Observation-to-mechanism.

### Tags
structure_to_signal; causal_chain; avoid_figure_description

### Context
The manuscript must explain why face dissolution produces a distinct T2 pathway instead of only reporting a bimodal spectrum.

### Typical Failure Pattern
The paragraph reports matrix and vug peaks as separate curve features but does not explain what physical decoupling creates the spectral separation.

### Result Observation
Dissolution localizes near the inlet, creating large vugs behind the reaction front and leaving a dense matrix ahead. The T2 spectrum evolves from one peak to separated matrix and vug peaks, then returns to a long-T2-dominated peak.

### Mechanism Move
The text connects spatial separation between vugs and residual matrix to weakened pore coupling and restricted magnetization exchange, which produces persistent peak separation and delayed hydraulic connection.

### Evidence Role
The T2 components and peak fractions serve as signal evidence for matrix preservation, vug growth, and weak coupling across the reaction front.

### Why It Works
The paragraph does not stop at "Peak 1 decreases and Peak 2 increases." It explains why the spectral morphology arises from the face-dissolution geometry.

### Transferable Rule
When a signal splits into components, identify the physical domains that became decoupled and explain why exchange between them changed.

### AI Instruction
If a draft reports peak separation without mechanism, add the chain: geometry contrast -> exchange or coupling change -> signal morphology -> transport implication.

## Case MCR-SELF-003: Channeling Links Transient Bimodality to Early Breakthrough

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Section 3.1 channeling paragraph.

### Mechanism-Writing Type
Breakthrough mechanism; Structure-to-signal; Regime comparison.

### Tags
breakthrough_mechanism; transition_explanation; causal_chain

### Context
Channeling must be distinguished from both face dissolution and wormholing using a transient signal pathway and a permeability outcome.

### Typical Failure Pattern
The sentence jumps from transient bimodality directly to early breakthrough without naming peak merging, conduit formation, or strengthened pore coupling.

### Result Observation
A principal channel rapidly penetrates the domain, the T2 spectrum briefly becomes bimodal, and the spectrum then shifts toward a merged long-relaxation component near breakthrough.

### Mechanism Move
The paragraph explains that channel enlargement along much of its length reorganizes the flow field, strengthens diffusive exchange between matrix pores and the conduit, promotes pore coupling, and allows early permeability breakthrough with limited matrix dissolution.

### Evidence Role
The transient T2 bimodality is treated as a stage marker. The rapid peak merging and breakthrough porosity are used to show that coupling and conduit formation become efficient quickly.

### Why It Works
The writing converts a time sequence into a mechanism sequence: penetration -> flow focusing -> temporary separation -> stronger exchange -> merged signal -> breakthrough.

### Transferable Rule
For transient signal behavior, explain what structural transition each signal stage represents and how the transition changes the final hydraulic outcome.

### AI Instruction
When a draft says a feature is "transient," force it to answer: transient between which two physical states, and why does that transition matter?

## Case MCR-SELF-004: Tortuosity Validates T2-Derived Flow-Path Interpretation

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Section 3.2 tortuosity paragraphs.

### Mechanism-Writing Type
Metric validation; Regime comparison.

### Tags
metric_validation; secondary_metric_positioning; evidence_hierarchy

### Context
After Section 3.1 interprets T2 pathways as pore coupling and flow-path reorganization, the manuscript needs an independent hydraulic check.

### Typical Failure Pattern
A secondary metric is introduced as a separate result block rather than as validation of an earlier T2 interpretation.

### Result Observation
Tortuosity decreases with increasing porosity, but the timing and path of the decrease differ among regimes. Face dissolution reduces tortuosity late, whereas channeling and wormholing show earlier tortuosity reduction with different breakthrough timing.

### Mechanism Move
The text positions tortuosity as hydraulic validation: lower tortuosity indicates straighter, better-connected pathways, supporting the interpretation that T2 peak merging reflects flow-path optimization.

### Evidence Role
Tortuosity is a secondary metric. It tests whether the T2-derived interpretation is hydraulically meaningful rather than replacing the NMR mechanism as the protagonist.

### Why It Works
The metric enters only after the signal interpretation has created a testable mechanism claim. It strengthens the story without opening a separate tortuosity story.

### Transferable Rule
Introduce a secondary metric as validation for a specific previous interpretation, not as a new independent result block.

### AI Instruction
When a Results subsection introduces another metric, require a backward link that states which earlier mechanism claim the metric validates or constrains.

## Case MCR-SELF-005: MVC Turns a Macroscopic Hierarchy Into a Coupling Mechanism

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Section 3.3 breakthrough and MVC paragraphs.

### Mechanism-Writing Type
Metric validation; Breakthrough mechanism; Mini synthesis.

### Tags
metric_validation; breakthrough_mechanism; mini_synthesis

### Context
The porosity-permeability relation establishes that channeling breaks through earlier than wormholing and face dissolution, but this hierarchy still needs a pore-coupling explanation.

### Typical Failure Pattern
A new index appears after the permeability hierarchy without first explaining what unresolved mechanism distinction the index will quantify.

### Result Observation
Channeling reaches the permeability threshold at lower porosity than wormholing, and the MVC peak occurs earlier for channeling than for wormholing. Face dissolution shows weak and eventually disappearing matrix-vug connectivity.

### Mechanism Move
MVC is introduced from the T2 signal to quantify matrix-vug coupling. Its timing explains why a single coherently enlarging conduit in channeling produces faster breakthrough than competing and later-coalescing wormholes.

### Evidence Role
The porosity-permeability curve gives the macroscopic hierarchy; MVC explains the microscopic coupling sequence behind that hierarchy.

### Why It Works
The new metric grows out of an unresolved mechanism question and closes the Results chain by linking signal, coupling, and permeability breakthrough.

### Transferable Rule
A new Results metric should appear only after the manuscript has made clear what mechanism distinction existing plots cannot resolve.

### AI Instruction
If a draft introduces a new index, ask what prior comparison it explains. Add the missing bridge from macroscopic pattern to microscopic mechanism.

## Case MCR-REF-2018-001: Particle Shape Is Tested Against Dilute-State Theory

### Source
Physical Explanation of Archie's Porosity Exponent in Granular Materials / Geophysical Research Letters / 2018 / Section 3.1.

### Mechanism-Writing Type
Metric validation; Observation-to-mechanism.

### Tags
metric_validation; mechanism_before_data; evidence_hierarchy

### Context
The paper needs to explain why Archie's exponent varies among granular materials instead of treating it as an empirical fitting constant.

### Result Observation
At dilute states, simulated porosity exponents follow the same trend predicted by differential effective medium theory as particle shape changes.

### Mechanism Move
The authors use theory to interpret the trend: particle asphericity controls the dilute-state baseline exponent, while small simulation-theory discrepancies are attributed to voxel representation rather than to a new geologic mechanism.

### Evidence Role
The comparison to analytical theory validates the physical origin of the metric at dilute states and defines a baseline for later dense-state behavior.

### Why It Works
The result is not simply "shape affects m." It identifies the range where a known mechanism applies and prevents later dense-state effects from being conflated with particle shape.

### Transferable Rule
When a metric has multiple possible controls, first isolate the condition where a known theory explains it, then use that baseline to interpret later deviations.

### AI Instruction
If a Results paragraph reports a metric trend, ask whether there is a baseline theory or limiting case that should anchor the interpretation.

## Case MCR-REF-2018-002: Particle-Size Effects Are Explained by Sample State

### Source
Physical Explanation of Archie's Porosity Exponent in Granular Materials / Geophysical Research Letters / 2018 / Section 3.2.

### Mechanism-Writing Type
Regime comparison; Observation-to-mechanism.

### Tags
regime_comparison; transition_explanation; evidence_hierarchy

### Context
Previous theory and experiments disagree about whether particle size range affects Archie's exponent.

### Result Observation
Multisized and monosized samples with the same particle shape behave similarly at dilute states, but diverge as porosity decreases and the samples become nondilute.

### Mechanism Move
The authors resolve the apparent contradiction by separating sample states: effective medium theory applies to dilute samples, whereas experimental particle-size effects arise in packed, nondilute media.

### Evidence Role
The simulations act as a state-controlled comparison that reconciles conflicting literature rather than adding another disconnected result.

### Why It Works
The paragraph turns a literature conflict into a mechanism boundary condition: the same variable matters differently depending on sample state.

### Transferable Rule
When results appear to conflict with prior work, identify the physical or methodological state that changes the mechanism before claiming disagreement.

### AI Instruction
If a draft says "our result differs from previous studies," require a state variable, regime boundary, or assumption difference that explains why.

## Case MCR-REF-2018-003: Archie's Exponent Is Linked to Pore-Throat Electric-Field Focusing

### Source
Physical Explanation of Archie's Porosity Exponent in Granular Materials / Geophysical Research Letters / 2018 / Section 3.3 and Discussion.

### Mechanism-Writing Type
Structure-to-signal; Observation-to-mechanism; Metric validation.

### Tags
structure_to_signal; causal_chain; metric_validation

### Context
The paper has shown that Archie's exponent increases during compaction, but the physical cause still needs pore-scale explanation.

### Result Observation
As porosity decreases, the local electric-field intensity distribution becomes more heterogeneous, with high-intensity regions increasingly concentrated near pore throats.

### Mechanism Move
The authors link the exponent to spatial variation in the electric field: denser granular packing concentrates electrical flow through pore throats, increasing the nonuniformity that raises the exponent.

### Evidence Role
Field histograms and pore-throat volume fraction provide the mechanistic bridge between a bulk exponent and pore-scale transport geometry.

### Why It Works
The metric is translated into a physical process. The reader learns what the exponent means structurally, rather than only how it changes numerically.

### Transferable Rule
For a bulk geophysical metric, explain the pore-scale redistribution of flux, exchange, or connectivity that makes the metric change.

### AI Instruction
When a draft reports a bulk metric trend, require a sentence that names the pore-scale field, pathway, or exchange process responsible for the trend.

## Case MCR-REF-2024-001: Flow Focusing Profile Turns Visual Regimes Into a Mechanism Metric

### Source
Quantifying Dissolution Dynamics in Porous Media Using a Spatial Flow Focusing Profile / Geophysical Research Letters / 2024 / Results and Discussion opening and Section 4.1.

### Mechanism-Writing Type
Metric validation; Regime comparison.

### Tags
metric_validation; regime_comparison; avoid_figure_description

### Context
The paper argues that dissolution regimes cannot be reliably distinguished by visual pattern comparison alone.

### Result Observation
The flow focusing profile decreases during uniform dissolution, develops a moving transition during wormholing, and increases across the system during channeling.

### Mechanism Move
The authors convert flow distribution into a spatial profile so that each regime is described by how flow focusing evolves along the medium, not by final appearance alone.

### Evidence Role
The profile is a quantitative replacement for visual classification and a mechanism readout of how flow paths reorganize during dissolution.

### Why It Works
The metric is introduced to solve a specific interpretive problem: visual similarity can hide different flow-evolution histories.

### Transferable Rule
A new metric is strongest when it is introduced as the answer to a named limitation of visual or qualitative interpretation.

### AI Instruction
If a draft proposes a metric, check whether the previous paragraph states what existing observation cannot distinguish and how the metric fixes that limitation.

## Case MCR-REF-2024-002: Temporal Profile Evolution Separates Channeling From Wormholing

### Source
Quantifying Dissolution Dynamics in Porous Media Using a Spatial Flow Focusing Profile / Geophysical Research Letters / 2024 / Sections 4.1-4.3.

### Mechanism-Writing Type
Regime comparison; Breakthrough or transition mechanism.

### Tags
regime_comparison; transition_explanation; causal_chain

### Context
Channeling and wormholing can produce visually similar connected pathways, so the Results must explain how their histories differ.

### Result Observation
Wormholing shows a profile transition that advances from inlet to outlet, whereas channeling shows a more uniform profile increase along preexisting pathways across the whole system.

### Mechanism Move
The authors contrast growth mechanisms: wormholes grow as an advancing dissolution front, while channeling widens initially favorable pathways along their full length because reactant penetration and heterogeneity allow broad, multi-threaded channels to develop.

### Evidence Role
The temporal profile distinguishes regime history and prevents final structure from being overinterpreted.

### Why It Works
The comparison is organized around the physical process causing divergence, not around separate descriptions of two images.

### Transferable Rule
When two regimes look similar at the end, compare their time evolution and identify the process that makes their trajectories diverge.

### AI Instruction
If a draft compares regimes by final morphology only, add the history variable that separates them: front advance, whole-path enlargement, coalescence, or homogenization.

## Case MCR-REF-2025-001: Wormholing BTC Features Are Mapped to Transport Zones

### Source
Anomalous Transport in Dissolving Porous Media: Transitions Between Fickian and Non-Fickian Regimes / Geophysical Research Letters / 2025 / Sections 3.1-3.2.

### Mechanism-Writing Type
Observation-to-mechanism; Breakthrough mechanism.

### Tags
breakthrough_mechanism; causal_chain; evidence_hierarchy

### Context
The paper must explain why wormholing changes solute transport from Fickian to non-Fickian and why the BTC develops early arrival, a plateau, and late tailing.

### Result Observation
During wormholing, the BTC evolves from a narrow distribution to one with early arrival, plateau-like behavior, and a long tail.

### Mechanism Move
The authors map each BTC feature to a transport region: fast particles move through a major wormhole, intermediate arrivals come through neighboring and secondary wormholes, and late particles are trapped in low-velocity undissolved regions.

### Evidence Role
BTC shape, particle snapshots, and velocity fields jointly assign signal features to physical transport zones.

### Why It Works
The paragraph translates curve morphology into a spatial mechanism, making the anomalous transport behavior interpretable rather than merely classified.

### Transferable Rule
For breakthrough curves or distributions, assign each curve feature to a physical pathway, storage zone, or exchange process.

### AI Instruction
When a draft reports early arrival, plateau, tailing, or multiple peaks, require a zone-by-zone mechanism explaining which particles or fluids create each feature.

## Case MCR-REF-2025-002: Uniform Dissolution Explains Non-Fickian to Fickian Transition

### Source
Anomalous Transport in Dissolving Porous Media: Transitions Between Fickian and Non-Fickian Regimes / Geophysical Research Letters / 2025 / Section 3.2.

### Mechanism-Writing Type
Observation-to-mechanism; Regime comparison.

### Tags
observation_to_mechanism; regime_comparison; causal_chain

### Context
The paper contrasts wormholing-induced heterogeneity with uniform-dissolution-induced homogenization.

### Result Observation
Under uniform dissolution, initially broad BTCs narrow, tailing weakens, velocity distributions become narrower, and the system transitions toward Fickian transport.

### Mechanism Move
The authors explain that low Damkohler conditions allow reactant penetration throughout the network, so pores dissolve more evenly. Diffusion hindrance further limits growth in larger pores, allowing smaller pores to catch up and reducing velocity heterogeneity.

### Evidence Role
Diameter distributions and velocity PDFs support the mechanism by showing that the pore network and flow field become more homogeneous.

### Why It Works
The paragraph explains both the transport outcome and the pore-growth process that causes it.

### Transferable Rule
When a regime produces a negative result such as reduced heterogeneity or weaker tailing, still explain the active process that removes the contrast.

### AI Instruction
If a draft says a system becomes "more uniform," require the mechanism that equalizes it and the transport consequence of that equalization.

## Case MCR-REF-2025-003: A Phase Diagram Synthesizes Heterogeneity and Damkohler Controls

### Source
Anomalous Transport in Dissolving Porous Media: Transitions Between Fickian and Non-Fickian Regimes / Geophysical Research Letters / 2025 / Section 3.3.

### Mechanism-Writing Type
Mini synthesis; Regime comparison.

### Tags
mini_synthesis; regime_comparison; evidence_hierarchy

### Context
After detailed mechanism sections for wormholing and uniform dissolution, the paper must generalize across initial heterogeneity and reaction-transport conditions.

### Result Observation
The phase diagram contains persistent Fickian, non-Fickian to Fickian, Fickian to non-Fickian, and persistent non-Fickian outcomes.

### Mechanism Move
The authors synthesize the previous mechanisms: wormholing increases heterogeneity and pushes transport toward non-Fickian behavior, while uniform dissolution reduces flow heterogeneity and pushes transport toward Fickian behavior; initial heterogeneity controls how far each transition can go.

### Evidence Role
The phase diagram is not just a classification map. It summarizes how initial structure and dissolution regime combine to determine transport-regime transitions.

### Why It Works
The section uses the phase diagram to compress earlier mechanism chains into a transferable rule across parameter space.

### Transferable Rule
After mechanism examples, use a map or classification figure to synthesize which control variables determine the observed transition paths.

### AI Instruction
When a Results section moves from representative cases to a phase diagram, make the phase diagram paragraph explicitly reuse the mechanisms established earlier.

## Case MCR-REF-2026-001: T2 Peak Separation Is Interpreted as Weakened Pore Coupling

### Source
How Does Fluid Exchange Between Pores in Unsaturated Porous Media / Geophysical Research Letters / 2026 / Section 3.1.

### Mechanism-Writing Type
Structure-to-signal; Observation-to-mechanism.

### Tags
structure_to_signal; observation_to_mechanism; causal_chain

### Context
The paper needs to show how NMR responses reveal pore coupling changes during desaturation.

### Result Observation
As saturation decreases, long-relaxation components weaken or disappear and the main T2 peaks become more separated.

### Mechanism Move
The authors interpret peak separation as evidence that lower saturation weakens inter-pore magnetization exchange. Water loss from larger pores and reduced pathway connectivity restrict coupling between pore environments.

### Evidence Role
Measured and simulated T2 distributions provide mutually supporting signal evidence for saturation-dependent pore coupling.

### Why It Works
The paragraph does not treat peak separation as a pore-size observation only; it links signal morphology to exchange between pore populations.

### Transferable Rule
When interpreting NMR spectra in evolving pore systems, distinguish apparent pore-size changes from coupling or exchange changes whenever connectivity is changing.

### AI Instruction
If a draft equates T2 peak shifts directly with pore size, check whether changing pore coupling or exchange could be the mechanism that needs to be stated.

## Case MCR-REF-2026-002: Off-Diagonal Exchange and Geometry Metrics Explain Coupling Loss

### Source
How Does Fluid Exchange Between Pores in Unsaturated Porous Media / Geophysical Research Letters / 2026 / Sections 3.2-3.4.

### Mechanism-Writing Type
Metric validation; Structure-to-signal; Mini synthesis.

### Tags
metric_validation; structure_to_signal; mini_synthesis

### Context
After T2 peak separation suggests weaker pore coupling, the paper needs quantitative and geometric evidence for why coupling weakens.

### Result Observation
The off-diagonal exchange amplitude in T2-store-T2 maps decreases with saturation, the renormalized coupling parameter increases, water-pathway tortuosity rises, and connectivity ratio eventually drops sharply.

### Mechanism Move
The authors use exchange-map amplitude to quantify inter-pore proton migration, then use tortuosity and connectivity metrics to explain the underlying geometry: desaturation first makes water pathways narrower and more tortuous, then disconnects them into isolated clusters.

### Evidence Role
The NMR exchange metric validates the signal interpretation, while geometry metrics explain the physical cause of the weakening coupling.

### Why It Works
The section stacks evidence in the right order: signal observation, exchange quantification, geometric cause, and final coupling mechanism.

### Transferable Rule
When a signal metric diagnoses a mechanism, pair it with an independent structural metric that explains why the signal changed.

### AI Instruction
If a Results section has both signal and structure metrics, organize them as diagnosis and cause rather than as parallel lists.
