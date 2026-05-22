# OCAR / Funnel Reference Cases

This file stores reference-paper cases for the OCAR / Funnel Structure Designer.
The cases focus on function, not sentence-level imitation: how a paper moves the
reader from a broad process, to a process-based challenge, to the study action,
and finally to a usable scientific resolution.

## Case Index

- OCAR-SELF-001: Current manuscript abstract funnel.
- OCAR-SELF-002: Current manuscript introduction funnel.
- OCAR-SELF-003: Current manuscript methods opening funnel.
- OCAR-SELF-004: Current manuscript results opening funnel.
- OCAR-REF-2018-A: Archie porosity exponent abstract funnel.
- OCAR-REF-2018-I: Archie porosity exponent introduction funnel.
- OCAR-REF-2024-A: Spatial flow focusing profile abstract funnel.
- OCAR-REF-2024-I: Spatial flow focusing profile introduction funnel.
- OCAR-REF-2025-A: Dissolution and anomalous transport abstract funnel.
- OCAR-REF-2025-I: Dissolution and anomalous transport introduction funnel.
- OCAR-REF-2026-A: Unsaturated pore coupling abstract funnel.
- OCAR-REF-2026-I: Unsaturated pore coupling introduction funnel.

## Extraction Template

```markdown
## Case OCAR-XXX: Short title

### Source
Paper title / journal / year / position

### Target Section
Abstract / Introduction / Methods opening / Results opening / Paragraph

### Tags
tag_1; tag_2; tag_3

### Central Storyline
One sentence describing the paper-level story.

### O - Opening
Text or summary:

Function:

### C - Challenge
Text or summary:

Function:

### A - Action
Text or summary:

Function:

### R - Resolution
Text or summary:

Function:

### Why This OCAR Works

### Transferable Rule

### AI Instruction
```

## Case OCAR-SELF-001: Current Manuscript Abstract Funnel

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Abstract.

### Target Section
Abstract.

### Tags
process_first_opening; method_necessity; resolution_as_takeaway; diagnostic_signature

### Central Storyline
Time-resolved NMR T2 evolution can diagnose dissolution regimes by tracking matrix-vug coupling and permeability breakthrough.

### O - Opening
Text or summary:
Mineral dissolution reorganizes pore networks through variable pathways, while non-invasive tracking remains difficult.

Function:
Opens with a physical process and its monitoring consequence, not with an application list.

### C - Challenge
Text or summary:
The unresolved problem is whether quantitative NMR signatures can diagnose carbonate dissolution dynamics.

Function:
Turns the general monitoring problem into a signal-interpretation challenge.

### A - Action
Text or summary:
The study couples pore-scale reactive transport simulations with NMR forward modeling for face dissolution, wormholing, and channeling.

Function:
The method is introduced as the necessary bridge between evolving geometry and measurable T2 responses.

### R - Resolution
Text or summary:
Distinct T2 pathways and an MVC index reveal how earlier matrix-vug exchange coincides with tortuosity reduction and efficient breakthrough.

Function:
Closes by stating what the reader can diagnose from the signal.

### Why This OCAR Works
The abstract does not stop at "we simulated dissolution and NMR." It makes the NMR signal useful by connecting it to coupling sequence and hydraulic breakthrough.

### Transferable Rule
In a mechanism-driven abstract, make the result resolve the monitoring or interpretation problem introduced in the first two sentences.

### AI Instruction
When revising an abstract, check whether the final sentence answers the Challenge in a diagnostic, reader-usable form.

## Case OCAR-SELF-002: Current Manuscript Introduction Funnel

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Introduction.

### Target Section
Introduction.

### Tags
process_first_opening; nested_funnel; generic_gap_to_process_gap; action_not_method_list

### Central Storyline
NMR can become a process-based diagnostic for dissolution regimes only if T2 evolution is linked to pore coupling and breakthrough timing.

### O - Opening
Text or summary:
Mineral dissolution reshapes pore networks and controls flow-path creation, permeability change, and leakage risk across different regimes.

Function:
Begins from process and consequence, then narrows to regime behavior and practical stakes.

### C - Challenge
Text or summary:
Current regime identification often depends on images, flow fields, or visual classification, while NMR interpretations mostly describe apparent pore size or porosity.

Function:
Builds a nested funnel: first, dissolution regimes need continuous field-applicable diagnosis; second, NMR has potential but lacks a dynamic metric for pore coupling and breakthrough.

### A - Action
Text or summary:
The study integrates reactive transport with NMR simulation, compares T2 evolution with permeability and tortuosity, and defines MVC.

