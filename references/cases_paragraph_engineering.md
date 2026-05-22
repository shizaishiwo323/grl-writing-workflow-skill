# Cases for Paragraph Engineering

Purpose: store paragraph-level writing-function cases that teach AI how a high-quality paragraph carries one clear role through topic sentence, evidence order, mechanism explanation, local echo, and mini-implication.

Use this file when revising a paragraph that has useful scientific material but unclear paragraph function, weak opening sentence, disordered evidence, buried mechanism, weak paragraph-to-paragraph transition, or an ending that stops at data rather than returning to the argument.

These cases are extracted from reference papers in `范例文章/` and from the current manuscript revision history. Target paragraphs are summarized or lightly excerpted to preserve structure-function lessons rather than to create a sentence bank.

## Case Types
1. Function-first topic sentence
2. Evidence order
3. Observation-to-mechanism paragraph
4. Paragraph-to-paragraph echo
5. Mini-implication ending
6. Detail compression / detail repositioning

## Case Index

### Reference Paper Cases

- PE-REF-2024-001: PE-TOPIC / Flow focusing profile opens by naming its diagnostic function.
- PE-REF-2026-001: PE-TOPIC / Results opening assigns the integrated framework one task.
- PE-REF-2024-002: PE-ORDER / Channeling paragraph orders visual contrast before metric behavior.
- PE-REF-2025-001: PE-ORDER / BTC paragraph orders transport zones before curve features.
- PE-REF-2018-001: PE-MECH / Electric-field heterogeneity turns an exponent trend into mechanism.
- PE-REF-2026-002: PE-MECH / Water-pathway geometry explains weakening pore coupling.
- PE-REF-2025-002: PE-ECHO / Transport observations create the need for mechanism analysis.
- PE-REF-2026-003: PE-ECHO / T2 peak separation prepares quantitative exchange mapping.
- PE-REF-2024-003: PE-END / Heterogeneity paragraph ends by upgrading metric value.
- PE-REF-2025-003: PE-END / BTC comparison ends by turning curve shape into diagnostic inference.

### Self Manuscript Cases

- PE-SELF-001: PE-COMPRESS / Tortuosity details are compressed into hydraulic validation.
- PE-SELF-002: PE-MECH / Channeling paragraph maps conduit growth to T2 merging and breakthrough.
- PE-SELF-003: PE-END / MVC paragraph turns metric timing into breakthrough mechanism.

## Extraction Template

```markdown
## Case PE-XXX: Short Title

### Source
Paper title / section / paragraph location

### Case Type
PE-TOPIC / PE-ORDER / PE-MECH / PE-ECHO / PE-END / PE-COMPRESS

### Paragraph Function
orient / define / compare / validate / interpret / conclude

### Target Skill Problem
topic sentence / evidence order / mechanism buried / evidence overload / weak ending / weak paragraph echo

### Tags
- paragraph_function: interpret
- problem_type: mechanism_buried
- section: Results
- stage: Stage 3
- shared_with: mechanism_results

### Previous Context
What question or pressure did the previous paragraph or subsection leave?

### Target Paragraph
Structural summary or short excerpt of the paragraph.

### Next Context
How does the next paragraph or subsection continue?

### Why This Paragraph Works
Explain paragraph structure, not content quality alone.

### Sentence-Level Function Map
S1: topic / orientation / claim
S2: observation / evidence
S3: mechanism / interpretation
S4: supporting evidence
S5: mini-implication / transition

### Transferable Rule
Reusable rule for future paragraph revision.

### AI Instruction
When the user gives a similar paragraph, what should AI check or revise first?
```

## Case PE-REF-2024-001: Flow Focusing Profile Opens by Naming Its Diagnostic Function

### Source
Szawełło et al., "Quantifying Dissolution Dynamics in Porous Media Using a Spatial Flow Focusing Profile" / Section 3, Flow Focusing Profile / opening paragraphs.

