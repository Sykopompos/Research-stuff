**Autism Spectrum: A Signal Processing Architecture**

**Excitatory/Inhibitory Balance, Predictive Coding, and the Consequences of Heightened Bottom-Up Signal Propagation**

*Cortical E/I Balance as the Neural Foundation • Predictive Coding and Prior Weighting • Sensory Profile from TRN Gating and Bottom-Up Amplification • Social Cognition as Different Prior Architecture • Monotropism and Deep Attention • Alexithymia and Interoceptive Prediction • ADHD-Autism Intersection*

M. Finnegan --- v0.1 --- March 2026 --- Preprint, not yet peer reviewed

  **Simulation Design Notice** --- *This paper is one component of a series applying a biological detection architecture framework to neurodevelopmental conditions, part of an ongoing project to build a biologically-grounded computational brain and body simulation. This document combines established literature findings, literature-based inferences, and explicit simulation-level modeling assumptions. Where claims are speculative or emerging, this is noted inline. Nothing in this paper constitutes medical advice, diagnosis, or treatment recommendation.*

  ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  ***Dependency notice:** This paper is one component of a larger reference stack. The five-operation framework (FQ1--FQ5) is developed in the companion documents BrainBody Unified Reference v1.3 and NeurochemFormula Correspondence v1.6, which exist in the same repository. Unlike other papers in this series, this paper does not import neurochemical parameter mappings from those documents. The mechanistic claims here are grounded in the published E/I balance and predictive coding literature directly. Published citations are provided for all empirical claims.*

**Abstract**

Autism Spectrum Disorder (ASD) is a neurodevelopmental profile affecting approximately 1--2% of the population worldwide \[Baxter15; Maenner23\]. Its core characteristics --- differences in sensory processing, social communication, and patterns of attention and interest --- span a wide range of expression across individuals. This paper applies a five-operation detection framework (FQ1--FQ5) to describe the autism profile from the architecture itself: what it propagates, what it filters, what it detects, and how those characteristics interact with environments calibrated for a different signal processing configuration.

The central proposed mechanism is an altered excitatory/inhibitory (E/I) balance in cortical circuits: a relative reduction in GABAergic inhibition and increase in glutamatergic excitation that reduces the effectiveness of top-down predictive dampening relative to bottom-up sensory propagation \[Nelson15; Hollestein23; Noel23\]. On the predictive coding account, the brain continuously generates predictions about incoming sensory signals and propagates only the prediction error forward. When top-down inhibitory precision is reduced, prediction errors propagate more fully --- the sensory world is experienced with less pre-filtering by prior expectation. Sensory experiences are more vivid, more detailed, and more variable. Social signals, which are highly contextual and require strong priors to interpret, carry more uncertainty. Familiar patterns and environments produce stronger stabilizing effects, because consistent sensory predictions are rare and therefore more salient when they occur.

The sensory profile, social cognition differences, preference for predictable environments, deep attentional focus in matched domains, and interoceptive differences associated with alexithymia are each consistent with the same underlying account. This paper describes each in turn, maps them to the FQ1--FQ5 framework, and treats the implications for intervention as following from the architecture.

**§1 --- The Architecture: E/I Balance and the Predictive Processing Profile**

The autism cognitive profile is organized here around a single architectural difference: altered balance between excitatory and inhibitory signaling in cortical circuits, and the downstream consequences of that difference for how sensory information propagates and how predictions are weighted.

Cortical computation involves a continuous interplay between excitatory (glutamatergic) pyramidal neurons and inhibitory (GABAergic) interneurons. The ratio of excitatory to inhibitory activity --- the E/I ratio --- sets fundamental parameters of how cortical circuits process and transmit signals. A higher E/I ratio produces more sensitive, less filtered cortical responses; a lower ratio produces more dampened, more prediction-dominated responses \[Nelson15\].

In autism, multiple lines of evidence converge on an elevated E/I ratio in sensory and prefrontal cortical circuits. Magnetic resonance spectroscopy (MRS) studies document reduced GABA concentrations in visual, auditory, and somatosensory cortices \[Brix15\]. Genetic studies identify enriched mutations in glutamate and GABA signaling genes --- SHANK3, GRIN2A, GABRB3 --- that affect synaptic scaffolding and shift the E/I ratio \[Hollestein23\]. EEG-derived functional E/I ratio measures show elevated excitation-dominated dynamics in ASD relative to neurotypical controls \[Donoghue20\]. The E/I imbalance is not uniform across the autism spectrum: it shows regional, developmental, and individual variation consistent with the heterogeneity of the profile \[Colomar23\].

  **The E/I ratio in autism:** Available evidence associates the autism profile with an elevated E/I ratio in sensory and prefrontal cortical circuits --- increased glutamatergic excitation relative to GABAergic inhibition. This produces more sensitive cortical responses: stimuli are represented with less top-down dampening, less pre-filtering by prior expectation, and more propagation of prediction error. The precise characterization of this difference and its relationship to behavioral features varies across studies and individuals \[Hollestein23; Nelson15; Colomar23\].

**1.1 The Five-Operation Framework Applied Here**

This paper uses a five-operation decomposition framework (FQ1--FQ5) to map the autism profile onto a consistent analytical structure. The five operations are: FQ1 Propagation (what signals transmit and how); FQ2 Gating (what controls passage and threshold); FQ3 Detection (what measures deviation or error); FQ4 Accumulation (what integrates over time and state); and FQ5 Refinement (what updates the structure itself). These operations are applied to the autism profile in §6. The framework is developed in full in the companion documents BrainBody Unified Reference v1.3 and NeurochemFormula Correspondence v1.6. Readers familiar with those documents can treat the FQ labels as cross-references; readers new to the framework can treat them as section headings that organize the mechanistic account without depending on the broader stack.