Function:
Presents methods as a sequence of actions that answer the nested challenge.

### R - Resolution
Text or summary:
The framework aims to use transient T2 signals and MVC to monitor dissolution regimes, connectivity, and permeability breakthrough.

Function:
Turns the contribution into an interpretive capability, not only a modeling workflow.

### Why This OCAR Works
The funnel uses two layers of narrowing: dissolution-regime diagnosis first, then NMR-specific interpretability. This makes MVC feel necessary before it appears in Results.

### Transferable Rule
If a method is already familiar, introduce its limitation after its potential: "the method can observe X, but current interpretation cannot explain Y."

### AI Instruction
When diagnosing an Introduction, look for both the field-level gap and the method-specific gap. If either is missing, the Action will sound like a method list.

## Case OCAR-SELF-003: Current Manuscript Methods Opening Funnel

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Methods opening.

### Target Section
Methods opening.

### Tags
method_necessity; action_not_method_list; structure_signal_link

### Central Storyline
The workflow must keep dissolution geometry and NMR observables synchronized so that signal changes can be interpreted as structure changes.

### O - Opening
Text or summary:
The section opens by presenting an integrated framework that links dissolution dynamics with NMR responses.

Function:
Defines the method section as evidence logic, not as a catalog of numerical settings.

### C - Challenge
Text or summary:
Pore geometry, flow, solute concentration, hydraulic properties, and NMR observables evolve together and must be compared at matched times.

Function:
Identifies the alignment problem the workflow must solve.

### A - Action
Text or summary:
The reactive transport module resolves geometry, flow, and concentration; selected snapshots are passed into the NMR forward model.

Function:
Shows how each module contributes to the evidence chain.

### R - Resolution
Text or summary:
The synchronized framework enables direct comparison among pore-structure evolution, hydraulic properties, and NMR observables.

Function:
States why the workflow can answer the paper's central interpretation question.

### Why This OCAR Works
The opening tells readers what the workflow proves before technical equations arrive.

### Transferable Rule
A Methods opening should first name the evidence link the methods create, then introduce modules and parameters.

### AI Instruction
When a Methods section feels technical too early, add a one-paragraph OCAR opening that explains what comparison the workflow makes possible.

## Case OCAR-SELF-004: Current Manuscript Results Opening Funnel

### Source
Tracking Spatiotemporal Mineral Dissolution Through Quantitative Nuclear Magnetic Resonance Signatures / current manuscript / Results and Discussion opening.

### Target Section
Results opening.

### Tags
section_level_funnel; reader_orientation; action_not_method_list

### Central Storyline
Representative dissolution regimes provide the structural basis for interpreting NMR T2 signatures and breakthrough efficiency.

### O - Opening
Text or summary:
The simulations span a Pe-Da parameter space to generate dissolution regimes.

Function:
Defines the result space before asking readers to interpret specific cases.

### C - Challenge
Text or summary:
The full parameter map is broad, so the Results must focus on representative regimes that expose contrasting mechanisms.

Function:
Prevents the Results from becoming a parameter-sweep inventory.

### A - Action
Text or summary:
The section selects face dissolution, channeling, and wormholing cases for detailed comparison.

Function:
Turns parameter selection into a mechanism-comparison design.

### R - Resolution
Text or summary:
These regimes form the structural basis for interpreting the following T2 signatures and breakthrough efficiency.

Function:
Prepares a forward pointer to the next Results subsections.

### Why This OCAR Works
The opening tells readers why three cases are enough and what they will explain downstream.

### Transferable Rule
At the start of Results, do not only announce the dataset. State how the selected cases will function in the mechanism argument.

### AI Instruction
When Results begins with a parameter list, revise it into a section-level OCAR that explains why those cases are the right comparison set.

## Case OCAR-REF-2018-A: Archie Porosity Exponent Abstract Funnel

### Source
Niu and Zhang, Physical Explanation of Archie's Porosity Exponent in Granular Materials / Geophysical Research Letters / 2018 / Abstract.

### Target Section
Abstract.

### Tags
generic_gap_to_process_gap; mechanism_resolution; reader_usable_resolution

### Central Storyline
Archie's porosity exponent can be physically explained by pore-scale controls on the local electrical field in granular media.

### O - Opening
Text or summary:
Archie's law is widely used to interpret resistivity, but the physical basis of its exponent remains unclear.

Function:
Starts from a familiar empirical relation and identifies the missing physical meaning.

### C - Challenge
Text or summary:
The exponent varies across materials, and its controlling textural mechanism is not resolved.

