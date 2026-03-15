# The Peripheral Nervous System as a Distributed Sensing and Effector Network

*Autonomic, Enteric, and Somatic Divisions: Architecture, Coupling, and Disease Relevance*

**M. Finnegan**

v0.8 — March 2026 — Unpublished draft, not yet peer reviewed

---

> **Article Scope and Companion References:** This paper is an integrative review of the peripheral nervous system organized around three functional divisions: the autonomic nervous system (sympathetic [SNS] and parasympathetic [PSNS]), the enteric nervous system, and the somatic peripheral nervous system (DRG sensory neurons, NMJ, and proprioceptors). Each division is analyzed using a five-operation decomposition (Propagation, Gating, Detection, Accumulation, Refinement) used here as an analytical scaffold rather than a theoretical claim. Brain-interface effects of each division's signals are covered in the companion Brain-Body reference (BrainBody v1.3) and in the relevant brain structure maps. Evidence confidence tiers are specified at the end of §1.

---

## Abstract

The peripheral nervous system (PNS) is conventionally divided into autonomic and somatic subdivisions, with the autonomic further divided into sympathetic and parasympathetic. This organizational scheme captures anatomical origin but understates functional complexity. The autonomic nervous system is not a simple motor relay: recent single-cell transcriptomic profiling of sympathetic ganglia and vagal ganglia has identified organ-specific neuronal subtypes at every level, and 80–90% of vagal fibers are afferent — the brain is primarily receiving from the body rather than commanding it. The enteric nervous system, often omitted from PNS discussions, contains as many neurons as the spinal cord and executes gut motility, secretion, and mucosal defense through local reflex arcs that function autonomously. The somatic PNS — through dorsal root ganglion neurons, the neuromuscular junction, and proprioceptors — provides both the body's surface sensory array and the motor output pathway for voluntary movement.

This paper describes the three-division architecture of the peripheral nervous system, maps the cross-division interactions that help determine integrated function, and identifies the multi-system failure cascades that produce clinical disease. Evidence confidence is tiered throughout; organ-specific neuronal subtype diversity, microbiome-driven ENS modulation, and the proposed clinical cascade patterns are distinguished from established consensus mechanisms. The paper is written as a companion to the Brain-Body Unified Reference and the Endocrine System paper, with upstream CNS effects cited to those documents rather than duplicated here.

---

## §1 — The Peripheral Nervous System as a Three-Division Architecture

The peripheral nervous system comprises all neural tissue outside the brain and spinal cord. Three functional divisions are distinguished here by anatomy, neurotransmitter identity, and computational role.

The autonomic nervous system (ANS) operates below voluntary awareness and regulates the internal environment: heart rate, blood pressure, digestion, glandular secretion, and organ perfusion. Its sympathetic division (SNS) mobilizes resources in response to threat or demand. Its parasympathetic division (PSNS) maintains and restores during low-demand states. These are not simply opposing systems that toggle between states — they co-activate in organ-specific patterns and regulate each other via baroreflex and central command pathways.

The enteric nervous system (ENS) is the largest division of the peripheral nervous system. Embedded in the gut wall from esophagus to rectum, it contains approximately 500 million neurons — rivaling the spinal cord in scale [2] — and can execute complete reflex arcs for peristalsis, secretion, and mucosal defense without spinal cord or brain input. It is also the primary interface between the gut microbiome and the nervous system: microbiome-derived metabolites activate enteroendocrine cells, which signal enteric and vagal neurons through a cascade now understood to operate in milliseconds via direct neuropod cell synapses as well as through minutes-long hormonal diffusion.

The somatic PNS carries sensory signals — both conscious (pain, touch, temperature) and subconscious (proprioception) — to the brain, and voluntary motor commands from the brain to skeletal muscle. Dorsal root ganglion (DRG) neurons are the sensory array: at least 22 molecularly distinct subtypes in the human DRG have been identified, spanning nociception, mechanosensation, thermosensation, and proprioception. Motor output is delivered through the neuromuscular junction (NMJ), a specialized high-reliability synapse with a safety factor of 3–4× normal threshold. Proprioceptors — muscle spindles and Golgi tendon organs — close the motor control loop by reporting muscle length and tension to the spinal cord and cerebellum in real time.

These three divisions share the brainstem NTS as a primary integration hub, are modulated by overlapping descending signals from the same cortical and subcortical structures, and are coupled through the gut-brain axis and the pain-autonomic interface. **Note on terminology:** the three top-level divisions are autonomic, enteric, and somatic; the five analytic components listed below reflect the standard functional subdivisions within those divisions — the autonomic split into SNS and PSNS, the somatic split into sensory (DRG) and motor (NMJ). Understanding PNS function at the system level requires all five components.

**The five components covered here:**

- **Sympathetic (SNS):** IML spinal cord T1–L2 → paravertebral/prevertebral ganglia → NE + NPY → target organs; adrenal medulla as humoral extension
- **Parasympathetic/Vagal (PSNS):** DMV + nucleus ambiguus (brainstem) → terminal ganglia → ACh → target organs; 80–90% of vagal fibers are afferent
- **Enteric (ENS):** myenteric plexus (motility) + submucosal plexus (secretion) + enteroendocrine cells (chemical sensing) + enteric glia
- **Somatic sensory (DRG):** nociceptors, LTMRs, proprioceptors → spinal cord dorsal horn → ascending pathways
- **Somatic motor (NMJ):** alpha motor neuron → NMJ → skeletal muscle; gamma motor neurons → intrafusal fiber contraction → spindle gain control

These five components share relay infrastructure (NTS, parabrachial nucleus, thalamus) and interact through direct coupling mechanisms described in §3.

---

### Evidence Tiers — Scope and Confidence of Claims

> **Note:** These tiers reflect the confidence with which claims are used within this review. They are not a formal evidence-grading system (e.g., GRADE) and should not be read as one. Reviewers may reasonably disagree on individual assignments.