**1.3 Predictive Coding: What Changes When Top-Down Dampening Is Reduced**

The predictive coding framework proposes that the brain is a prediction machine: it continuously generates top-down predictions about incoming sensory signals, and propagates forward only the difference between the prediction and the actual input --- the prediction error. Higher cortical areas send predictions downward; lower areas send prediction errors upward \[Rao99; Friston05\]. Under this account, perception is the result of combining prior expectations with incoming evidence, weighted by their relative precision.

Top-down predictions are implemented partly through GABAergic inhibitory interneurons at the cortical level: they suppress the baseline firing rate of sensory neurons, such that only prediction errors (deviations from the expected signal) propagate efficiently. When the E/I ratio is elevated and top-down GABAergic dampening is reduced, this prediction mechanism is less effective. Prediction errors propagate more completely. The brain receives a richer, less pre-filtered signal from sensory surfaces.

The hypo-priors model formalizes this \[Pellicano12\]: autistic individuals are proposed to have less informative prior expectations --- or equivalently, to weight incoming sensory evidence more heavily relative to prior predictions. The sensory world is more vivid because fewer signals are suppressed in advance as predicted and therefore unremarkable. The practical consequence is that:

-   **Sensory experiences are more detailed and intense:** features that neurotypical processing would suppress as predicted --- background sounds, textures, lighting variations, predictable environmental patterns --- propagate as full prediction errors rather than being attenuated by top-down expectation.

-   **Unexpected changes are more salient:** when the environment deviates from its recent pattern, the prediction error signal is not attenuated by a strong prior. Novel or unexpected stimuli produce larger, less dampened prediction error responses.

-   **Familiar and predictable environments have stabilizing value:** when sensory predictions are accurate --- the environment matches the internal model --- prediction errors are minimal and processing load is reduced. On this model, predictable environments produce a qualitatively different processing state compared to unpredictable ones.

-   **Prior updating is slower:** because incoming evidence is weighted heavily and priors weakly, changing well-established internal models requires more accumulated evidence than in high-prior architectures \[Lawson17; Wertheimer24\].

  *Note on heterogeneity: the predictive coding and E/I imbalance accounts are active research frameworks, not settled mechanisms. The direction and magnitude of E/I imbalance varies across studies, cortical regions, and individuals on the spectrum. The hypo-priors model explains many autism features well but does not account for all findings. It is used here as a working model for the signal processing account, explicitly labeled as such.*

**1.4 The Thalamic Sensory Gate**

A second architectural element relevant to the autism sensory profile is the thalamic reticular nucleus (TRN) --- a shell of GABAergic neurons that wraps the thalamic relay nuclei and functions as the master sensory gate for cortical input. TRN neurons are activated by corticothalamic and thalamocortical collaterals; they send inhibitory GABA output back onto thalamic relay neurons, implementing selective attenuation of thalamic transmission to cortex.

The TRN is the neural site where top-down cortical predictions modulate the gain of ascending sensory signals: corticothalamic projections from higher cortical areas adjust TRN activity, allowing top-down attention and prediction signals to filter what reaches primary cortex. When GABAergic function is reduced at the TRN level --- consistent with the elevated E/I ratio profile --- thalamic relay transmission is less attenuated. More sensory signal reaches cortex, with less pre-filtering \[Sherman13\].

Working model: the autism sensory profile may partly reflect a TRN calibration that passes more sensory input to cortex with less top-down modulation, consistent with the E/I imbalance account. This is a simulation-level inference pending direct measurement of TRN function in autism.

**§2 --- Sensory Processing: The Bottom-Up Signal Profile**

The sensory characteristics of the autism profile are among its most consistently documented features and the most directly addressed by the E/I/predictive coding account. Sensory over-responsivity --- heightened reactions to sounds, textures, lights, tastes, or smells that neurotypical individuals filter as background --- is present in 69--90% of autistic individuals across studies \[Marco11; Green19\]. Sensory under-responsivity and sensory-seeking behavior are also documented, occurring in different modalities in the same individual.

On the predictive coding account, these may reflect expressions of the same reduced top-down dampening applied to different sensory modalities and contexts:

-   **Over-responsivity:** signals that would normally be suppressed as predicted (background noise, predictable touch, ambient light) instead propagate as full prediction errors. The sensory experience is not louder or brighter in an absolute sense --- it is more completely processed, less attenuated by prior expectation.

-   **Under-responsivity:** in modalities where the internal model has established strong priors through repetition, prediction errors may be small even when the objective stimulus is large. This is consistent with the same architecture applied to familiar, highly-practiced sensory patterns.

-   **Sensory-seeking:** when sensory input produces reliable, predictable prediction errors --- a particular texture, a repeated movement, a specific sound --- it may provide a stable, manageable signal in an otherwise unpredictably variable sensory field. On this model, sensory-seeking behavior is a regulatory strategy.

The cross-modal and temporal aspects of sensory processing also show characteristic differences. Multisensory integration --- combining signals from different modalities into a single percept --- relies on prior-weighted causal inference: does this sound and this visual event come from the same source? When prior precision is reduced, multisensory binding is less reliable; signals from different modalities are more often processed as independent rather than integrated \[Noel23\]. This is consistent with documented multisensory integration differences in autism \[Stevenson14\].

