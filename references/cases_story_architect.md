# Scientific Story Architect Case Library

Purpose: extract how high-quality papers define one central story, assign a main character, keep methods and metrics as supporting actors, and use section and figure sequence to protect the storyline.

Use these cases as reference examples before applying OCAR, mechanism results, paragraph engineering, or sentence hierarchy.

## Case 1: NMR Signatures Track Dissolution-Driven Pore Coupling

## Source

Paper title: Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures
Journal: GRL target manuscript
Year: current manuscript draft
Section inspected: Key Points, Abstract, Introduction, Methods, Results and Discussion, Implications, Conclusions
Figures inspected: Figures 1-3

## Core Story

Time-resolved NMR T2 pathways can diagnose matrix-vug pore coupling during carbonate dissolution, and earlier coupling explains more efficient permeability breakthrough.

## Central Scientific Question

Can time-varying NMR T2 spectra diagnose dissolution-driven pore coupling and explain why different dissolution regimes reach permeability breakthrough at different times?

## Main Character

Dissolution-driven matrix-vug pore coupling.

## Supporting Actors

- Supporting actor 1: Coupled pore-scale reactive transport and NMR forward modeling.
- Supporting actor 2: Regime-specific T2 pathway shapes, including peak separation, overlap, and merging.
- Supporting actor 3: Permeability, tortuosity, and MVC as hydraulic and spectral validation of coupling.

## Potential Distractions

RTM implementation details, Pe-Da parameter sweep details, finite-element NMR numerical settings, and spatial T2 profiles can easily become parallel technical stories. They should stay subordinate to the question of whether NMR detects coupling and breakthrough mechanisms.

## Section-Level Storyline

| Section | Function in the story |
|---|---|
| Abstract | States the diagnostic claim: NMR signatures track dissolution dynamics and earlier matrix-vug exchange coincides with efficient breakthrough. |
| Introduction | Defines the gap: existing NMR interpretations mainly describe apparent pore size or porosity, but not dynamic regime-specific connectivity and breakthrough timing. |
| Methods | Builds the evidence bridge from evolving dissolution geometries to synchronized T2, permeability, tortuosity, and MVC outputs. |
| Results 1 | Shows the first layer of evidence: face dissolution, channeling, and wormholing produce distinct T2 pathways. |
| Results 2 | Tests whether the T2 interpretation corresponds to hydraulic reorganization using tortuosity. |
| Results 3 | Quantifies matrix-vug coupling with MVC and links early coupling to breakthrough efficiency. |
| Discussion | Broadens the story from simulated regimes to non-invasive monitoring of reactive pore-structure evolution. |
| Conclusion | Returns to the take-home message: transient NMR T2 evolution provides diagnostic signatures of pore coupling and permeability breakthrough efficiency. |

## Figure Sequence Logic

| Figure | Story function |
|---|---|
| Figure 1 | Establishes the coupled reactive transport-NMR framework, so the reader knows how geometry becomes signal. |
| Figure 2 | Shows the core phenomenon: each dissolution regime produces a diagnostic T2 pathway. |
| Figure 3 | Converts the phenomenon into mechanism by linking T2 stages to permeability, tortuosity, and MVC. |

## Why This Story Works

The manuscript does not treat RTM, NMR, tortuosity, and MVC as independent outputs. The story moves from observable signal to hydraulic validation to coupling quantification. Each later metric exists because the previous result creates a specific question: does the spectral pathway reflect flow-path optimization, and can that coupling be quantified?

## Transferable Rule

When a paper contains multiple methods and metrics, identify one physical process as the main character; methods and metrics should validate, quantify, or explain that process rather than become parallel claims.

## AI Instruction

When AI faces a similar manuscript, first name the physical process that carries the paper. Then force every method, metric, figure, and subsection to answer one of three roles: reveal the process, validate it, or quantify its consequence.

## Case 2: Pore Throats Explain Archie's Porosity Exponent

## Source

Paper title: Physical Explanation of Archie's Porosity Exponent in Granular Materials: A Process-Based, Pore-Scale Numerical Study
Journal: Geophysical Research Letters
Year: 2018
Section inspected: Key Points, Abstract, Introduction, Methods, Results, Discussion, Conclusions
Figures inspected: Figures 1-5