### Case Type
PE-TOPIC.

### Paragraph Function
define.

### Target Skill Problem
topic sentence; detail-before-function; metric introduced as method detail.

### Tags
- paragraph_function: define
- problem_type: topic_sentence
- section: Methods-to-Results bridge
- stage: Stage 3
- shared_with: mechanism_results / section_logic

### Previous Context
The Introduction argues that visual comparison is insufficient for distinguishing dissolution regimes, especially channeling versus wormholing. The model section has already described the pore network and governing parameters.

### Target Paragraph
The paragraph first states that the authors study spatial variation and temporal evolution of flow paths to determine dissolution regime. It then defines the flow focusing index for each cross section, explains what low and high values mean, and only afterward describes how a full profile is obtained along the flow direction.

### Next Context
The next paragraph moves from the definition to implementation in the pore network model: slicing the network, selecting edges that carry half the flow, and constructing the profile across the entire network.

### Why This Paragraph Works
The first sentence assigns the paragraph's function before the equation arrives. The metric is not presented as an isolated formula; the reader already knows it is being introduced to diagnose dissolution regimes. The details then proceed from purpose to definition to physical interpretation.

### Sentence-Level Function Map
S1: states the diagnostic task of studying flow-path variation.
S2: defines the index and its calculation target.
S3: explains the low-index physical limit.
S4: explains the high-index physical limit.
S5: generalizes from a local index to a spatial profile.

### Transferable Rule
When introducing a new metric, open with the metric's role in the argument before giving its formula or calculation procedure.

### AI Instruction
If a draft starts a paragraph with an equation or metric definition, first ask: "What problem does this metric solve in the manuscript?" Rewrite the topic sentence to name that function.

## Case PE-REF-2026-001: Results Opening Assigns the Integrated Framework One Task

### Source
Zhou et al., "How Does Fluid Exchange Between Pores in Unsaturated Porous Media?" / Section 3, Results and Discussions / opening paragraph.

### Case Type
PE-TOPIC.

### Paragraph Function
orient.

### Target Skill Problem
topic sentence; weak section opening; evidence not assigned to a central function.

### Tags
- paragraph_function: orient
- problem_type: weak_topic_sentence
- section: Results
- stage: Stage 3
- shared_with: story_architect / mechanism_results

### Previous Context
The Methods section has introduced NMR simulation, laboratory measurement, microCT imaging, and image-based pore network construction. Without framing, these could feel like parallel tools.

### Target Paragraph
The Results opening states that microCT-based NMR simulation and experimental validation are combined to quantify saturation-dependent pore coupling. It then names the two NMR outputs and the physical interpretation they will support: progressive weakening of coupling as saturation decreases, linked to tortuous and disconnected water pathways.

### Next Context
Section 3.1 starts with T2 distributions and explains how saturation-dependent peak behavior reveals pore coupling effects.

### Why This Paragraph Works
The paragraph compresses multiple methods into one results function. It tells the reader that the framework is not a tool inventory; it is a way to quantify weakening pore coupling and connect NMR response to water-pathway geometry.

### Sentence-Level Function Map
S1: states the integrated framework and its quantification task.
S2: names the two signal outputs and their shared conclusion.
S3: states the physical pathway interpretation.
S4: frames the framework as quantitative tracking rather than descriptive comparison.

### Transferable Rule
At the start of Results, convert a list of tools into one functional claim about what those tools jointly reveal.

### AI Instruction
When a Results opening lists methods or figures, rewrite it so the first sentence says what mechanism the combined evidence will resolve.

## Case PE-REF-2024-002: Channeling Paragraph Orders Visual Contrast Before Metric Behavior

### Source
Szawełło et al., "Quantifying Dissolution Dynamics in Porous Media Using a Spatial Flow Focusing Profile" / Section 4.1, Dissolution Regimes / channeling paragraph following Figure 2.

### Case Type
PE-ORDER.