**§3 --- Social Cognition: A Different Prior Architecture**

Social signals are the most contextual, variable, and prior-dependent class of signals in the environment. Interpreting a facial expression, a tone of voice, or a social gesture requires integrating the current signal with a rich prior model of the other person's likely states, intentions, and context. When top-down priors are weighted less heavily relative to bottom-up signals, social interpretation carries more uncertainty on this account: the prior architecture that normally reduces social ambiguity is less dominant, and interpretation relies more heavily on incoming evidence.

  **Social cognition on the predictive coding account:** Theory of Mind --- the ability to attribute mental states to others --- is often framed as absent or impaired in autism. An alternative account consistent with the evidence: mentalizing processes are present but operate with different prior precision and speed \[Cook13; Livingston19\]. Social signals require strong, rapidly applied priors to interpret under real-time interaction conditions; reduced prior weighting produces a profile where social interpretation is present but slower, requires more explicit processing, and is more effortful. The difference is in the architecture of prior weighting rather than in the presence or absence of social cognition.

Several documented characteristics are consistent with this account:

-   **Social signal processing is slower and more effortful:** real-time social interaction requires rapid prior-weighted interpretation of continuously updating signals. When prior weighting is reduced, social interpretation requires more explicit, slower processing rather than automatic, prior-driven inference. This is consistent with documented differences in real-time social interaction that are less apparent in offline or explicit social cognition tasks \[Cook13\].

-   **Double empathy:** autistic individuals often report difficulty interpreting neurotypical social signals, and neurotypical individuals often report equivalent difficulty interpreting autistic social signals. This bidirectional finding --- the 'double empathy problem' --- is consistent with two different prior architectures encountering each other's signal style \[Milton12\]. Autistic individuals show social understanding differences with neurotypical partners but can show highly attuned social interaction with other autistic individuals.

-   **Social camouflage:** many autistic individuals --- disproportionately female and ADHD-comorbid presentations --- develop deliberate strategies for social performance that mask their natural interaction style \[Cage19; Hull20\]. This masking is metabolically costly and associated with increased anxiety, burnout, and late diagnosis. Masking behavior is associated with intact social motivation alongside a mismatch between interaction architectures.

-   **Sameness and social routine:** when a social partner's behavior is highly predictable and scripted, social interaction is substantially easier. Predictable social patterns produce accurate predictions and minimal prediction error. Unpredictable or contextually ambiguous social interactions produce high prediction error load.

**§4 --- Restricted Interests, Repetitive Behaviors, and Monotropism**

Restricted interests and repetitive behaviors (RRBs) are one of the two core diagnostic criteria for autism. The predictive coding account provides a mechanistic description of their function.

Monotropism --- the tendency toward deep, highly focused attention in a single domain at a time rather than distributed attention across multiple domains --- describes a characteristic attentional architecture \[Murray05\]. In the predictive coding frame, highly developed expertise in a domain builds strong, precise priors for that domain: the autistic sensory architecture, which produces more vivid prediction errors in general, produces a particularly stable and efficient processing state within deeply familiar domains. Deep engagement in a focused area of interest provides a reliable, manageable prediction environment in a world that otherwise delivers high prediction error load.

-   **Restricted interests as deep priors:** intense, highly developed areas of interest produce a body of domain-specific prior knowledge that allows prediction-driven processing rather than bottom-up error-dominated processing. This is mechanistically coherent with the same architecture that produces sensory over-responsivity in unfamiliar domains: the architecture favors depth over breadth in prior development.

-   **Repetitive behaviors as prediction regulation:** repetitive motor behaviors --- stimming, rocking, hand-flapping --- may produce reliable, self-generated sensory prediction errors. Working model: they may function as a self-regulation mechanism: generating predictable sensory patterns reduces the ambient unpredictable prediction error load. Evidence supports reduced anxiety and arousal during stimming, consistent with a regulatory rather than meaningless function \[Kapp19\].

-   **Resistance to change as prior preservation:** when a well-established environmental routine is disrupted, the prediction errors associated with the disruption are more salient and less attenuated than in high-prior architectures. Insistence on sameness reflects the stabilizing value of accurate predictions in a system where accurate predictions are harder to achieve and more valuable when they exist.

  *Working model: the monotropism account and the predictive coding/E-I balance account are consistent and mutually supportive, but the direct mechanistic link between them --- specifically the prediction that monotropic attention depth correlates with E/I ratio measures --- has not been directly tested. Both are treated here as simulation-level inferences with strong descriptive support.*

**§5 --- Alexithymia and Interoceptive Differences**

Alexithymia --- difficulty identifying and describing one's own emotional states --- is present in approximately 40--65% of autistic individuals, substantially above the general population rate of approximately 10% \[Bird13; Kinnaird19\]. It is not a feature of autism per se but a co-occurring profile with its own mechanistic account.

The interoceptive prediction account of alexithymia proposes that emotional awareness requires the anterior insula to generate accurate top-down predictions of internal body states, with the posterior insula forwarding only prediction errors from visceral afferents. When these interoceptive predictions are imprecise --- either because the internal body state model is poorly calibrated or because bottom-up interoceptive signals are processed with the same reduced top-down dampening as external sensory signals --- the resulting body state representations are ambiguous and difficult to label \[Seth16; Quattrocki14\].

In the autism profile, both pathways are plausible contributors:

-   **Reduced top-down dampening of interoceptive signals:** the same E/I imbalance that reduces external sensory filtering may reduce internal sensory filtering. Interoceptive signals from the viscera may propagate with less top-down prediction, producing more diffuse, less clearly labeled body state representations.

-   **Less developed interoceptive prior model:** reduced accumulation of interoceptive learning experiences in typical developmental contexts may result in a less refined anterior insula prediction model for body states associated with specific emotional contexts. This is a working model inference without direct empirical test.

The clinical consequence: autistic individuals with alexithymia may have difficulty both identifying and communicating emotional states --- the emotional response may be intact or elevated while the labeling pathway is less reliable. This distinction matters for therapeutic approaches that rely on emotional self-report as the primary data channel \[Kinnaird19\].

**§6 --- FQ1--FQ5 Decomposition of the Autism Profile**

  ---------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Operation**          **Autism Profile Instantiation**

  **FQ1 PROPAGATION**    Sensory signal propagation: thalamic relay → TRN GABA filter → primary cortex. In the autism profile, ascending sensory signals propagate with less top-down attenuation: TRN GABAergic gating may be less effective, and cortical prediction-error propagation is less dampened by descending predictions. The result is more complete propagation of prediction errors --- sensory signals arrive at cortex with less top-down pre-filtering \[Nelson15\]. This is consistent with documented sensory over-responsivity and the vividness of sensory experience reported by autistic individuals. Glutamate-mediated excitation is the primary propagation driver; GABA-mediated inhibition is the primary dampening mechanism that is proposed to be relatively reduced.

  **FQ2 GATING**         The primary gate is the cortical prediction mechanism: descending GABAergic predictions suppress the baseline firing of sensory neurons, such that only prediction errors propagate upward \[Rao99; Friston05\]. In the autism profile, this gate is less dominant: elevated E/I ratio reduces the effectiveness of predictive suppression. More prediction error propagates through the gate, producing more vivid sensory experience and greater sensitivity to environmental change. Thalamic TRN gating provides a second gate: GABA from TRN onto relay nuclei attenuates ascending thalamic signal. Reduced GABAergic tone at TRN may pass more signal to cortex. Working model: both gates operate at a higher effective threshold in the autism profile, consistent with the E/I imbalance account.

  **FQ3 DETECTION**      Prediction error detection is more sensitive: signals that neurotypical processing attenuates as predicted instead register as detectable prediction errors. This produces heightened detection of environmental change, sensory detail, pattern deviations, and inconsistencies. In social cognition, this manifests as detection of non-obvious details, inconsistencies in social presentation, and logical contradictions that high-prior social processing would typically smooth over. In special interest domains, highly developed priors produce efficient detection of domain-specific deviations and novelty. FQ3 detection operates at a different signal class and sensitivity calibration than the neurotypical mode \[Noel23\].

  **FQ4 ACCUMULATION**   Prediction error accumulation in high-load environments: when the sensory environment produces continuous unpredicted signals, prediction errors accumulate faster than the system can incorporate them into updated models. On this model, sensory overload reflects accumulation of prediction errors that exceeds the system's update capacity. Autistic burnout and the additional load from social camouflage are consistent with this accumulation account \[Raymaker20\], though the direct link between prediction error load and burnout phenomenology has not been empirically tested in this framework.

  **FQ5 REFINEMENT**     Prior updating is slower when incoming evidence conflicts with established internal models \[Lawson17\]. This has two expressions: (1) resistance to changing well-established routines and expectations (the prior is strong and updating requires more evidence), and (2) slower adaptation to novel environments even when intellectually understood. Conversely, within domains where strong priors have been developed through deep interest, FQ5 refinement is highly efficient: the autistic architecture builds detailed, precise prior models within focused domains. Environmental accommodation and predictable structure accelerate FQ5 adaptation by reducing the prediction error load during prior-updating phases.
  ---------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**§7 --- Natural History and Lifespan Trajectory**

Autism is a lifelong profile, not a developmental condition that resolves. The characteristics described here are architectural: they reflect a different configuration of the signal processing system.

Trajectory is heavily influenced by environmental fit and accumulated prior development:

-   **Early childhood:** sensory environments and social demands in early childhood settings (nursery, school) are calibrated for neurotypical sensory processing and social prior architectures. For autistic children, these environments produce high prediction error load across sensory, social, and cognitive domains simultaneously. Early identification and environmental accommodation substantially affect long-term trajectory \[Zwaigenbaum15\].

-   **Language development:** approximately 25--30% of autistic individuals are minimally verbal or non-speaking, reflecting variability in how the autism profile interacts with language acquisition circuits. Many minimally verbal autistic individuals have strong comprehension and communicate effectively via augmentative means; speech production and language comprehension are dissociable \[Mirenda08\].

-   **Adolescence:** social complexity increases substantially in adolescence, as neurotypical social conventions become more implicit, contextual, and rapidly-updated. The processing demands of social camouflage often increase. Anxiety and depression comorbidities are elevated during this period, associated with cumulative masking load and social mismatch rather than directly with the autism profile \[Lai20\].

-   **Adulthood:** autistic adults in environments that match their profile --- with predictable structure, clear communication, sensory accommodation, and domains aligned with focused interests --- report substantially better quality of life than those in chronically mismatched environments \[Mason19\]. Environmental self-selection in adulthood is a major determinant of functional outcome.