## Core Story

Archie's porosity exponent is not only an empirical fitting parameter; in granular materials, its increase during compaction is explained by progressively concentrated electrical flow through pore throats.

## Central Scientific Question

What pore-scale textural feature physically controls Archie's porosity exponent across dilute and dense granular states?

## Main Character

Pore-throat-controlled concentration of the local electrical field.

## Supporting Actors

- Supporting actor 1: DEM-based sample preparation across dilute, loose, and dense states.
- Supporting actor 2: Finite-difference effective conductivity calculations.
- Supporting actor 3: Particle-shape theory at dilute states and pore-throat volume fraction at dense states.

## Potential Distractions

Particle preparation details, particle size distributions, numerical voxelization, and competing historical interpretations of Archie law should not obscure the main mechanism: dense-state electrical flow becomes concentrated near pore throats.

## Section-Level Storyline

| Section | Function in the story |
|---|---|
| Abstract | States the two-level answer: dilute-state m depends on particle properties; dense-state m rises with electric-field nonuniformity and pore-throat volume. |
| Introduction | Opens with the practical importance of resistivity interpretation, then defines the unresolved physical meaning of m. |
| Methods | Generates controlled granular states and computes conductivity so m can be tied to pore-scale geometry rather than fitted statistically. |
| Results 1 | Shows that m varies systematically with porosity and particle properties. |
| Results 2 | Separates dilute-state particle-shape control from dense-state evolution. |
| Results 3 | Uses electric-field maps to explain why m increases as porosity decreases. |
| Discussion | Converts the visual/electrical pattern into a transferable pore-throat volume correlation. |
| Conclusion | Repeats the mechanism: m increases because electric flow becomes increasingly nonuniform and throat-focused. |

## Figure Sequence Logic

| Figure | Story function |
|---|---|
| Figure 1 | Establishes how sample states are created, making porosity evolution controlled rather than arbitrary. |
| Figure 2 | Shows the problem pattern: m changes from dilute to dense states. |
| Figure 3 | Explains the dilute-state baseline through particle shape and orientation. |
| Figure 4 | Reveals the mechanism: dense samples concentrate electrical flow near contacts and throats. |
| Figure 5 | Converts the mechanism into a compact rule by collapsing samples onto pore-throat volume fraction. |

## Why This Story Works

The paper first isolates the baseline factor at dilute states, then explains why that baseline fails under compaction. The final correlation is persuasive because it arrives after the field-map mechanism, not before it.

## Transferable Rule

A strong mechanism paper can let one empirical relationship remain in the background while making the physical origin of its parameter the actual protagonist.

## AI Instruction

When AI reads a parameter-explanation paper, do not summarize the parameter alone. Identify the physical structure or process that makes the parameter change, then check whether the figure sequence moves from pattern to mechanism to transferable predictor.

## Case 3: Flow Focusing Profile Quantifies Dissolution Regimes

## Source

Paper title: Quantifying Dissolution Dynamics in Porous Media Using a Spatial Flow Focusing Profile
Journal: Geophysical Research Letters
Year: 2024
Section inspected: Key Points, Abstract, Introduction, Pore Network Model, Flow Focusing Profile, Results and Discussion, Conclusions
Figures inspected: Figures 1-4

## Core Story

A spatial flow focusing profile turns qualitative dissolution-regime classification into a quantitative space-time diagnostic, especially for distinguishing wormholing from channeling.

## Central Scientific Question

Can dissolution regimes that look visually similar be distinguished quantitatively from the spatial and temporal evolution of flow focusing?

## Main Character

The flow focusing profile as a dynamic regime diagnostic.

## Supporting Actors

- Supporting actor 1: Pore network dissolution model used to generate controlled regime evolution.
- Supporting actor 2: Cross-section-based flow focusing index f50%.
- Supporting actor 3: Morphological phase diagram and heterogeneity sweep.

## Potential Distractions

Network-model equations, parameter-space coverage, and transport-parameter details can pull attention away from the central point that the profile's evolution, not final morphology alone, distinguishes regimes.

## Section-Level Storyline