### Paragraph Function
compare.

### Target Skill Problem
evidence order; comparison without hierarchy; mechanism buried.

### Tags
- paragraph_function: compare
- problem_type: evidence_order
- section: Results and Discussion
- stage: Stage 3
- shared_with: mechanism_results / narrative_echo

### Previous Context
The previous paragraph explains the uniform and wormholing examples in Figure 2, including how their flow focusing profiles evolve.

### Target Paragraph
The channeling paragraph starts by saying the middle-column case looks partly similar to wormholing because a main flow path appears, then immediately identifies what is structurally different: multiple pores enlarge along the full system length and branch near inlet and outlet. The next paragraph states the mechanism: preexisting flow pathways widen along their entire length, so the profile increases across the medium instead of forming an advancing sigmoidal front.

### Next Context
The following section expands from representative examples to a broader parameter sweep and morphological phase diagram.

### Why This Paragraph Works
The paragraph does not begin with every visual detail. It first tells the reader which comparison matters, then names the distinguishing structural feature, then lets the metric behavior explain why this is channeling rather than wormholing.

### Sentence-Level Function Map
S1: comparison topic: channeling resembles wormholing in one visible respect.
S2: contrast: the pathway is structurally different.
S3: evidence: enlargement occurs along the entire length.
S4: evidence: branching near inlet and outlet adds pattern detail.
S5: classification: the behavior is identified as channeling.

### Transferable Rule
For regime comparison paragraphs, order evidence as shared feature -> discriminating feature -> mechanism/metric reason -> regime label.

### AI Instruction
If a draft compares two regimes by listing many observations, identify the one discriminating feature first and move secondary visual details after it.

## Case PE-REF-2025-001: BTC Paragraph Orders Transport Zones Before Curve Features

### Source
Deng et al., "Anomalous Transport in Dissolving Porous Media: Transitions Between Fickian and Non-Fickian Regimes" / Section 3.2 / final-stage wormholing transport paragraph.

### Case Type
PE-ORDER.

### Paragraph Function
interpret.

### Target Skill Problem
evidence order; mechanism buried; curve description before physical zones.

### Tags
- paragraph_function: interpret
- problem_type: evidence_order
- section: Results and Discussion
- stage: Stage 3
- shared_with: mechanism_results

### Previous Context
The preceding paragraph explains that intermediate-stage wormholes create multiple particle arrival times and that unreacted regions become trapping zones.

### Target Paragraph
The paragraph first divides the final-stage flow field into three transport regions: a highly permeable main channel, lower-permeability secondary channels, and low-velocity minimally dissolved regions. It then maps these regions onto BTC features: early arrival, plateau, and power-law tailing. Finally, it states that the BTC shape is the combined contribution of the three zones and that breakthrough of the leading wormhole drives the change from intermediate to final BTC shape.

### Next Context
The next paragraph turns to the uniform dissolution regime and contrasts homogenization against wormholing-induced flow focusing.

### Why This Paragraph Works
The paragraph places physical zones before curve features. This prevents the BTC from becoming a descriptive signal and makes the curve a readable outcome of a spatial transport partition.

### Sentence-Level Function Map
S1: states the stage and partitions the flow field into three zones.
S2: maps zones to three tracer breakthrough behaviors.
S3: explains early arrival through the main wormhole.
S4: explains plateau through nearby and secondary-channel particles.
S5: explains tailing through low-velocity regions.
S6: concludes that BTC shape is the summed contribution of the zones.
S7: transitions by identifying leading-wormhole breakthrough as the stage-change driver.

### Transferable Rule
When interpreting a signal curve, introduce the physical compartments or pathways first, then assign each curve feature to one compartment.

### AI Instruction
If a paragraph starts by describing curve morphology, ask which physical regions generate each feature and reorder the paragraph around that mapping.

## Case PE-REF-2018-001: Electric-Field Heterogeneity Turns an Exponent Trend Into Mechanism