-   **Late diagnosis:** adults receiving autism diagnoses after years of misidentification (often as anxiety, depression, ADHD, or personality differences) report a characteristic reorientation to prior experiences. Masking behaviors that were automatically applied without a framework now have a mechanistic account. The diagnosis does not change the profile; it changes the conceptual frame for understanding it \[Bargiela16\].

**§8 --- Co-occurring Profiles**

Autism co-occurs with other neurodevelopmental and psychiatric conditions at rates substantially above chance \[Lai19\]:

-   **ADHD:** the most common co-occurring neurodevelopmental profile, present in approximately 50--70% of autistic individuals \[Lichtenstein10; Lai19\]. The autism profile and ADHD operating point are mechanistically distinct but functionally compound: the autism sensory architecture produces high ambient prediction error load, and the ADHD reduced WM gate stability produces difficulty managing that load under sustained task demands. The compound profile is often misidentified as one or the other condition, because the combined presentation looks different from either in isolation. See ADHD paper for the operating point account.

-   **Anxiety:** highly prevalent, present in 40--80% of autistic individuals \[van Steensel11\]. Elevated prediction error load is itself anxiogenic: sustained uncertainty about sensory and social prediction increases limbic activation. Social camouflage adds metabolic and cognitive load. Anxiety in autism is associated with the profile-environment mismatch rather than directly with the autism architecture, though they interact \[Kerns14\].

-   **Depression:** elevated, particularly in adolescent and adult autistic individuals. Associated with accumulated masking load, chronic mismatch between self and environment, and secondary effects of misidentification and misunderstanding. The LHb→VTA→DA_tonic mechanism described in the Depression paper produces a motivation floor reduction on top of whatever baseline the autism profile carries.

-   **Epilepsy:** co-occurs in 6--27% of autistic individuals \[Lukmanji19\], substantially above population rates. The elevated E/I ratio that characterizes the autism profile is the same mechanism that, when sufficiently extreme, lowers the seizure threshold. Epilepsy comorbidity is consistent with elevated cortical excitability in at least a significant subset of the autism population, though co-occurrence data alone does not establish the mechanistic link directly.

-   **Sensory processing disorder:** sensory over- and under-responsivity are described here as expressions of the same E/I/predictive coding architecture rather than as separately categorized comorbidities.

-   **Tourette syndrome and tic disorders:** elevated co-occurrence, with shared genetic architecture involving synaptic signaling genes. The CSTC gate failure in Tourette's (described in the Tourette's paper) and the cortical E/I imbalance in autism are distinct mechanisms but co-occur at rates above chance, suggesting shared genetic vulnerability at the synaptic scaffolding level.

**§9 --- Intervention Analysis**

No pharmacological intervention addresses the core autism profile. Available medications target co-occurring conditions (anxiety, depression, ADHD, epilepsy, sleep disruption) rather than the signal processing architecture itself. The intervention landscape for autism is predominantly behavioral, educational, and environmental. The framework presented here is intended to organize the mechanistic logic of interventions, not to claim that existing clinical practice has been validated by the model.

  ------------------------------------------------------- --------------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Treatment / Intervention**                            **Target**                                                      **Mechanism**                                                                                                                                                                                                                                                                                                                                                                                                                                                                    **Evidence and Notes**

  Occupational therapy (sensory integration)              FQ1--FQ2 (sensory gate calibration)                             Sensory integration therapy (SIT) exposes the individual to controlled sensory inputs in a graduated, predictable framework, building prior models for specific sensory experiences. On the predictive coding account, SIT builds sensory priors: the sensory experience becomes predictable and therefore less alarming. Environmental sensory modification (noise reduction, lighting adjustment, texture accommodation) reduces the ambient prediction error load directly.   Evidence for SIT in autism is mixed; systematic reviews show modest effects on sensory responsivity and functional outcomes \[Schaaf18\]. Environmental modification is lower-cost and broadly recommended as a first-line accommodation. Individualized sensory profiles guide specific modifications.

  Speech and language therapy (SLT)                       FQ1--FQ3 (communication signal architecture)                    SLT for autism addresses the specific communication differences of the profile. For minimally verbal or non-speaking autistic individuals, augmentative and alternative communication (AAC) provides a channel for communication that bypasses the speech production system. For verbal autistic individuals, SLT addresses pragmatics, prosody, and contextual communication signal interpretation.                                                                             Evidence-supported for improving functional communication \[Kasari14\]. AAC is particularly well-evidenced: there is no evidence that AAC delays speech development, and strong evidence it improves functional communication for non-speaking autistic individuals. Early initiation is associated with better outcomes.

  Applied Behavior Analysis (ABA)                         FQ5 (behavioral repertoire training)                            ABA and its contemporary NDBI variants use reinforcement-based learning to build behavioral repertoires in child-led, play-based formats aligned with the child's interests and predictable structures.                                                                                                                                                                                                                                                                          Behavioral interventions for autism have the largest evidence base of any approach; NDBI formats show strong outcomes for functional communication and daily living skills \[Weitlauf14\]. Lovaas87 is the foundational trial but represents an earlier discrete-trial format; contemporary practice has shifted substantially toward NDBI approaches.

  Predictable structure and environmental accommodation   FQ2--FQ4 (prediction error load reduction)                      Structured environments with predictable routines reduce ambient prediction error load. Visual schedules, advance notice of transitions, and consistent physical environments allow prediction-driven processing rather than error-driven processing. This is an intervention that affects the operating state of the system directly.                                                                                                                                           Low-cost, widely applicable, consistently reported as effective by autistic individuals and their families. The evidence base is largely observational, but the mechanistic rationale is strong \[Mesibov10\]. Evidence and clinical guidance support environmental accommodation as a concurrent component of behavioral intervention rather than a later addition.

  Pharmacological (for co-occurring conditions)           FQ2 (anxiety/ADHD gate effects); FQ3--FQ4 (seizure threshold)   Medications targeting ADHD (stimulants, guanfacine, viloxazine) are used for co-occurring ADHD operating point effects; see ADHD paper. SSRIs for anxiety and depression; anti-epileptics for seizure management. Risperidone and aripiprazole are FDA-approved for irritability associated with autism but address behavioral dysregulation as an outcome, not the signal processing architecture.                                                                              No medication addresses core autism characteristics. Medications for co-occurring conditions follow their own evidence bases. Risperidone/aripiprazole: FDA-approved for autism-associated irritability \[McCracken02\] but with significant metabolic side effects; guidelines support time-limited, targeted use for specific dysregulation presentations rather than as general autism treatment.
  ------------------------------------------------------- --------------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**§10 --- Connections Across the Framework**