| Section | Function in the story |
|---|---|
| Abstract | Announces the new quantitative measure and its key payoff: temporal profile changes distinguish wormholing and channeling. |
| Introduction | Defines the gap: visual comparison is insufficient, especially for subtly different dissolution regimes. |
| Methods | Supplies a controlled pore network model so the proposed profile can be tested across regimes. |
| Results 1 | Defines and illustrates the flow focusing profile. |
| Results 2 | Shows representative uniform, wormholing, and channeling profile behaviors. |
| Results 3 | Extends the diagnostic to phase diagrams and demonstrates the role of heterogeneity. |
| Discussion | Interprets why final structures can look similar while their profile histories differ. |
| Conclusion | Returns to the rule that spatial plus temporal flow-focusing information is needed for robust regime classification. |

## Figure Sequence Logic

| Figure | Story function |
|---|---|
| Figure 1 | Introduces the network model and the flow focusing index/profile calculation. |
| Figure 2 | Shows the core diagnostic contrast among uniform dissolution, channeling, and wormholing. |
| Figure 3 | Tests the profile across parameter space and builds the morphological phase diagram. |
| Figure 4 | Shows that heterogeneity shifts the regime and that similar final structures can have different histories. |

## Why This Story Works

The paper's metric is not introduced as a generic new index. It is motivated by a classification failure, demonstrated on representative cases, then stress-tested against parameter and heterogeneity variation.

## Transferable Rule

If a paper proposes a metric, its story should begin with the specific judgment the old approach cannot make; the metric then becomes necessary rather than decorative.

## AI Instruction

When AI faces a metric paper, ask what ambiguity the metric resolves. Then check that the figures first define the metric, then demonstrate its distinguishing power, and only then generalize it.

## Case 4: Dissolution Regimes Switch Transport Behavior

## Source

Paper title: Anomalous Transport in Dissolving Porous Media: Transitions Between Fickian and Non-Fickian Regimes
Journal: Geophysical Research Letters
Year: 2025
Section inspected: Key Points, Abstract, Introduction, Methods, Results and Discussions, Conclusions
Figures inspected: Figures 1-5

## Core Story

Dissolution can switch solute transport regimes because wormholing creates preferential pathways and stagnation zones that produce non-Fickian transport, whereas uniform dissolution homogenizes flow and restores Fickian transport.

## Central Scientific Question

How do initial pore-network heterogeneity and dissolution regime determine whether solute transport becomes Fickian or non-Fickian as the pore structure evolves?

## Main Character

Dissolution-induced alteration of flow-field heterogeneity.

## Supporting Actors

- Supporting actor 1: Pore network dissolution model across uniform and wormholing regimes.
- Supporting actor 2: Passive particle tracking and breakthrough curves as transport diagnostics.
- Supporting actor 3: Velocity PDFs and phase diagram linking initial heterogeneity and Damkohler number to transport transitions.

## Potential Distractions

Detailed reaction-rate equations, particle-tracking settings, and the G parameter should stay in service of the main mechanism: dissolution changes heterogeneity, and heterogeneity changes transport behavior.

## Section-Level Storyline

| Section | Function in the story |
|---|---|
| Abstract | States the contrast: wormholing drives Fickian-to-non-Fickian transition; uniform dissolution drives non-Fickian-to-Fickian transition. |
| Introduction | Connects dissolution pattern formation with the underexplored problem of solute transport in evolving rocks. |
| Methods | Couples dissolution simulation with passive solute transport so structural change and BTC evolution can be compared. |
| Results 1 | Shows the two headline transport transitions using BTCs and particle maps. |
| Results 2 | Explains the mechanism through diameter fields and velocity heterogeneity. |
| Results 3 | Generalizes the result into a phase diagram controlled by initial heterogeneity and Damkohler number. |
| Discussion | Interprets distinctive BTC features such as early arrival, plateau behavior, and late-time tailing as signatures of correlated dissolution structures. |
| Conclusion | Returns to prediction: transport behavior can be anticipated from initial heterogeneity and reaction-flow regime. |

## Figure Sequence Logic