### Source
Niu and Zhang, "Physical Explanation of Archie's Porosity Exponent in Granular Materials" / Section 3.3, Evolution of m / opening mechanism paragraph.

### Case Type
PE-MECH.

### Paragraph Function
interpret.

### Target Skill Problem
mechanism buried; observation-to-mechanism; abstract parameter not physically grounded.

### Tags
- paragraph_function: interpret
- problem_type: mechanism_buried
- section: Results
- stage: Stage 3
- shared_with: mechanism_results / sentence_hierarchy

### Previous Context
Earlier Results show that Archie's porosity exponent varies with porosity, particle shape, and particle size range. The remaining question is what physical process makes m increase as granular materials become denser.

### Target Paragraph
The paragraph starts from the unexplained trend in m, then introduces the formation factor in terms of electric-field energy in pore space. It explains that a uniform local electric field would make m close to unity, whereas complex pore geometry creates nonuniform fields that increase m. The paragraph ends by interpreting change in m as an indicator of spatial variation in local electric-field strength.

### Next Context
The following paragraph applies this interpretation to five compaction states and shows that the field-strength distribution becomes more heterogeneous as solid concentration increases.

### Why This Paragraph Works
The paragraph converts an empirical exponent into a physical observable. It does not merely add equations; it uses the equations to define what kind of pore-scale heterogeneity m is measuring.

### Sentence-Level Function Map
S1: states the unresolved physical cause of increasing m.
S2: introduces the formation-factor expression.
S3: derives the microscopic interpretation of m.
S4: gives the simple uniform-field limit.
S5: contrasts real pore geometry and nonuniform fields.
S6: states the mechanism-level meaning of m variation.

### Transferable Rule
When a result is an abstract fitted parameter, add a paragraph that translates the parameter into a physical field, geometry, or process before interpreting trends.

### AI Instruction
If a draft says a fitted exponent "increases" or "decreases" without physical meaning, require one sentence that defines what the parameter represents mechanistically.

## Case PE-REF-2026-002: Water-Pathway Geometry Explains Weakening Pore Coupling

### Source
Zhou et al., "How Does Fluid Exchange Between Pores in Unsaturated Porous Media?" / Section 3.4, Determinants of Pore Coupling Effect Under Unsaturated Conditions / final mechanism paragraph.

### Case Type
PE-MECH.

### Paragraph Function
interpret.

### Target Skill Problem
observation-to-mechanism; mechanism buried; weak synthesis after metric analysis.

### Tags
- paragraph_function: interpret
- problem_type: mechanism_buried
- section: Results and Discussion
- stage: Stage 3
- shared_with: mechanism_results / narrative_echo

### Previous Context
The preceding paragraphs define tortuosity, connectivity ratio, characteristic diffusion length, and a renormalized coupling parameter. They show how these quantities vary with saturation.

### Target Paragraph
The paragraph synthesizes the metric evolution into a mechanism sequence: decreasing saturation reduces inter-pore-channel water, which narrows and tortuously lengthens water pathways, restricting molecular exchange. At lower saturation, insufficient water breaks connectivity, splits the connected water space into small clusters, and finally isolates pore environments so fluid diffusion and pore coupling are blocked.

### Next Context
The next section moves to geophysical implications, explaining how NMR interpretation and hydraulic-property estimation can benefit from tracking pore coupling.

### Why This Paragraph Works
The paragraph arrives after the metrics have been established, so it can compress them into a clear mechanism chain. It moves from geometry change to diffusion constraint to connectivity loss to NMR-relevant coupling loss.

### Sentence-Level Function Map
S1: announces that saturation-induced geometry and connectivity govern coupling strength.
S2: mechanism step: reduced water narrows and lengthens pathways.
S3: consequence: diffusion paths become longer and exchange is restricted.
S4: lower-saturation step: connectivity fails and clusters form.
S5: final consequence: isolated pores block diffusion and eliminate coupling.