-   **ADHD:** the compound autism-ADHD profile is common and clinically distinct from either in isolation. The autism profile produces high ambient prediction error load; ADHD reduces the WM gate available to manage that load. The combined profile often produces greater functional consequence than either alone, and misidentification in both directions is frequent. The double masking problem --- autism masking and ADHD compensation both simultaneously active --- substantially increases the cognitive cost of functioning in mismatched environments.

-   **Epilepsy:** the E/I imbalance account is consistent with the elevated seizure risk: both reflect elevated cortical excitability, though the co-occurrence data does not establish the shared mechanism directly.

-   **Depression:** cumulative masking load, chronic profile-environment mismatch, and misidentification across developmental years produce the accumulated conditions described in the Depression paper's mismatch-driven depression account. The LHb→VTA mechanism further reduces tonic DA and motivation on top of the autism architecture.

-   **Tourette's:** shared genetic vulnerability at the level of synaptic scaffolding genes produces co-occurrence above chance. The CSTC gate failure in Tourette's and the cortical E/I profile in autism are distinct mechanisms but may share upstream genetic determinants at the synaptic protein level \[Robertson00\].

-   **Gifted Detection and 2e:** working model: the autism profile and high-capacity structural pattern recognition may interact in 2e configurations in ways consistent with the Gifted paper account. This is a simulation-level inference; no direct test of this combination exists.

**§11 --- Conclusion**

Autism is characterized here as a signal processing architecture with an altered excitatory/inhibitory balance in cortical circuits, producing reduced effectiveness of top-down predictive dampening and more complete propagation of bottom-up prediction errors. The sensory profile, social cognition differences, and preference for predictable environments are most directly consistent with the E/I/predictive coding account. The extensions to monotropism, alexithymia, and burnout are more loosely connected and treated here as simulation-level inferences. Direct tests of the unified mechanism across these domains remain limited.

The architecture processes signals differently from the neurotypical mode: more vividly, with less pre-filtering by expectation, with stronger emphasis on incoming evidence relative to prior predictions. These characteristics produce advantages in domains that reward detailed observation, pattern detection within familiar systems, and deep prior development. They produce friction in environments calibrated for the neurotypical predictive architecture.

No pharmacological intervention currently addresses the core profile. Effective intervention focuses on reducing prediction error load through environmental accommodation, building domain-specific priors through structured learning, providing alternative communication channels where speech production is affected, and identifying and accommodating the co-occurring ADHD, anxiety, and depression profiles that compound the functional consequences. Environmental match \-\-- finding or constructing contexts where the autism signal processing architecture produces functional advantages rather than chronic friction \-\-- is associated with substantially better quality of life outcomes \[Mason19\].

  *The distinction between the architecture and the environments it is placed in matters clinically. The autism profile produces different functional outcomes in matched versus mismatched environments. This is a difference in fit, not in the architecture.*

**References**

\[Baxter15\] A.J. Baxter et al., The epidemiology and global burden of autism spectrum disorders, Psychol Med 45 (2015) 601--613. \[Global ASD prevalence; epidemiology; burden estimates\]

\[Maenner23\] M.J. Maenner et al., Prevalence and characteristics of autism spectrum disorder among children aged 8 years --- Autism and Developmental Disabilities Monitoring Network, MMWR Surveill Summ 72 (2023). \[US prevalence estimate 1 in 36; demographic patterns\]

\[Nelson15\] S.B. Nelson & V. Valakh, Excitatory/inhibitory balance and circuit homeostasis in autism spectrum disorders, Neuron 87 (2015) 684--698. \[E/I imbalance in ASD; GABA deficit; glutamate excess; genetic mechanisms; homeostatic plasticity\]

\[Hollestein23\] V. Hollestein et al., Excitatory/inhibitory imbalance in autism: the role of glutamate and GABA gene-sets in symptoms and cortical brain structure, Transl Psychiatry 13 (2023) 18. \[GABA/glutamate gene-set analysis; cortical thickness; E/I and autism symptoms; AIMS-2-TRIALS LEAP cohort\]

\[Noel23\] J.P. Noel & D.E. Angelaki, A theory of autism bridging across levels of description, Trends Cogn Sci 27 (2023) 631--641. \[ASD as altered causal inference; divisive normalization; E/I imbalance as neural implementation; predictive coding bridge\]