**Tier A — Established consensus (well-replicated, textbook-level):**
Sympathetic NE → α/β adrenergic receptor effects; parasympathetic ACh → muscarinic receptor effects; baroreflex feedback loop (baroreceptors → NTS → RVLM/nAmb); SCN → PVN → sympathetic chain → pineal NE → melatonin synthesis (strict serial pathway); HRV-RMSSD as vagal tone proxy; NMJ ACh quantal transmission; Ia monosynaptic stretch reflex; PIEZO2 required for touch and proprioception (human genetic evidence); EC cell 5-HT requires microbiome spore-forming bacteria; EC cell peripheral 5-HT does not cross the BBB; GLP-1 incretin amplification (50–70% of oral glucose insulin response); gate control (Aβ concurrent activity suppresses C-fiber signal via GABAergic interneuron).

**Tier B — Cross-axis mechanisms with direct experimental support:**
Cholinergic anti-inflammatory pathway: vagal tone → splenic α7 nAChR → TNF-α/IL-1β suppression [human sepsis and rodent]; satellite glia active modulation in sympathetic ganglia [mouse, eLife 2022]; stellate ganglion organ-specific adrenergic subtypes (NA1a/NA1b/NA1c, scRNA-seq) [Ajijola 2020]; nodose ganglion 18–27 molecularly distinct subtypes [scRNA-seq, Kupari 2019]; intestinal mechanoreceptor (IGLE) → direct AgRP neuron inhibition [mouse, Cell 2019]; ENS autonomy (peristalsis continues after vagotomy but is modulated by vagal input); SCFA → GPR41/43 on EEC → GLP-1 and ENS activation; neuropod cell direct EEC→ENS synapse (rapid synaptic-scale transduction [15]); nutrients detected indirectly via epithelium → 5-HT → ENS, not by direct ENS sensing [Nature 2025]; peripheral sensitization (TRPV1 sensitized by PGE2/NGF); central sensitization cascade (BDNF-TrkB-KCC2 after nerve injury); CGRP → neurogenic inflammation + migraine (anti-CGRP antibodies clinically validated); NMJ electrical activity component alongside agrin/MuSK (ETV4, snRNA-seq 2025); alpha-synuclein ENS seeding → retrograde vagal spread toward brainstem (PD gut-first hypothesis); sympathetically maintained pain (SNS sprouting into DRG after injury); HRV biofeedback as trainable vagal tone intervention.

**Tier C — Emerging findings or integrative hypotheses (preprint, single study, or extrapolated from animal models):**
Human DRG reference atlas (22 neuronal subtypes, 2025 preprint — awaiting peer review); PDZRN4 as therapeutic NMJ target [mouse, 2025]; microbial metabolites direct vagal activation via luminal receptors [Jameson 2024, mouse]; topological crypt-villus stress sensor segregation [Touhara 2025]; enteric glia sex differences in motility regulation [mechanism incomplete]; Long COVID dysautonomia mechanism [emerging 2023–2025]; specific probiotic strain → ENS functional recovery; acetate BBB crossing → microglial GPR109A neuroprotection [limited human evidence]; psychobiotics [preclinical predominant; human trials mixed]; the multi-system failure cascade syntheses in §4 are integrative hypotheses — each component mechanism is individually supported, but the cascades as unified clinical patterns are proposed rather than directly measured.

---

## §2 — Detection Architecture of Each Division

Each division is organized below using five operations: **Propagation** (what transmits the signal), **Gating** (what controls passage or threshold), **Detection** (what measures deviation or error), **Accumulation** (what integrates over time or chronic state), and **Refinement** (what updates the structure itself). This decomposition is an analytical scaffold for locating control logic and identifying coupling points; it does not represent a theoretical claim beyond the established biology described. Tier A claims are established consensus; Tier B claims have direct experimental support as noted; Tier C findings are flagged at point of use.

### §2.1 — Sympathetic Nervous System

The SNS is organized as a two-neuron chain: short preganglionic neurons (IML, T1–L2) release ACh → nAChR on postganglionic neurons in paravertebral or prevertebral ganglia → postganglionic neurons release NE at target organs. The adrenal medulla is a modified postganglionic structure receiving direct preganglionic innervation and releasing epinephrine into the bloodstream, providing humoral reach beyond synaptic NE.

**Propagation:** SNS drive originates in the RVLM (rostral ventrolateral medulla), which is tonically active and modulated by baroreceptor feedback, hypothalamic stress signals (PVN CRH), and cortical/limbic descending input. RVLM → IML is the primary sympathetic motor pathway [4]. Postganglionic neurons are unmyelinated C-fibers (~0.5–2 m/s), releasing NE with NPY as a co-transmitter at high firing frequencies. Stellate ganglion contains five adrenergic subtypes total, three of which innervate the heart (NA1a: high NPY; NA1b/NA1c: low NPY), confirmed by single-cell transcriptomic profiling [8, 10].

**Gating:** Presynaptic α2 autoreceptors on postganglionic terminals provide frequency-dependent autoinhibition — α2A and α2C subtypes show distinct frequency-response profiles in mouse, likely conserved in humans [confirmed in rodent; human data limited]. Satellite glia in sympathetic ganglia actively modulate neuronal excitability via purinergic signaling; their role is not passive support [9, 11]. Baroreflex provides the primary negative feedback gate: BP rise → NTS → CVLM → RVLM inhibition → reduced IML drive.

**Detection:** The SNS does not directly sense organ state; it receives processed error signals from the RVLM, which integrates baroreceptor feedback, chemoreceptor signals, and descending stress commands. The adrenal medulla detects splanchnic drive directly via nAChR.

**Accumulation:** Chronic sympathetic excess — as in sustained psychological stress, heart failure, or chronic pain — produces β1 receptor downregulation on the heart, α1 upregulation on vasculature, reduced baroreflex gain, and structural remodeling of the stellate ganglion, increasing ventricular arrhythmia risk [10]. These changes develop over weeks to months.

**Refinement:** Exercise training increases vagal dominance via baroreflex resetting, reducing resting sympathetic tone. HRV biofeedback protocols train the vagal-sympathetic balance over 6-week periods, with demonstrated reduction in resting HR and anxiety symptoms [12].

### §2.2 — Parasympathetic (PSNS) and Vagal Architecture