Function:
Moves from a broad empirical problem to a mechanism gap.

### A - Action
Text or summary:
The study combines discrete element modeling and finite-difference electrical simulations across dilute to dense granular states.

Function:
Introduces a pore-scale tool as the way to isolate physical controls.

### R - Resolution
Text or summary:
At dilute states, particle properties dominate; as porosity decreases, pore-throat concentration and nonuniform electrical fields increase the exponent.

Function:
Provides a mechanistic explanation rather than only a fitted correlation.

### Why This OCAR Works
The abstract connects a practical empirical parameter to a specific pore-scale mechanism.

### Transferable Rule
For papers about empirical indices, make the Challenge about missing physical meaning and make the Resolution name the controlling mechanism.

### AI Instruction
If a manuscript says an index "changes," ask what microphysical redistribution makes it change.

## Case OCAR-REF-2018-I: Archie Porosity Exponent Introduction Funnel

### Source
Niu and Zhang, Physical Explanation of Archie's Porosity Exponent in Granular Materials / Geophysical Research Letters / 2018 / Introduction.

### Target Section
Introduction.

### Tags
field_background_opening; generic_gap_to_process_gap; mechanism_resolution

### Central Storyline
A pore-scale numerical study can reconcile conflicting controls on Archie's exponent by separating dilute and nondilute granular behavior.

### O - Opening
Text or summary:
Electrical and electromagnetic methods need constitutive links between measured resistivity and material properties.

Function:
Begins from the measurement-to-property translation problem.

### C - Challenge
Text or summary:
Many textural factors and geological processes have been linked to the exponent, but their roles are interrelated and no consensus exists.

Function:
Defines the gap as unresolved dominant control, not as a simple lack of studies.

### A - Action
Text or summary:
The study simulates compaction and electrical conduction in granular samples, then extracts pore attributes.

Function:
Uses numerical isolation to separate particle properties, porosity, and pore-throat effects.

### R - Resolution
Text or summary:
The intended contribution is a pore-scale link between material texture and the porosity exponent across sample states.

Function:
Signals that the paper will explain why previous controls appear inconsistent.

### Why This OCAR Works
The Introduction first establishes why the empirical parameter matters, then narrows to the unresolved physical control.

### Transferable Rule
When the literature lists many candidate controls, convert the list into a single unresolved relation among those controls.

### AI Instruction
When seeing a literature paragraph full of factors, ask: "What single physical relation has not been separated yet?"

## Case OCAR-REF-2024-A: Spatial Flow Focusing Profile Abstract Funnel

### Source
Szawello et al., Quantifying Dissolution Dynamics in Porous Media Using a Spatial Flow Focusing Profile / Geophysical Research Letters / 2024 / Abstract.

### Target Section
Abstract.

### Tags
process_first_opening; generic_gap_to_process_gap; method_necessity; temporal_resolution

### Central Storyline
A spatial flow focusing profile can quantify dissolution regimes and distinguish patterns that visual classification cannot reliably separate.

### O - Opening
Text or summary:
Dissolution patterns depend on the relative strength of flow, transport, and surface reaction.

Function:
Opens with the governing process competition.

### C - Challenge
Text or summary:
Regime distinction often relies on qualitative visual comparison of emergent structures.

Function:
Defines a classification challenge rooted in inadequate process diagnostics.

### A - Action
Text or summary:
The study proposes a spatial flow focusing profile that evaluates flow focusing along cross sections of the medium and tests it in pore-network simulations.

Function:
Introduces a metric whose spatial design matches the heterogeneous nature of dissolving systems.

### R - Resolution
Text or summary:
Temporal changes in the profile distinguish wormholing from channeling, and heterogeneity shifts regime transitions.

Function:
Shows the reader what the new metric can diagnose.

### Why This OCAR Works
The Abstract makes the metric necessary by first showing why final morphology alone is insufficient.

### Transferable Rule
When proposing a metric, explain what existing observation cannot separate and why the metric's structure matches the process.

### AI Instruction
If a metric is introduced, check whether the Challenge explains why a simpler global number or visual label is not enough.

## Case OCAR-REF-2024-I: Spatial Flow Focusing Profile Introduction Funnel

### Source
Szawello et al., Quantifying Dissolution Dynamics in Porous Media Using a Spatial Flow Focusing Profile / Geophysical Research Letters / 2024 / Introduction.

### Target Section
Introduction.

### Tags
process_first_opening; application_to_process_shift; nested_funnel; method_necessity