\[Donoghue20\] T. Donoghue et al., Measurement of excitation-inhibition ratio in autism spectrum disorder using critical brain dynamics, Sci Rep 10 (2020). \[Functional E/I ratio from EEG; elevated excitation-dominated dynamics in ASD; validation in autism and healthy controls\]

\[Colomar23\] L. Colomar et al., Role of cortical excitatory/inhibitory imbalance in autism spectrum disorders from a symptom severity trajectories framework, BMC Psychiatry 23 (2023) 213. \[E/I imbalance protocol; longitudinal design; regional and individual variability\]

\[Rao99\] R.P. Rao & D.H. Ballard, Predictive coding in the visual cortex: a functional interpretation of some extra-classical receptive-field effects, Nat Neurosci 2 (1999) 79--87. \[Canonical predictive coding account; layer 2/3 top-down predictions; layer 4 bottom-up; prediction error propagation\]

\[Friston05\] K. Friston, A theory of cortical responses, Philos Trans R Soc Lond B Biol Sci 360 (2005) 815--836. \[Predictive coding as free energy minimization; precision-weighted prediction errors; cortical hierarchy\]

\[Pellicano12\] E. Pellicano & D. Burr, When the world becomes 'too real': a Bayesian explanation of autistic perception, Trends Cogn Sci 16 (2012) 504--510. \[Hypo-priors model; reduced Bayesian priors in autism; sensory over-responsivity from attenuated top-down prediction\]

\[Lawson17\] R.P. Lawson et al., Adults with autism overestimate the volatility of the sensory environment, Nat Neurosci 20 (2017) 1293--1299. \[Slower prior updating in autism; overestimation of environmental volatility; Bayesian learning rate\]

\[Wertheimer24\] O. Wertheimer & Y. Hart, Autism spectrum disorder variation as a computational trade-off via dynamic range of neuronal population responses, Nat Neurosci 27 (2024) 2476--2486. \[Dynamic range model; hypo-priors; slow updating; computational trade-off account; ASD heterogeneity\]

\[Brix15\] M.K. Brix et al., Brain MR spectroscopy in autism spectrum disorder --- the GABA excitatory/inhibitory imbalance theory revisited, Front Hum Neurosci 9 (2015) 365. \[MRS GABA concentrations in visual, auditory, somatosensory cortex; ASD vs controls\]

\[Sherman13\] S.M. Sherman & R.W. Guillery, Functional Connections of Cortical Areas: A New View from the Thalamus, MIT Press (2013). \[Thalamic relay architecture; TRN as sensory gate; corticothalamic top-down modulation; predictive coding implementation in thalamus\]

\[Marco11\] E.J. Marco et al., Sensory processing in autism: a review of neurophysiologic findings, Pediatr Res 69 (2011) 48R--54R. \[Sensory over- and under-responsivity prevalence in autism; neurophysiological correlates\]

\[Green19\] S.A. Green et al., Sensory over-responsivity: the relationship between sensory processing and internalizing symptoms in autism spectrum disorders, J Abnorm Child Psychol 47 (2019) 683--693. \[Sensory over-responsivity prevalence; association with anxiety; sensory-emotional bidirectionality\]

\[Stevenson14\] R.A. Stevenson et al., Multisensory temporal integration in autism spectrum disorders, J Neurosci 34 (2014) 691--697. \[Multisensory binding differences; widened temporal binding window; causal inference in autism\]

\[Cook13\] R. Cook et al., Alexithymia, not autism, predicts poor recognition of emotional facial expressions, Psychol Sci 24 (2013) 723--732. \[Alexithymia as mediator of social cognition differences; separating autism and alexithymia effects\]

\[Livingston19\] L.A. Livingston et al., Compensatory strategies below the behavioural surface in autism: a qualitative study, Lancet Psychiatry 6 (2019) 766--777. \[Compensatory/camouflage strategies in autism; social cognition processes present but effortful; masking mechanisms\]

\[Milton12\] D.E.M. Milton, On the ontological status of autism: the 'double empathy problem', Disabil Soc 27 (2012) 883--887. \[Double empathy problem; bidirectional social signal mismatch; social cognition reframe away from deficit\]

\[Cage19\] E. Cage & Z. Troxell-Whitman, Understanding the reasons, contexts and costs of camouflaging for autistic adults, J Autism Dev Disord 49 (2019) 1899--1911. \[Masking/camouflage in autism; costs; contexts; relationship to late diagnosis\]

\[Hull20\] L. Hull et al., The role of camouflaging in the identification of autistic adults, J Autism Dev Disord 50 (2020) 2852--2864. \[Camouflage measurement; sex differences in masking; impact on diagnosis and wellbeing\]

\[Murray05\] D. Murray et al., Attention, monotropism and the diagnostic criteria for autism, Autism 9 (2005) 139--156. \[Monotropism account of autism; attention tunnel; interest-based motivation; alternative to deficit framing\]

\[Kapp19\] S.K. Kapp et al., 'Stimming' and the social functions of self-stimulatory behavior in autism, Autism 23 (2019) 1931--1941. \[Self-stimulatory behavior as regulatory function; reduced anxiety during stimming; reframing stimming\]

\[Bird13\] G. Bird & C. Cook, Mixed emotions: the contribution of alexithymia to the emotional symptoms of autism, Transl Psychiatry 3 (2013) e285. \[Alexithymia prevalence in autism (\~40--65%); dissociation from social cognition differences; measurement issues\]