### Transferable Rule
After several supporting metrics, end the paragraph sequence with a causal mechanism chain that uses the metrics as evidence rather than repeating their trends.

### AI Instruction
If a paragraph lists metric changes, rewrite the ending as "variable change -> geometry/process change -> transport/signal consequence."

## Case PE-REF-2025-002: Transport Observations Create the Need for Mechanism Analysis

### Source
Deng et al., "Anomalous Transport in Dissolving Porous Media: Transitions Between Fickian and Non-Fickian Regimes" / Section 3.1 ending to Section 3.2 opening.

### Case Type
PE-ECHO.

### Paragraph Function
orient.

### Target Skill Problem
weak paragraph echo; abrupt section transition; new subsection starts without inheriting previous question.

### Tags
- paragraph_function: orient
- problem_type: weak_paragraph_echo
- section: Results and Discussion
- stage: Stage 3
- shared_with: narrative_echo / mechanism_results

### Previous Context
Section 3.1 establishes that wormholing shifts transport from Fickian to non-Fickian and uniform dissolution shifts transport from non-Fickian to Fickian. It also notes that dissolution-induced non-Fickian behavior differs from random preexisting heterogeneity.

### Target Paragraph
Section 3.2 opens by stating that, to elucidate mechanisms driving the transport-regime transition during dissolution, the authors now analyze flow fields and dissolution patterns in detail. It then previews that wormholing and uniform regimes produce distinct patterns and heterogeneity alterations, which are shown in the next figures.

### Next Context
The following paragraphs explain the wormholing feedback loop and then the uniform-dissolution homogenization process.

### Why This Paragraph Works
The subsection opening inherits the unresolved "why" from the previous subsection. It prevents the next figures from feeling like extra data by framing them as the mechanism needed to explain the observed transport transitions.

### Sentence-Level Function Map
S1: backward link: names the need to explain transport-regime transitions.
S2: method of explanation: analyze flow fields and dissolution patterns.
S3: forward pointer: names the two regimes and the figures that will support the mechanism.

### Transferable Rule
When a new subsection follows a descriptive result, its opening should state the unresolved mechanism that the new evidence will explain.

### AI Instruction
If a Results subsection begins with a new figure, add a backward-link sentence that says which observation from the previous subsection now requires mechanism explanation.

## Case PE-REF-2026-003: T2 Peak Separation Prepares Quantitative Exchange Mapping

### Source
Zhou et al., "How Does Fluid Exchange Between Pores in Unsaturated Porous Media?" / Section 3.1 ending to Section 3.2 opening.

### Case Type
PE-ECHO.

### Paragraph Function
orient.

### Target Skill Problem
weak paragraph echo; signal observation not connected to next analysis; evidence overload.

### Tags
- paragraph_function: orient
- problem_type: weak_paragraph_echo
- section: Results and Discussion
- stage: Stage 3
- shared_with: narrative_echo / mechanism_results

### Previous Context
Section 3.1 shows that T2 peaks merge at high saturation and separate as saturation decreases, implying weakened pore coupling. It also states that the underlying mechanisms need further analysis.

### Target Paragraph
Section 3.2 opens by assigning the T2-store-T2 map a new role: it qualitatively assesses inter-pore magnetization exchange and provides insight into the degree of pore coupling. The paragraph then explains diagonal peaks as protons remaining in their pore environments and off-diagonal peaks as exchange between large and small pores.

### Next Context
The next paragraphs use off-diagonal peak asymmetry and amplitude decline to quantify progressive weakening of pore coupling with decreasing saturation.

### Why This Paragraph Works
The paragraph transforms the previous section's qualitative signal observation into a need for exchange mapping. It defines just enough of the new tool for the reader to understand how the next evidence will resolve the previous question.