The parasympathetic (PSNS) efferent pathway originates in the brainstem (cranial nerves III, VII, IX, X) and sacral spinal cord (S2–S4). The vagus nerve (CN X) constitutes approximately 75% of parasympathetic outflow, innervating the thoracic and abdominal viscera through terminal ganglia located at or within target organs, allowing highly localized control [1]. A critical feature: the vagus nerve is primarily afferent — approximately 80–90% of its fibers carry sensory information from organs to the brain, not motor commands from brain to organs [7, 8].

**Propagation:** Cardiac vagal output originates in the nucleus ambiguus (nAmb), which sends myelinated B-fibers to intracardiac ganglia → short postganglionic ACh → M2 receptors on SA/AV nodes → bradycardia and reduced conduction velocity. Visceral output (gut, lungs, liver) originates in the dorsal motor nucleus of the vagus (DMV), organized viscerotopically: distinct neuronal populations project to esophagus, stomach, intestine, and liver in spatially segregated subregions.

**Gating:** nAmb firing is gated by NTS baroreceptor input, respiratory rhythm (producing respiratory sinus arrhythmia — RSA), and top-down cortical/limbic input via the PAG. RSA amplitude is the physiological basis of HRV: breathing-synchronized vagal tone modulation creates beat-to-beat heart rate variability, and RMSSD is a validated proxy for vagal tone [6].

**Detection:** The vagal afferent system — through the nodose and jugular ganglia — constitutes the brain's primary organ state sensing apparatus. The nodose ganglion contains 18–27 molecularly distinct neuron types by single-cell RNA sequencing [7], dedicated to surveying cardiovascular, pulmonary, gastrointestinal, hepatic, and immune state. This fiber ratio (80–90% afferent) means the primary mode of organ-brain interaction via the vagus is sensing, not commanding.

**Accumulation:** Chronic vagal withdrawal — common in depression, PTSD, and chronic pain — reduces HRV, impairs the cholinergic anti-inflammatory pathway, reduces cephalic-phase insulin secretion, and impairs gut motility. These changes develop over weeks to months and are associated with elevated cardiovascular risk and systemic inflammation [5, 12].

**Refinement:** Vagal tone is trainable. HRV biofeedback at resonance frequency breathing increases RMSSD and reduces trait anxiety over 6-week protocols [12]. Implanted VNS is FDA-approved for epilepsy (1997) and treatment-resistant depression (2005). Transcutaneous t-VNS (gammaCore) is FDA-cleared for cluster headache and episodic migraine; its use for other indications is supported by evidence but not fully FDA-approved.

### §2.3 — Enteric Nervous System

The ENS is a semi-autonomous neural computer embedded in the gut wall [2, 20]. Its two primary plexuses serve distinct functions: the myenteric plexus (between muscle layers) controls motility through ascending excitatory (ACh + SP) and descending inhibitory (NO + VIP) reflex arcs; the submucosal plexus (in the submucosa) controls secretion, mucosal blood flow, and epithelial function. Peristalsis continues after vagotomy — demonstrating ENS autonomy — but is modulated in amplitude and frequency by vagal efferent input.

**Propagation:** The peristaltic reflex is initiated by intrinsic primary afferent neurons (IPANs) detecting distension, not by direct luminal sensing. A critical recent finding [18]: enteric neurons do not directly sense nutrients; detection is mediated through the epithelium, primarily via serotonin (5-HT) released by enterochromaffin (EC) cells in response to luminal chemical and mechanical stimuli. Different nutrients activate neurochemically defined ensembles of myenteric and submucosal neurons through this epithelial-first pathway.

**Gating:** EC cell 5-HT release gates ENS circuit gain. Peripheral 5-HT from EC cells is produced by a gut-specific enzyme (TPH1), does not cross the blood-brain barrier, and is a completely separate pool from central 5-HT. Microbiome spore-forming bacteria are required for over 90% of colonic EC cell serotonin synthesis [14, 42] — dysbiosis therefore directly reduces ENS 5-HT tone and gut motility. SNS NE → α2 on ENS neurons provides a motility brake during fight-or-flight states.

**Detection:** Neuropod cells — a subset of enteroendocrine cells that form direct synaptic contacts with ENS neurons — provide rapid synaptic-scale chemosensory transduction [15], far faster than hormonal diffusion. Vagal afferents in the gut lumen respond directly to select microbial metabolites via receptor-mediated signaling [17], providing a real-time microbiome-to-brain signaling pathway independent of EEC hormone intermediaries. Topological segregation of stress-sensor subtypes along the crypt-to-villus axis adds spatial specificity to gut chemosensation [19].

**Accumulation:** Post-infectious IPAN sensitization can persist months to years after gut inflammation resolves, producing the post-infectious IBS phenotype. Alpha-synuclein misfolding in ENS myenteric neurons — triggered in part by reduced SCFA production from PD-associated gut dysbiosis — represents one of the earliest detectable changes in Parkinson's disease, preceding motor symptoms by years to decades [16]. Obesity is associated with vagal mechanoreceptor desensitization and GLP-1 receptor downregulation, progressively reducing satiety signaling efficiency [rodent diet-induced obesity models; human data consistent but indirect].

**Refinement:** Microbiome restoration partially recovers ENS serotonin synthesis and neuroprotection over weeks. Enteric glia support ENS circuit maintenance through GDNF signaling; glial regulation of gut motility shows sex differences, mechanism incompletely understood (Tier B, recent).

### §2.4 — Somatic Peripheral Nervous System: DRG Sensory Neurons

DRG neurons are the first-order sensory neurons for all somatic (and some visceral) modalities. Their pseudo-unipolar morphology — one axon bifurcating into peripheral receptor branch and central spinal cord branch — places cell bodies outside the CNS, partially unprotected by the blood-brain barrier. This exposes them to circulating inflammatory mediators and makes the DRG a site of peripheral sensitization in both inflammatory and neuropathic pain states.

A human DRG reference atlas constructed from 126 donors (2025, preprint [22]) resolves 22 neuronal subtypes spanning nociception, mechanosensation, thermosensation, and proprioception. Prior to this resource, most mechanistic understanding was derived from rodent models. The 2025 atlas confirms that human DRG neurons are substantially larger than their mouse counterparts and that hair follicle-innervating A-fiber LTMRs conduct faster in humans — suggesting species-specific adaptations in mechanosensation. Cross-species validation confirms conserved core modules alongside human-specific adaptations [23]. Individual human subtype identities should be treated with caution until the preprint receives peer review (Tier C for human-specific claims).