\[Kinnaird19\] E. Kinnaird et al., Investigating alexithymia in autism: a systematic review and meta-analysis, Eur Psychiatry 55 (2019) 80--89. \[Meta-analysis alexithymia in ASD; prevalence; relationship to anxiety and other outcomes\]

\[Seth16\] A.K. Seth & K.J. Friston, Active interoceptive inference and the emotional brain, Philos Trans R Soc Lond B Biol Sci 371 (2016) 20160007. \[Predictive interoception; aInsula prediction vs pInsula error; alexithymia as interoceptive model failure\]

\[Quattrocki14\] E. Quattrocki & K. Friston, Autism, oxytocin and interoception, Neurosci Biobehav Rev 47 (2014) 410--430. \[Interoceptive prediction account of autism; oxytocin and social prediction; aInsula-insula model\]

\[Zwaigenbaum15\] L. Zwaigenbaum et al., Early identification of autism spectrum disorder: recommendations for practice and research, Pediatrics 136 Suppl 1 (2015) S10--40. \[Early identification and intervention; trajectory effects; environmental accommodation\]

\[Mirenda08\] P. Mirenda, A back door to literacy? AAC experience and its relationship to autism, Topics Lang Disord 28 (2008) 141--150. \[AAC and autism; relationship to speech development; non-speaking autistic individuals\]

\[Lai20\] M.C. Lai et al., A systematic review of mental health assessment in autistic adolescents and adults, Dev Psychopathol 32 (2020) 1576--1604. \[Mental health in autistic adolescents and adults; anxiety, depression, burnout; masking load\]

\[Mason19\] D. Mason et al., Quality of life for autistic people: a systematic review, Autism Res 12 (2019) 428--441. \[QoL determinants in autism; environmental fit; employment, relationships, accommodation\]

\[Bargiela16\] S. Bargiela et al., The experiences of late-diagnosed women with autism spectrum conditions, J Autism Dev Disord 46 (2016) 3281--3294. \[Late diagnosis experiences; reorientation; impact on self-understanding; female and late-diagnosed autistic adults\]

\[Lai19\] M.C. Lai et al., Prevalence of co-occurring mental health diagnoses in the autism population, Lancet Psychiatry 6 (2019) 819--829. \[Co-occurring conditions; ADHD, anxiety, depression prevalence in autism; systematic review\]

\[Lichtenstein10\] P. Lichtenstein et al., The genetics of autism spectrum disorders and related neuropsychiatric disorders in childhood, Am J Psychiatry 167 (2010) 1357--1363. \[ADHD-autism genetic overlap; shared heritability; co-occurrence rates\]

\[van Steensel11\] F.J. van Steensel et al., Anxiety disorders in children and adolescents with autistic spectrum disorders, Clin Child Fam Psychol Rev 14 (2011) 302--317. \[Anxiety prevalence in autism 40--80%; types; relationship to autism features\]

\[Kerns14\] C.M. Kerns et al., Anxiety in autism spectrum disorder, Curr Psychiatry Rep 16 (2014) 446. \[Anxiety mechanisms in autism; social and sensory contributors; clinical considerations\]

\[Lukmanji19\] S. Lukmanji et al., The co-occurrence of epilepsy and autism: a systematic review, Epilepsy Behav 98 (2019) 238--248. \[Epilepsy prevalence in autism 6--27%; E/I ratio connection; risk factors\]

\[Robertson00\] M.M. Robertson, Tourette syndrome, associated conditions and the complexities of treatment, Brain 123 (2000) 425--462. \[TS comorbidities; shared genetic vulnerability; synaptic scaffolding genes\]

\[Schaaf18\] R.C. Schaaf et al., An intervention for sensory difficulties in children with autism, J Autism Dev Disord 48 (2018) 1493--1506. \[SIT RCT in autism; sensory outcomes; functional goal attainment\]

\[Kasari14\] C. Kasari et al., Communication interventions for minimally verbal children with autism: sequential multiple assignment randomized trial, J Am Acad Child Adolesc Psychiatry 53 (2014) 635--646. \[SLT and AAC in autism; minimally verbal interventions; early communication outcomes\]

\[Lovaas87\] O.I. Lovaas, Behavioral treatment and normal educational and intellectual functioning in young autistic children, J Consult Clin Psychol 55 (1987) 3--9. \[Foundational ABA study; intensive behavioral intervention outcomes\]

\[Weitlauf14\] A.S. Weitlauf et al., Interventions targeting sensory challenges in children with autism spectrum disorder, Pediatrics 134 (2014) e1168--1182. \[Comprehensive review of behavioral interventions; evidence grades; NDBI approaches\]

\[Mesibov10\] G.B. Mesibov & M. Shea, The TEACCH program in the era of evidence-based practice, J Autism Dev Disord 40 (2010) 570--579. \[Structured teaching; visual schedules; environmental predictability; TEACCH outcomes\]

\[McCracken02\] J.T. McCracken et al., Risperidone in children with autism and serious behavioral problems, N Engl J Med 347 (2002) 314--321. \[Risperidone FDA approval for autism-associated irritability; RUPP trial; behavioral outcomes and side effects\]

\[Raymaker20\] D.M. Raymaker et al., 'Having all of your internal resources exhausted beyond measure and being left with no clean-up crew': defining autistic burnout, Autism Adulthood 2 (2020) 132--143. \[Autistic burnout; cumulative masking and prediction error load; definition and characteristics\]

*Autism_Spectrum_v0_1.docx --- Draft --- Unpublished --- Do not distribute*