### Sentence-Level Function Map
S1: topic: T2-store-T2 map provides exchange-based coupling assessment.
S2: setup: axes and peak categories are defined.
S3: interpretation: diagonal peaks mean no exchange.
S4: interpretation: off-diagonal peaks mean inter-pore exchange.
S5: transition: monitoring off-diagonal peaks enables quantitative coupling estimation.

### Transferable Rule
When moving from one signal representation to another, state what the second representation can explain that the first one only suggested.

### AI Instruction
If a draft introduces a new analysis after a signal trend, check whether the new analysis is framed as the answer to a specific unresolved interpretation.

## Case PE-REF-2024-003: Heterogeneity Paragraph Ends by Upgrading Metric Value

### Source
Szawełło et al., "Quantifying Dissolution Dynamics in Porous Media Using a Spatial Flow Focusing Profile" / Section 4.3, Impact of Heterogeneity / final paragraph.

### Case Type
PE-END.

### Paragraph Function
conclude.

### Target Skill Problem
weak ending; ending stops at observation; mini-implication missing.

### Tags
- paragraph_function: conclude
- problem_type: weak_ending
- section: Results and Discussion
- stage: Stage 3
- shared_with: narrative_echo / grl_reviewer_philosophy

### Previous Context
The paragraph compares dissolution patterns under different initial heterogeneity levels and shows that high heterogeneity favors channeling-like evolution.

### Target Paragraph
The paragraph first states that similar final structures can arise from different histories. It then argues that the flow focusing profile captures that history and can distinguish regimes even when visual comparison of final patterns fails. The ending raises the broader implication: structures previously labeled as wormholing may actually reflect channeling dynamics.

### Next Context
The Conclusions generalize this point, emphasizing that spatial and temporal information is essential for identifying dissolution regimes.

### Why This Paragraph Works
The ending does not simply repeat the result that heterogeneity matters. It upgrades the paragraph into a claim about interpretive risk: final-shape visual classification can mislead, and time-resolved flow focusing can correct it.

### Sentence-Level Function Map
S1: observation: final structures may appear similar.
S2: method value: the profile captures evolution history.
S3: contrast: visual comparison can miss subtle regime differences.
S4: mini-implication: prior classifications may need reinterpretation.

### Transferable Rule
End a Results paragraph by stating what the observation changes about interpretation, classification, or the next analytical step.

### AI Instruction
If a paragraph ends with a figure observation, ask "So what does this prevent, enable, or revise?" Add one sentence that answers this at the paragraph's functional level.

## Case PE-REF-2025-003: BTC Comparison Ends by Turning Curve Shape Into Diagnostic Inference

### Source
Deng et al., "Anomalous Transport in Dissolving Porous Media: Transitions Between Fickian and Non-Fickian Regimes" / Section 3.1 / final comparison paragraph.

### Case Type
PE-END.

### Paragraph Function
conclude.

### Target Skill Problem
weak ending; comparison without implication; mini-implication missing.

### Tags
- paragraph_function: conclude
- problem_type: weak_ending
- section: Results and Discussion
- stage: Stage 3
- shared_with: mechanism_results / narrative_echo

### Previous Context
The section has compared BTCs from wormholing-induced heterogeneity and an initially random heterogeneous network. Both can produce non-Fickian behavior, but their BTC shapes differ.

### Target Paragraph
The paragraph states that dissolution-induced non-Fickian behavior is fundamentally different from random-heterogeneity non-Fickian behavior. It explains that the plateau or secondary peak appears in wormholing-generated structures but not in randomly assigned pore-size heterogeneity. It then links this difference to modeling strategy and ends by suggesting that BTC characteristics may reveal whether subsurface heterogeneity is preexisting or dissolution-induced.

### Next Context
The next subsection turns from this diagnostic observation to the physical mechanisms that create the transport-regime transitions.

### Why This Paragraph Works
The paragraph does not end at "the curves look different." It converts curve-shape difference into a modeling implication and then into a diagnostic inference about heterogeneity origin.