| Figure | Story function |
|---|---|
| Figure 1 | Establishes the pore network, boundary conditions, and initial heterogeneity controls. |
| Figure 2 | Shows the core phenomenon: BTCs switch transport regimes during dissolution. |
| Figure 3 | Explains the wormholing mechanism through preferential pathways and increased velocity heterogeneity. |
| Figure 4 | Explains the uniform dissolution mechanism through homogenized diameter and velocity fields. |
| Figure 5 | Converts the mechanism into a phase diagram of possible transport-transition types. |

## Why This Story Works

The paper does not merely report that BTCs change. It assigns opposite transport outcomes to opposite structural mechanisms, then uses the phase diagram to make the mechanism predictive.

## Transferable Rule

For mechanism papers with two contrasting regimes, make the contrast symmetric: name what each regime does to the same controlling variable, then show how that variable changes the observed behavior.

## AI Instruction

When AI analyzes a regime-comparison paper, identify the common mediator that both regimes affect. In this case, dissolution regime affects flow heterogeneity, which then controls transport.

## Case 5: Saturation Controls Pore Coupling Through Water-Pathway Connectivity

## Source

Paper title: How Does Fluid Exchange Between Pores in Unsaturated Porous Media?
Journal: Geophysical Research Letters
Year: 2026
Section inspected: Key Points, Abstract, Introduction, Experimental and Simulation Methods, Results and Discussions, Geophysical Implications, Conclusion
Figures inspected: Figures 1-3

## Core Story

Decreasing saturation weakens and eventually blocks pore coupling because water pathways become increasingly tortuous and disconnected, and this coupling loss can be tracked by NMR T2 and T2-store-T2 responses.

## Central Scientific Question

How does decreasing saturation alter inter-pore fluid exchange, and can NMR quantify the resulting pore-coupling evolution in unsaturated porous media?

## Main Character

Saturation-controlled water-pathway connectivity as the mechanism governing pore coupling.

## Supporting Actors

- Supporting actor 1: Micro-CT-based pore and phase visualization.
- Supporting actor 2: NMR T2 distributions and T2-store-T2 maps from simulation and measurement.
- Supporting actor 3: Coupling and pathway metrics, including off-diagonal map amplitude, water-pathway tortuosity, and connectivity ratio.

## Potential Distractions

Pulse-sequence settings, inversion details, image clustering, and surface-relaxivity calibration can become technical side stories. Their function is to validate the coupling signal and explain its physical control.

## Section-Level Storyline

| Section | Function in the story |
|---|---|
| Abstract | States the mechanism: reduced saturation creates tortuous and disconnected water pathways that restrict and block pore coupling. |
| Introduction | Defines why pore coupling matters and why unsaturated conditions remain hard to quantify with NMR. |
| Methods | Integrates micro-CT, NMR simulation, and NMR measurement so pore geometry, phase distribution, and signal response can be compared. |
| Results 1 | Shows how T2 distributions reveal weakening coupling as saturation decreases. |
| Results 2 | Quantifies inter-pore exchange using T2-store-T2 off-diagonal features. |
| Results 3 | Explains the signal change through water-pathway tortuosity and disconnection. |
| Discussion | Extends the mechanism to geophysical interpretation of unsaturated subsurface systems. |
| Conclusion | Repeats the main mechanism and method payoff: NMR can monitor saturation-dependent pore coupling. |

## Figure Sequence Logic

| Figure | Story function |
|---|---|
| Figure 1 | Defines coupled versus uncoupled pore systems and presents the integrated measurement-simulation workflow. |
| Figure 2 | Shows the observable NMR evidence: T2 distributions and T2-store-T2 maps change with saturation. |
| Figure 3 | Links the NMR signal to mechanism through off-diagonal amplitude, coupling parameter, tortuosity, and connectivity. |

## Why This Story Works

The paper keeps the method technically rich but story-simple. NMR outputs are introduced as observations; micro-CT-derived pathway metrics explain why those observations change; the Discussion then returns to the monitoring value of the same coupling mechanism.

## Transferable Rule

When a method measures an invisible exchange process, pair the signal with an independent structural visualization so the signal is interpreted as mechanism, not just correlation.

## AI Instruction

When AI faces a signal-interpretation paper, separate three layers: the invisible process, the observable signal, and the independent structural explanation. The story should move through those layers in that order.