### Central Storyline
Dissolution regimes require a quantitative, spatial, and temporal metric because channeling and wormholing can look similar in final structure but differ in evolution.

### O - Opening
Text or summary:
Dissolution processes generate complex spatial and temporal patterns through flow, transport, reaction, and evolving medium properties.

Function:
Starts from pattern formation as a process, then connects to natural and engineered consequences.

### C - Challenge
Text or summary:
Traditional regime classification is visual and becomes difficult for adjacent regimes such as wormholing, channeling, and uniform dissolution.

Function:
Narrows the problem from "dissolution matters" to "current classification cannot reliably separate similar regimes."

### A - Action
Text or summary:
The paper constructs a flow focusing profile by slicing the medium along the flow direction and tracking focusing in space and time.

Function:
The method is justified by the fact that a dissolving medium is spatially heterogeneous and cannot be represented by one global number.

### R - Resolution
Text or summary:
Temporal profile evolution supplies the information needed to distinguish wormholing from channeling.

Function:
Makes the contribution a diagnostic capacity, not just a new descriptor.

### Why This OCAR Works
The final Action paragraph explicitly rejects an insufficient metric type before defining the new one.

### Transferable Rule
A strong metric paper often says: "A single number is not enough because the system has different regions with different functions."

### AI Instruction
For metric-building manuscripts, diagnose whether the metric's dimensionality, such as spatial or temporal structure, is motivated by the failure mode of previous classification.

## Case OCAR-REF-2025-A: Dissolution and Anomalous Transport Abstract Funnel

### Source
Deng et al., Anomalous Transport in Dissolving Porous Media: Transitions Between Fickian and Non-Fickian Regimes / Geophysical Research Letters / 2025 / Abstract.

### Target Section
Abstract.

### Tags
process_first_opening; mechanism_resolution; broad_to_specific

### Central Storyline
Dissolution regimes can switch solute transport between Fickian and non-Fickian behavior by reorganizing flow heterogeneity.

### O - Opening
Text or summary:
Mineral dissolution alters pore structures and affects fluid flow and solute transport.

Function:
Begins with a process-to-consequence chain.

### C - Challenge
Text or summary:
Dissolution produces different patterns, but their effects on solute transport dynamics need to be explained.

Function:
Focuses the problem on how evolving structure changes transport behavior.

### A - Action
Text or summary:
The study uses pore-network modeling to vary initial heterogeneity and dissolution regime.

Function:
Sets up a controlled test of structure-regime interactions.

### R - Resolution
Text or summary:
Wormholing increases heterogeneity and causes non-Fickian transport, while uniform dissolution homogenizes the network and restores Fickian transport.

Function:
Provides a two-sided mechanism that is easy for the reader to remember.

### Why This OCAR Works
The result is expressed as a regime-dependent mechanism pair, not as a loose set of observations.

### Transferable Rule
When comparing regimes, state the contrast as paired mechanisms: regime A does X because Y; regime B does the opposite because Z.

### AI Instruction
If an abstract lists multiple findings, compress them into a clear contrast table in sentence form.

## Case OCAR-REF-2025-I: Dissolution and Anomalous Transport Introduction Funnel

### Source
Deng et al., Anomalous Transport in Dissolving Porous Media: Transitions Between Fickian and Non-Fickian Regimes / Geophysical Research Letters / 2025 / Introduction.

### Target Section
Introduction.

### Tags
process_first_opening; nested_funnel; generic_gap_to_process_gap; mechanism_resolution

### Central Storyline
Solute transport in evolving porous media depends on how dissolution regimes alter heterogeneity and velocity structure.

### O - Opening
Text or summary:
Mineral dissolution changes pore structure, flow patterns, and the balance between uniform dissolution and wormholing.

Function:
Defines the evolving medium before introducing transport theory.

### C - Challenge
Text or summary:
Anomalous transport is well studied in fixed heterogeneous media, but less is known about transport when dissolution actively changes the pore structure.

Function:
Creates a nested funnel from static heterogeneity to evolving heterogeneity.

### A - Action
Text or summary:
The study simulates dissolution and solute transport in pore networks across heterogeneity levels and dissolution regimes.

Function:
Pairs the two controlling axes needed to test the Challenge.

### R - Resolution
Text or summary:
The paper aims to explain how medium heterogeneity and dissolution regime jointly shape Fickian or non-Fickian transport.

Function:
Returns to transport prediction rather than stopping at dissolution morphology.

### Why This OCAR Works
The Introduction shifts the reader from "dissolution changes pores" to "evolving pores change transport regime."