### Sentence-Level Function Map
S1: comparison claim: two non-Fickian behaviors have different origins.
S2: evidence: plateau/secondary peak appears only in dissolution-induced wormholing.
S3: modeling implication: different upscaling strategies may be needed.
S4: broader interpretation: velocity correlation models may fit dissolution-created structures.
S5: mini-implication: BTC characteristics can help infer heterogeneity origin.

### Transferable Rule
When comparing two similar-looking behaviors, end by naming the practical or interpretive decision that the comparison changes.

### AI Instruction
If a paragraph compares two mechanisms but stops at difference, add a final sentence that states what the difference lets the reader infer or decide.

## Case PE-SELF-001: Tortuosity Details Are Compressed Into Hydraulic Validation

### Source
Current manuscript revision / Section 3.2, Tortuosity Evolution Across Dissolution Regimes / teacher-revised tortuosity opening and comparison paragraphs.

### Case Type
PE-COMPRESS.

### Paragraph Function
validate.

### Target Skill Problem
evidence overload; detail repositioning; secondary metric treated as an independent result.

### Tags
- paragraph_function: validate
- problem_type: evidence_overload / secondary_metric_positioning
- section: Results and Discussion
- stage: Stage 3 / Stage 4
- shared_with: mechanism_results / sentence_hierarchy

### Previous Context
Section 3.1 has already interpreted regime-specific T2 evolution as matrix-vug coupling and flow-path reorganization. The next metric should test that interpretation, not open a separate tortuosity story.

### Target Paragraph
The unrevised version spent substantial space on tortuosity anomalies, segment-wise maxima, and late-stage deceleration. The revised version first assigns tortuosity a validation function: it is an independent hydraulic reference for testing whether T2-derived spectral evolution reflects flow-path optimization. It keeps the global trend, the key timing contrast among regimes, and the breakthrough values, while moving detailed segment-wise evolution for non-central modes to Supporting Information.

### Next Context
The following paragraphs use porosity-permeability evolution and MVC to explain why similar tortuosity values can still produce different breakthrough timing.

### Why This Paragraph Works
The revision does not delete technical correctness for style. It changes the paragraph's function: tortuosity becomes supporting evidence for the NMR interpretation. Details that are correct but low-function are compressed or redirected so the main paragraph remains easy and pleasant to read.

### Sentence-Level Function Map
S1: assigns tortuosity the role of independent hydraulic validation.
S2: gives the global decreasing trend and physical meaning.
S3: highlights the face-dissolution exception only as needed for the mechanism.
S4: compares channeling and wormholing through timing and breakthrough values.
S5: returns to the validation claim: transient T2 evolution reflects hydraulically connected pathway reorganization.

### Transferable Rule
When a paragraph introduces a secondary metric, keep only the details that validate the central mechanism and move detailed metric behavior to SI or a later support paragraph.

### AI Instruction
If a draft paragraph is technically accurate but overloaded, identify its one function first. Keep details that serve that function, compress repeated numerical evidence, and move side analyses that belong to Supporting Information.

## Case PE-SELF-002: Channeling Paragraph Maps Conduit Growth to T2 Merging and Breakthrough

### Source
Current manuscript / Section 3.1, T2 evolution of channeling regime.

### Case Type
PE-MECH.

### Paragraph Function
interpret.

### Target Skill Problem
observation-to-mechanism; signal feature jumps to breakthrough; mechanism buried.

### Tags
- paragraph_function: interpret
- problem_type: mechanism_buried
- section: Results and Discussion
- stage: Stage 3
- shared_with: mechanism_results / narrative_echo

### Previous Context
The preceding paragraphs have established face dissolution as persistent peak separation and wormholing as broad peak overlap. Channeling must be distinguished from both using a transient T2 pathway.