**Propagation:** Nociceptors transduce noxious stimuli through modality-specific ion channels — TRPV1 (heat >43°C, capsaicin, acid), TRPA1 (reactive chemicals, cold allodynia), TRPM8 (innocuous cold) — and conduct via C-fibers (0.5–2 m/s, aching/burning) and Aδ-fibers (5–30 m/s, sharp) [3, 27]. Low-threshold mechanoreceptors (LTMRs) [30] use PIEZO2 as a primary mechanotransduction channel; PIEZO2 loss-of-function in humans produces severe loss of both touch and proprioception, confirming its essential role in both modalities [24]. Peptidergic nociceptors (previously treated as one class) comprise at least seven molecularly distinct subtypes with distinct thresholds and axon morphologies [21].

**Gating:** Gate control operates at the dorsal horn: simultaneous Aβ tactile fiber activity activates GABAergic inhibitory interneurons that suppress C-fiber nociceptor signal transmission — the physiological basis of TENS analgesia and vibration analgesia [25]. Descending inhibition from the PAG via the RVM provides a second gating layer through 5-HT and NE projections to the dorsal horn.

**Detection:** Each nociceptor subtype detects a specific stimulus modality; threshold is set by inflammatory sensitization state. The key sensitization cascade: tissue damage → PGE2/NGF/bradykinin → TRPV1 phosphorylation and Nav1.8 upregulation → reduced detection threshold → hyperalgesia (exaggerated pain to noxious stimuli) and allodynia (pain from normally innocuous stimuli). Nav1.8-selective blockers (suzetrigine/VX-548, FDA-approved January 2025) represent the first peripherally-selective sodium channel pain drug, validating Nav1.8 as a nociceptor-specific therapeutic target.

**Accumulation:** Neuropathic pain involves ectopic discharge from DRG cell bodies after nerve injury, Nav1.8 upregulation, satellite glia gap junction coupling (spreading sensitization to neighboring neurons), and central sensitization via BDNF-TrkB-KCC2 downregulation at the dorsal horn — shifting GABA from inhibitory to excitatory [26, 37]. These changes persist over weeks to months and are the substrate for chronic pain syndromes.

**Refinement:** Resolution of acute inflammation reverses TRPV1 sensitization within hours to days. Chronic sensitization involves epigenetic changes in DRG neurons — histone acetylation patterns sustaining Nav1.8 upregulation have been described in rodent neuropathic pain models — that are slower to reverse [rodent; human epigenetic mechanisms under investigation]. CGRP monoclonal antibodies (erenumab, fremanezumab) prevent migraine by blocking peripheral CGRP signaling at trigeminal afferents [28].

### §2.5 — Somatic Peripheral Nervous System: NMJ and Proprioceptors

The neuromuscular junction is the output synapse of the somatic motor system. Its safety factor of 3–4× — meaning the end-plate potential normally far exceeds the threshold for muscle action potential — makes it highly reliable under normal conditions. Disease reduces this safety factor: myasthenia gravis (anti-AChR or anti-MuSK antibodies) progressively destroys postsynaptic architecture until transmission fails. The molecular maintenance of the NMJ is driven by agrin/LRP4/MuSK signaling and, as recently identified, by electrical activity through the ETV4 transcription factor [29] — NMJ maintenance depends on both trophic and activity-dependent mechanisms.

Proprioceptors — muscle spindles and Golgi tendon organs — provide the continuous positional and force feedback that enables motor control. Muscle spindle Ia afferents (encoding velocity) project monosynaptically to alpha motor neurons, producing the stretch reflex (latency ~30 ms), and to the cerebellum via spinocerebellar tracts for real-time motor correction. GTO Ib afferents encode active tension and drive autogenic inhibition, preventing excessive force production. Both use PIEZO2 as a primary mechanotransduction channel [24].

Gamma motor neurons continuously adjust spindle sensitivity by contracting intrafusal fibers, maintaining Ia afferent sensitivity during muscle shortening. Without alpha-gamma co-activation, muscle spindles would go silent during contraction, eliminating proprioceptive feedback during the most important phase of movement. Age-related proprioceptive decline — driven by decreased spindle density and reduced Ia firing accuracy — is a major contributor to falls risk in older adults [31].

---

## §3 — Cross-Division Interaction Network

The three PNS divisions share brainstem relay structures (NTS, parabrachial nucleus), are modulated by overlapping descending pathways, and interact through direct molecular mechanisms. The cross-division interaction network helps determine the integrated peripheral state — which is often not well predicted by any single division in isolation.

Table 1 maps the primary cross-division interactions, showing each system as both driver and target. Confidence markers follow the evidence tier definitions from §1.

**Table 1. Cross-division interaction network.** (A) Tier A consensus; (B) directly supported; (B-C) mixed confidence; (C) emerging/synthetic.

| System Driver | → SNS | → PSNS/Vagal | → ENS | → Somatic PNS | Mechanism |
|---|---|---|---|---|---|
| SNS activation | — | Reciprocal PSNS withdrawal (baroreceptor, central) | NE → α2 on ENS → motility suppression (A) | NE → α1/α2 on DRG nociceptors; SNS → DRG sprouting after injury → CRPS (B) | RVLM → IML → NE release; baroreceptor reflex |
| PSNS/Vagal tone | Reciprocal SNS suppression (baroreceptor) | — | ACh → M1/M3 on ENS + EC cells → motility + secretion (B); cephalic insulin via direct vagal→pancreas M3 pathway (B) | Descending: PAG → RVM → dorsal horn → pain gate modulation (B) | NTS → nAmb → DMV → organ targets; HRV as proxy |
| ENS/gut signals | GLP-1, CCK, 5-HT → vagal → NTS → hypothalamus; HPA coupling via EndocrineSystem [34] (B) | Vagal afferents 80–90% afferent → NTS; gut state continuously updates brain (A) | — | Visceral-somatic convergence at dorsal horn → referred pain (A) | Nodose ganglion → NTS → RVLM/hypothalamus/parabrachial |
| Somatic PNS (pain/proprioception) | Pain → reflex sympathetic response; stress hyperalgesia (B) | Pain → reflex vagal withdrawal; proprioception → cerebellum → motor correction (B) | Visceral afferents converge with somatic at dorsal horn; no direct somatic→ENS | — | Spinothalamic (pain) and dorsal column (touch/proprioception) pathways |
| Microbiome/ENS interface | SCFAs → EEC → GLP-1 → vagal → NTS → hypothalamus; HPA via [34] (B) | SCFAs + microbial metabolites → vagal afferent direct activation [Jameson 2024] (B) | SCFAs → GPR41/43; tryptophan → 5-HT synthesis; α-syn seeding in ENS (B-C) | Tryptophan/kynurenine competition affects central pain processing (B) | Portal → liver → portal vagal afferents; systemic metabolite diffusion |