### Transferable Rule
A good nested funnel can move from a known process, to a known theory, to the unresolved case where the process changes the theory's assumptions.

### AI Instruction
When an Introduction has two fields, identify which field supplies the process and which supplies the unresolved consequence.

## Case OCAR-REF-2026-A: Unsaturated Pore Coupling Abstract Funnel

### Source
Zhou et al., How Does Fluid Exchange Between Pores in Unsaturated Porous Media? / Geophysical Research Letters / 2026 / Abstract.

### Target Section
Abstract.

### Tags
process_first_opening; method_necessity; nested_funnel; resolution_as_takeaway

### Central Storyline
NMR simulation and measurement can track how decreasing saturation weakens pore coupling by making water pathways tortuous and disconnected.

### O - Opening
Text or summary:
Inter-pore fluid exchange driven by diffusion, or pore coupling, affects pore-scale physicochemical dynamics.

Function:
Opens by defining the target process and its importance.

### C - Challenge
Text or summary:
NMR has tracked pore coupling in saturated media, but unsaturated systems are difficult because water-pathway geometry and connectivity change.

Function:
Builds a method-specific nested challenge: NMR is promising, but the target state breaks simple interpretation.

### A - Action
Text or summary:
The study combines micro-CT-based NMR simulation with measurements across samples of different pore environments and saturations.

Function:
Introduces paired simulation and validation as necessary for interpreting unsaturated NMR responses.

### R - Resolution
Text or summary:
Reduced saturation makes water pathways increasingly tortuous and eventually disconnected, restricting and then blocking pore coupling.

Function:
Turns the NMR framework into a physical interpretation of connectivity loss.

### Why This OCAR Works
The abstract introduces NMR after the target process, so the method serves the mechanism rather than replacing it.

### Transferable Rule
When a paper extends a method to a harder state, state what changes in that state make interpretation difficult.

### AI Instruction
If a manuscript says "we apply method X to condition Y," ask what physical complication in Y makes the application nontrivial.

## Case OCAR-REF-2026-I: Unsaturated Pore Coupling Introduction Funnel

### Source
Zhou et al., How Does Fluid Exchange Between Pores in Unsaturated Porous Media? / Geophysical Research Letters / 2026 / Introduction.

### Target Section
Introduction.

### Tags
process_first_opening; nested_funnel; method_necessity; reader_usable_resolution

### Central Storyline
Unsaturated pore coupling can be interpreted from NMR only by linking relaxation responses to water-pathway connectivity.

### O - Opening
Text or summary:
Subsurface pore networks govern fluid migration and storage, and diffusive exchange between pores affects heat, solute mixing, and reactions.

Function:
Starts from pore-network process and downstream physicochemical consequences.

### C - Challenge
Text or summary:
Simplified experiments and idealized simulations do not capture natural pore architecture or dynamic water-pathway connectivity under partial saturation; NMR interpretation is complicated by changing connectivity.

Function:
Creates two narrowing steps: physical mechanism unknown, then NMR response difficult to quantify.

### A - Action
Text or summary:
The study integrates micro-CT visualization, NMR T2 and T2-store-T2 simulation, and measurement validation at varying saturation.

Function:
Matches each method to a needed link: structure, signal, exchange, and validation.

### R - Resolution
Text or summary:
The framework reveals how decreasing saturation weakens pore coupling through increasingly tortuous and disconnected water pathways.

Function:
Closes by giving a mechanism that can guide NMR characterization of unsaturated media.

### Why This OCAR Works
The Introduction makes the study's multi-method design feel necessary because each method resolves a different part of the funnel.

### Transferable Rule
For multi-method papers, avoid a method list by mapping each method to one missing link in the mechanism.

### AI Instruction
When revising an Action paragraph with several tools, rewrite it as a sequence of evidence functions: visualize, simulate, validate, quantify.

## Cross-Case Transferable Rules

- Start with a physical process and consequence before listing applications.
- Convert "many studies have shown..." into "these studies still cannot explain or diagnose this process link."
- Use nested funnels when the field-level problem and method-level limitation are both important.
- Introduce a new metric only after explaining why existing visual, global, or bulk descriptors fail.
- For Methods openings, state the evidence link created by the workflow before giving equations and parameters.
- For Results openings, explain why selected cases are mechanistically representative.
- Make Resolution reader-usable: what can now be diagnosed, separated, predicted, or interpreted?
- Pair contrasting regimes as contrasting mechanisms rather than as parallel descriptions.
- If a method is promising but insufficient, state both parts explicitly.
- Keep technical details after their function is clear.