### Target Paragraph
The paragraph begins by positioning channeling as intermediate between face dissolution and wormholing. It then traces the mechanism sequence: an early principal channel penetrates the system, flow focuses into that pathway, velocity contrast with the matrix creates transient T2 bimodality, the principal pathway expands along its full length, diffusive exchange across both flanks strengthens, pore coupling increases, the spectrum merges toward the long-relaxation peak, and breakthrough occurs shortly after the displayed 50% stage.

### Next Context
The next synthesis paragraph compares all three regimes as distinct matrix-vug exchange pathways before the paper moves to tortuosity validation.

### Why This Paragraph Works
The paragraph does not treat transient bimodality as a label. It explains what physical state the transient signal sits between and why rapid peak merging corresponds to efficient conduit formation with limited matrix dissolution.

### Sentence-Level Function Map
S1: comparison topic: channeling is intermediate between face dissolution and wormholing.
S2: structural observation: a principal channel penetrates early.
S3: signal observation: flow focusing and velocity contrast create transient T2 bimodality.
S4: mechanism: full-length channel enlargement alters the flow field.
S5: coupling explanation: diffusive exchange on both flanks strengthens pore coupling.
S6: evidence: vug fraction, matrix fraction, and peak center changes quantify the shift.
S7: mini-implication: transient bimodality followed by merging explains early breakthrough.

### Transferable Rule
For a transient signal paragraph, define the physical transition that the signal marks and connect that transition to the hydraulic outcome.

### AI Instruction
If a draft says a signal is "transient," force it to answer: transient between which two physical states, what mechanism changes the signal, and why that matters for breakthrough or regime distinction.

## Case PE-SELF-003: MVC Paragraph Turns Metric Timing Into Breakthrough Mechanism

### Source
Current manuscript / Section 3.3, MVC interpretation paragraph.

### Case Type
PE-END.

### Paragraph Function
conclude.

### Target Skill Problem
weak ending; metric trend stops at values; mini-implication missing.

### Tags
- paragraph_function: conclude
- problem_type: weak_ending
- section: Results and Discussion
- stage: Stage 3 / Stage 4
- shared_with: mechanism_results / narrative_echo

### Previous Context
The subsection first shows that porosity-permeability curves capture a macroscopic breakthrough hierarchy, then introduces MVC to quantify matrix-vug coupling from the T2 signal.

### Target Paragraph
The paragraph compares the timing and strength of MVC peaks across regimes. Channeling reaches its MVC maximum at lower porosity, reflecting early establishment of a primary conduit and strong exchange. Wormholing peaks later because competing paths must coalesce before global coupling forms. Face dissolution remains subdued and eventually loses apparent exchange as matrix signal decays. The ending turns these trends into the main mechanism: early establishment and synchronous enlargement of a solitary dominant channel control breakthrough efficiency, and MVC distinguishes channeling from wormholing even when their geometries appear similar.

### Next Context
The Implications section generalizes the result: transient NMR T2 evolution and MVC provide diagnostic signatures for dissolution-driven pore coupling and permeability breakthrough.

### Why This Paragraph Works
The paragraph does not end by restating MVC values. It converts metric timing into a mechanism conclusion and a diagnostic payoff for the whole paper.

### Sentence-Level Function Map
S1: topic: MVC peak timing indicates maximum matrix-vug pore coupling.
S2: channeling evidence: early MVC maximum reflects early conduit establishment.
S3: wormholing contrast: delayed MVC peak reflects competition and coalescence.
S4: face-dissolution contrast: subdued MVC reflects weak exchange and near-complete dissolution need.
S5: mini-implication: early synchronous conduit enlargement controls breakthrough efficiency.
S6: paper-level payoff: MVC distinguishes geometrically similar regimes by coupling sequence and breakthrough timing.

### Transferable Rule
When a metric is introduced to resolve a mechanism contrast, the paragraph should end by naming the contrast it resolves, not merely by reporting the metric trend.

### AI Instruction
If a draft's metric paragraph ends with values, add a final sentence that explains what those values reveal about the central mechanism or diagnostic distinction.