### §3.1 — The Baroreflex as the Core ANS Integration Loop

The baroreflex is the primary real-time homeostatic loop integrating SNS and PSNS cardiovascular control. Baroreceptors in the aortic arch and carotid sinus detect blood pressure as mechanical stretch → vagal Aβ afferents → NTS → CVLM (inhibits RVLM → suppresses SNS) + nAmb (excites vagal cardiac output → reduces HR). This loop operates with a gain of approximately 20 ms/mmHg in healthy adults and is reduced in chronic hypertension, heart failure, and aging. HRV is the principal non-invasive metric of baroreflex-mediated vagal-sympathetic balance [6].

### §3.2 — The Cholinergic Anti-Inflammatory Pathway

Vagal efferents (DMV) → celiac ganglion → splenic sympathetic nerve → norepinephrine → choline acetyltransferase-expressing T cells → acetylcholine → α7 nicotinic receptors on splenic macrophages → JAK2/STAT3 → suppression of TNF-α, IL-1β, and IL-6. This pathway was initially described in rodent sepsis models [5] and has since been supported by human vagal nerve stimulation studies showing reduced inflammatory markers in rheumatoid arthritis [38] and Crohn's disease [39]. It provides one mechanism by which vagal tone modulates systemic inflammation — and by which chronic vagal withdrawal (depression, PTSD) is associated with elevated inflammatory markers. The pathway is indirect: vagal efferents do not directly contact macrophages; the relay through splenic NE and ChAT T cells is required.

### §3.3 — The Gut-Brain Sensing Hierarchy

The vagal-ENS-microbiome signaling stack operates through at least four parallel channels: (1) intestinal mechanoreceptors (IGLEs) detect distension → vagal afferents → NTS → hypothalamic AgRP inhibition, providing the fastest satiety signal [13]; (2) enteroendocrine cells release GLP-1, CCK, and 5-HT → vagal afferents → NTS → hypothalamus → metabolic regulation; (3) select microbial metabolites in the gut lumen directly activate vagal afferents through receptor-mediated signaling [17], bypassing EEC entirely; (4) systemic SCFAs and amino acid metabolites (tryptophan, indoles) reach the CNS through the portal circulation and partial BBB crossing.

A critical architectural point: peripheral 5-HT from EC cells is a completely separate pool from central 5-HT. Gut-derived 5-HT regulates ENS function and provides a vagal nausea/satiety signal via 5-HT3 on nodose afferents. It does not cross the blood-brain barrier. The gut-mood connection attributed to gut serotonin is indirect — it operates through vagal signaling to the NTS, not through peripheral 5-HT reaching the brain. Microbiome dysbiosis reduces EC cell 5-HT production (via reduced spore-forming bacteria) and shifts tryptophan toward the kynurenine pathway (via IDO1 activation), reducing central 5-HT substrate while increasing neurotoxic quinolinic acid [40] — a convergence that links gut dysbiosis to depression risk through a pathway that is distinct from gut-to-brain serotonin transfer.

### §3.4 — Visceral-Somatic Convergence and Referred Pain

Visceral afferents (via vagal and spinal routes) and somatic afferents converge on the same dorsal horn interneurons. The brain cannot distinguish input source from shared interneurons, producing referred pain: cardiac ischemia → left arm and jaw; renal colic → flank and groin; appendicitis → periumbilical (initially) → right iliac fossa (later, as parietal peritoneum involvement shifts to somatic). This convergence is a structural feature of DRG and dorsal horn anatomy, not a pathological phenomenon, and produces the fixed dermatomal referred pain maps used clinically [1]. It also means that visceral sensitization (from IBD, IBS, or ENS inflammation) can lower somatic pain thresholds in overlapping dermatomes — a mechanism of central sensitization that crosses the visceral-somatic divide.

### §3.5 — Sympathetically Maintained Pain and DRG Coupling

After peripheral nerve injury, SNS postganglionic axons can sprout into the DRG, forming perineuronal baskets around nociceptor cell bodies. Normally inhibitory α2 adrenergic receptors on nociceptors are downregulated after injury, while excitatory α1 receptors are upregulated, converting the sympathetic NE signal from inhibitory to excitatory. This produces sympathetically maintained pain — pain that worsens with sympathetic activation and is relieved by sympathetic blockade — the defining feature of complex regional pain syndrome (CRPS). The mechanism links the SNS to the somatic pain pathway through structural remodeling at the DRG level [41].

---

## §4 — Multi-System Failure Cascades

Each PNS division has characteristic failure modes emerging from the accumulation states described in §2. The following patterns are integrative syntheses (Tier C): each component mechanism is supported at the tier indicated, but the cascades as unified clinical patterns are proposed based on mechanistic connections, not directly measured as unified syndromes.

### §4.1 — Chronic Stress and Autonomic Dysregulation

Sustained psychological stress initiates a co-activation of the HPA axis and SNS that, over months to years, can propagate through the cross-division links described in §3. Sustained SNS activation is associated with: (1) reduced baroreflex gain → impaired HRV → elevated cardiovascular risk (Tier A/B, well-supported); (2) suppressed ENS motility via prevertebral ganglion NE release → functional dyspepsia and constipation patterns (Tier B); (3) sensitized DRG nociceptors and ENS IPANs via stress-driven mast cell activation — CRH, NE → mast cell degranulation → tryptase → PAR2 → sensitization [33] (Tier B); (4) reduced vagal tone → reduced cholinergic anti-inflammatory → elevated systemic cytokines (Tier B for each individual step; combined direction is inferred); (5) altered gut motility and immune state → possible microbiome composition shift → reduced SCFA (Tier C; directionality not established in humans). Each individual mechanism is supported; the HPA-ANS co-activation architecture and cortisol downstream effects are documented in the companion Endocrine System paper [34]. Their combined propagation as a unified cascade is an integrative hypothesis [33].

### §4.2 — Gut Dysbiosis and Peripheral Neural Decline

Gut dysbiosis — a persistent shift in microbiome composition reducing SCFA-producing and tryptophan-metabolizing bacteria — has documented effects across multiple PNS divisions. In the ENS: reduced butyrate → reduced HDAC inhibition → may reduce tight junction protein expression → increased intestinal permeability → elevated luminal LPS exposure → ENS neuroinflammation (each step supported; the full chain is inferential at stages 3–4 [32]); reduced EC cell 5-HT → impaired motility; alpha-synuclein misfolding in myenteric neurons — mechanism supported by histopathology (Tier B); clinical timeline of ENS-to-brainstem propagation in human PD remains a hypothesis (Tier C) [16]. In the vagal afferent system: reduced SCFA → reduced GPR41/43 activation on nodose afferents → reduced gut-to-brain metabolic signaling; reduced tryptophan → reduced serotonin precursor availability. In the somatic PNS: kynurenine pathway shift increases quinolinic acid (NMDA agonist) → may lower pain thresholds (indirect; Tier C). The combined pattern is consistent with the gut-centric early pathology described in Parkinson's disease, depression, and metabolic-cognitive syndrome — but the cascade as a unified clinical entity remains a proposed synthesis.

### §4.3 — Chronic Pain Chronification

Peripheral sensitization from sustained tissue damage or nerve injury can chronify through two sequential mechanisms: (1) peripheral: Nav1.8 upregulation + ectopic discharge from DRG cell bodies + satellite glia coupling (spreading sensitization across neighboring neurons); (2) central: activated spinal microglia release BDNF → TrkB on dorsal horn neurons → KCC2 downregulation → GABA becomes excitatory → dorsal horn hyperexcitability → central sensitization [26, 37]. Once central sensitization is established, the peripheral injury may resolve while chronic pain persists — the mechanism of fibromyalgia and post-inflammatory pain syndromes. The SNS can amplify this through DRG sprouting (α1 upregulation → CRPS), closing a positive feedback loop. Each link in this chain is individually supported at Tier B or higher; the full sequence as a unified pathological program is a proposed synthesis — the relative contribution of peripheral vs. central mechanisms varies substantially across patients and pain conditions, and no single study has traced the complete cascade in humans.

---

## §5 — The Integrated Peripheral Nervous System

The three PNS divisions form an integrated sensing and effector network that operates in parallel with the endocrine system to couple brain state to body state:

- **SNS:** fast (milliseconds to seconds) resource mobilization; sets cardiovascular, metabolic, and immune state for threat response; co-activates with HPA axis in acute stress
- **PSNS/Vagal:** fast (milliseconds to seconds) restoration and organ state maintenance; primary mode of organ interaction is afferent sensing (80–90% of vagal fibers); cholinergic anti-inflammatory pathway links vagal tone to systemic inflammation; HRV is the principal integration metric
- **ENS:** semi-autonomous gut computer; executes local motility, secretion, and mucosal defense reflexes; primary interface between microbiome and nervous system; source of approximately 90–95% of body serotonin (separate pool from CNS) [14, 42]
- **Somatic sensory (DRG):** body surface and visceral sensory array; converges with ENS visceral signals at dorsal horn; peripheral and central sensitization are the substrate of chronic pain
- **Somatic motor (NMJ + proprioceptors):** motor output and real-time feedback loop; NMJ safety factor determines neuromuscular reliability; proprioceptors feed back to cerebellum and spinal cord for continuous motor correction

These components operate at different timescales — milliseconds (NMJ, stretch reflex, vagal cardiac), seconds (baroreflex, nociception), minutes (ENS motility, peripheral sensitization), days to weeks (central sensitization, gut dysbiosis consequences) — yet are coupled through shared brainstem infrastructure and are usefully understood as a system rather than independent processes. The boundary between the peripheral and central nervous system is more porous than the classical division suggests: DRG neurons are partially outside the BBB; vagal ganglia lie outside the CNS but have direct afferent access to brainstem nuclei; ENS signals reach the hypothalamus and amygdala via the NTS-parabrachial pathway, shaping emotional and motivational state continuously.

---

## §6 — Scope, Limitations, and Companion References

This paper describes the functional architecture of the peripheral nervous system across three divisions. The framework's contribution is the cross-division interaction map and the identification of multi-system failure cascades — not the individual mechanistic findings, which are established in the cited literature. Four limitations apply.

**First,** evidence confidence varies substantially across divisions. Autonomic physiology and the NMJ are among the best-characterized areas of neuroscience (Tier A dominates). ENS microbiome coupling and ENS neuroplasticity contain significant Tier B evidence with important rodent-to-human translation caveats. Human DRG subtype-specific functional roles (2025 preprint) are Tier C until peer review. The evidence tiers box in §1 specifies confidence for major claims.

**Second,** brain-interface effects are not covered here. Receptor distributions, circuit-level effects at NTS, thalamus, insula, ACC, and amygdala, and disease-specific CNS mechanisms are covered in the companion Brain-Body reference (BrainBody v1.3) [35] and in the relevant brain structure maps (BrainMap_NTS, BrainMap_Insula, BrainMap_PAG, BrainMap_SensoryCortex, BrainMap_Cerebellum). The endocrine coupling described in §3 is covered in depth in the companion Endocrine System paper.

**Third,** the failure cascades in §4 are integrative syntheses. Each component mechanism is supported at the tier indicated; the cascades as unified clinical patterns are proposed rather than directly measured, and are intended to generate testable predictions rather than substitute for direct clinical evidence.

**Fourth,** neurotransmitter parameter values are not specified here. Canonical parameter values for NE, ACh, 5-HT, dopamine, GABA, and glutamate dynamics — receptor subtypes, signaling cascades, and simulation-ready formulas — are documented in the companion Neurochemistry Formula Correspondence reference [36]. That document is the authoritative source for NT parameters; values in this paper are qualitative only.

**Integration target:** This paper is designed to merge into the Brain-Body Unified Reference (BrainBody) as its peripheral nervous system architecture component, alongside the Endocrine System paper. Merge target: BrainBody §2 (organ-level reference) for the individual division architectures; BrainBody §3 (body-to-brain interface) for the cross-division interaction maps and gut-brain signaling hierarchy. The Simulation Role Appendix migrates with the merge and supersedes any division-level encoding guidance in earlier BrainBody drafts. Until the merge, this document stands as the canonical peripheral nervous system architecture reference.

---

## Appendix — Simulation Role Classification of Cross-Division Links

Each cross-division mechanism is classified as **Core Rule** (safe to encode as baseline), **Supported Modifier** (conditional, toggle-able), or **Hypothesis Layer** (optional provisional module). Classifications follow the evidence tier assignments in §1.

| Cross-System Link | Tier | Role | Notes |
|---|---|---|---|
| SNS NE → α/β adrenergic organ effects | A | Core Rule | Organ-specific receptor subtypes well-established; encode as per-organ NE response function |
| PSNS ACh → muscarinic receptor effects | A | Core Rule | M2 cardiac (Gi), M3 smooth muscle/glands (Gq); encode per organ target |
| Baroreflex: MAP → NTS → RVLM/nAmb → SNS/PSNS adjustment | A | Core Rule | Primary cardiovascular homeostasis loop; encode with baroreflex_gain parameter |
| SCN → sympathetic chain → pineal NE → melatonin synthesis | A | Core Rule | Strict serial pathway; NE floor elevation delays DLMO; full documentation in EndocrineSystem §2.5 [34] |
| HRV-RMSSD as vagal tone proxy parameter | A | Core Rule | Trainable; encode as current vagal_tone estimate |
| Gate control: Aβ concurrent activity → GABAergic suppression of C-fiber signal | A | Core Rule | Basis of TENS and vibration analgesia; encode as pain_gate_modulation |
| Ia monosynaptic stretch reflex (30 ms) | A | Core Rule | Fastest spinal reflex; encode with sub-100ms tick for motor control loop |
| NMJ ACh quantal transmission + safety factor | A | Core Rule | Safety factor ~3–4×; encode as threshold ratio; disease reduces it |
| EC cell 5-HT ≠ CNS 5-HT (separate pools, no BBB crossing) | A | Core Rule | Critical: gut serotonin controls motility, not mood directly; separate parameters |
| GLP-1 incretin amplification (50–70% of oral glucose insulin response) | A | Core Rule | Already Core Rule in EndocrineSystem paper; confirm here |
| Cholinergic anti-inflammatory pathway: vagal tone → TNF-α/IL-1β suppression | B | Supported Modifier | Human sepsis + rodent evidence; encode as vagal_tone × α7_nAChR_spleen → cytokine reduction |
| Satellite glia active modulation in sympathetic ganglia | B | Supported Modifier | Mouse; encode as ganglion_gain_modulator; toggle off for minimal model |
| Stellate ganglion organ-specific subtypes (NA1a high-NPY, NA1b/NA1c low-NPY) | B | Supported Modifier | scRNA-seq; encode as cardiac SNS subtype differentiation when modeling arrhythmia risk |
| Nutrients detected indirectly via epithelium → 5-HT → ENS | B | Supported Modifier | Not direct ENS sensing [Nature 2025]; encode EC cell as sensory intermediary |
| Intestinal IGLE mechanoreceptors → AgRP inhibition (satiety signal) | B | Supported Modifier | Mouse [Cell 2019]; encode as gut_stretch → hunger_suppression |
| SCFA → GPR41/43 → GLP-1 + ENS activation | B | Supported Modifier | Multiple studies; microbiome → butyrate → ENS neuroprotection; encode as microbiome_quality modifier |
| Peripheral pain sensitization: TRPV1 sensitized by PGE2/NGF | B | Supported Modifier | Encode as detection_threshold[heat] reduced by inflammatory_index |
| Central sensitization: BDNF-TrkB-KCC2 after nerve injury | B | Supported Modifier | Well-supported; encode as chronic_pain_index accumulating over weeks |
| Alpha-synuclein ENS seeding → retrograde vagal spread | B | Supported Modifier | Epidemiological + histopathological support; encode as alpha_syn_ENS_burden → PD risk |
| CGRP → neurogenic inflammation + migraine | B | Supported Modifier | Anti-CGRP antibodies clinically validated; encode CGRP as pain amplifier co-transmitter |
| HRV biofeedback → trainable vagal tone increase | B | Supported Modifier | 6-week protocols validated [Gitler 2025]; encode vagal_tone as trainable parameter |
| Human DRG 22 neuronal subtypes | C | Hypothesis Layer | 2025 preprint awaiting peer review; do not encode specific subtypes until confirmed |
| Long COVID dysautonomia mechanism | C | Hypothesis Layer | Emerging 2023–2025; mechanism unresolved; encode as optional dysautonomia_flag |
| Psychobiotics → CNS mood effects | C | Hypothesis Layer | Preclinical predominant; human trials mixed; treat as optional modifier with wide uncertainty |
| Chronic stress cascade as unified multi-system syndrome | C | Hypothesis Layer | Component mechanisms supported; cascade as unified pattern is proposed synthesis [§4.1]; encode components separately |

---

## References

- [1] Jänig W. *The Integrative Action of the Autonomic Nervous System.* Cambridge University Press (2006).
- [2] Furness JB. *The Enteric Nervous System.* Blackwell Publishing (2006).
- [3] Basbaum AI et al. Cellular and molecular mechanisms of pain. *Cell* 139(2) (2009) 267–284.
- [4] Guyenet PG. The sympathetic control of blood pressure. *Nat Rev Neurosci* 7(5) (2006) 335–346.
- [5] Tracey KJ. The inflammatory reflex. *Nature* 420 (2002) 853–859.
- [6] Task Force of the European Society of Cardiology and the North American Society. Heart rate variability: standards of measurement. *Eur Heart J* 17 (1996) 354–381.
- [7] Kupari J et al. An atlas of vagal sensory neurons and their molecular specialization. *Cell Rep* 27(8) (2019) 2508–2523.
- [8] Wang T et al. Molecular and functional diversity of the autonomic nervous system. *Nat Rev Neurosci* 26(10) (2025) 607–622.
- [9] Mapps AA et al. Satellite glia modulate sympathetic neuron survival, activity, and autonomic function. *eLife* 11 (2022) e74295.
- [10] Ajijola OA et al. Defining the neural fulcrum for chronic myocardial infarction: stellate ganglia transcriptomics, cell subtype identities, and morphological structure. *Heart Rhythm* 17(4) (2020) 677–684.
- [11] Scherschel K et al. Glia of the heart's nervous system. *Nat Rev Neurosci* 26 (2025) 737–748.
- [12] Gitler H et al. Harnessing non-invasive vagal neuromodulation: HRV biofeedback and SSP for cardiovascular and autonomic regulation. *PeerJ* (2025). [Narrative review; 6-week HRV biofeedback protocol data from Karavidas et al. 2007 therein]
- [13] Bai L et al. Genetic identification of vagal sensory neurons that control feeding. *Cell* 178(5) (2019) 1129–1143.
- [14] Yano JM et al. Indigenous bacteria from the gut microbiota regulate host serotonin biosynthesis. *Cell* 161(2) (2015) 264–276.
- [15] Bohórquez DV et al. Mechanosensory circuit formed by innervation of sensory enteroendocrine cells. *J Clin Invest* 125(2) (2015) 782–786. [Neuropod cell anatomy] See also: Bohórquez DV et al. Neuropod cell periphery in gut sensory transduction. *Science* 373(6559) (2021) 1107–1110.
- [16] Braak H et al. Gastric alpha-synuclein immunoreactive inclusions in Meissner and Auerbach's plexuses. *Acta Neuropathol* 105(5) (2003) 515–530.
- [17] Jameson KG et al. Select microbial metabolites in the small intestinal lumen regulate vagal activity via receptor-mediated signaling. *iScience* 28(2) (2024) 111699.
- [18] Gribble FM et al. Nutrients activate distinct patterns of small-intestinal enteric neurons. *Nature* (2025 Jul). DOI: 10.1038/s41586-025-09228-z.
- [19] Touhara KK et al. Topological segregation of stress sensors along the gut crypt-villus axis. *Nature* 640 (2025) 732–742.
- [20] Sharkey KA & Lomax AEG. The enteric nervous system. *Physiol Rev* 102 (2022) 1421–1492.
- [21] Qi L et al. A mouse DRG genetic toolkit reveals morphological and physiological diversity of somatosensory neuron subtypes. *Cell* 187(6) (2024) 1519–1534.
- [22] Bhuiyan SA et al. A Reference Atlas of the Human Dorsal Root Ganglion. *bioRxiv* 2025.11.05.686654 (2025). Preprint — not yet peer reviewed.
- [23] Jung M et al. Cross-species transcriptomic atlas of dorsal root ganglia reveals species-specific programs for sensory function. *Nat Commun* 14 (2023) 644.
- [24] Chesler AT et al. The role of PIEZO2 in human mechanosensation. *NEJM* 375 (2016) 1560–1568.
- [25] Melzack R & Wall PD. Pain mechanisms: a new theory. *Science* 150(3699) (1965) 971–979.
- [26] Woolf CJ. Central sensitization: implications for the diagnosis and treatment of pain. *Pain* 152(3 Suppl) (2011) S2–15.
- [27] Julius D. TRP channels and pain. *Annu Rev Cell Dev Biol* 29 (2013) 355–384.
- [28] Edvinsson L et al. CGRP as the target of new migraine therapies. *Nat Rev Neurol* 14 (2018) 338–350.
- [29] [Author TBC — confirm before release]. Single-nuclei sequencing of skeletal muscle reveals subsynaptic-specific transcripts involved in neuromuscular junction maintenance. *Nat Commun* 16 (2025) 2220. DOI: 10.1038/s41467-025-56494-y.
- [30] Abraira VE & Ginty DD. The sensory neurons of touch. *Neuron* 79(4) (2013) 618–639.
- [31] Kröger S & Watkins B. Muscle spindle function in healthy and diseased muscle. *Skeletal Muscle* 11(1) (2021) 1–13.
- [32] Stilling RM et al. The neuropharmacology of butyrate: the bread and butter of the microbiota-gut-brain axis? *Neurochem Int* 99 (2016) 110–132.
- [33] Mayer EA. Gut feelings: the emerging biology of gut-brain communication. *Nat Rev Neurosci* 12(8) (2011) 453–466.
- [34] Finnegan M. The Endocrine System as a Distributed Detection Architecture. Unpublished draft v1.1 (2026). [Companion paper]
- [35] Finnegan M. The Brain-Body System: A Unified Reference for Medicine. Unpublished draft v1.3 (2026). [Companion reference]
- [36] Finnegan M. Neurochemistry Formula Correspondence. Unpublished reference v1.6 (2026). [Canonical NT parameter values]
- [37] Coull JA et al. Trans-synaptic shift in anion gradient in spinal lamina I neurons as a mechanism of neuropathic pain. *Nature* 424 (2003) 938–942.
- [38] Koopman FA et al. Vagus nerve stimulation inhibits cytokine production and attenuates disease severity in rheumatoid arthritis. *Proc Natl Acad Sci USA* 113(29) (2016) 8284–8289.
- [39] Bonaz B et al. Chronic vagus nerve stimulation in Crohn's disease: a 6-month follow-up pilot study. *Neurogastroenterol Motil* 28(6) (2016) 948–953.
- [40] Schwarcz R et al. Kynurenines in the mammalian brain: when physiology meets pathology. *Nat Rev Neurosci* 13(7) (2012) 465–477.
- [41] Jänig W & Baron R. Complex regional pain syndrome: mystery explained? *Lancet Neurol* 2(11) (2003) 687–697.
- [42] Gershon MD & Tack J. The serotonin signaling system: from basic understanding to drug development for functional GI disorders. *Gastroenterology* 132(1) (2007) 397–414.
