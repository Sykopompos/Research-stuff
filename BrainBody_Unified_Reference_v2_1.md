# The Brain-Body System

## A Unified Reference for Medicine

*Hormones · Neurosteroids · Sex Differences · The Integrated System
Across the Lifespan*

*Peripheral Architecture · Organ Systems · Body-State Translation ·
Exercise Architecture*

M. Finnegan · ORCID: 0009-0009-4921-7722 · v2.1 — March 2026 ·
Unpublished draft, not yet peer reviewed

> **Simulation Design Notice**
> 
> *This paper is the reference architecture for a series applying a biological detection framework to disease — part of an ongoing project to build a biologically-grounded computational brain and body simulation. v2.1 expands substantially on v1.3: the highway model is extended from six to ten bidirectional axes; the peripheral nervous system and organ system architectures are incorporated in full; an exercise endocrine architecture section documents the four parallel musculoskeletal–hippocampal coupling channels now confirmed in the literature. Detailed FQ decompositions, Rust struct implementations, and silo analyses are in the individual Brain Maps, Peripheral Maps, and Organ System Maps that constitute the full map series. This document is the synthesis index.*
> 
> *All biological claims are mechanistic descriptions of established literature. Nothing in this paper constitutes medical advice.*

## Part I — The Integrated System

### §1 — The Core Argument: One System, Not Two

Medicine has treated the brain and body as separate systems for over a
century — and within that already fragmented picture, has treated
hormones primarily as reproductive signals. Neither separation reflects
biological reality. The brain and body run a continuous bidirectional
conversation across ten primary highways. Hormones are not passenger
signals traveling those highways — they are primary brain modulators
with dual mechanisms of action: fast membrane effects within minutes
\[11\] and slow genomic effects that reshape synaptic topology over
hours to days \[12\]. The brain itself synthesizes steroid hormones
(neurosteroids) independently of the gonads \[13,14\].

Estradiol, testosterone, progesterone and its metabolite
allopregnanolone, DHEA, pregnenolone, and thyroid hormone each have
specific brain targets, specific receptor pathways, and specific
cognitive, emotional, and pain consequences when their levels change.
These systems change dramatically across the human lifespan — from
organizational hormonal effects in the fetal brain that permanently
establish brain architecture, through puberty, peak reproductive years,
and the transitions of menopause and andropause, to the low-hormone
environment of elderhood.

The peripheral nervous system — autonomic, enteric, and somatic
divisions — is the real-time wiring between the brain and every organ.
The vagus nerve alone carries approximately 80–90% of its fibers
afferently: the brain is primarily listening to the body, not commanding
it \[1,2\]. The enteric nervous system operates with roughly 500 million
neurons and a degree of autonomy sufficient to regulate gut motility,
immune surveillance, and gut-brain signaling independently of the spinal
cord \[3\]. Eight major organ systems each maintain dedicated
bidirectional brain interfaces through multiple simultaneous channels:
neural, hormonal, immune, and mechanical.

This paper assembles the complete wiring diagram across all of these
systems. Individual brain structure maps (Brain Maps v2.0 series),
peripheral system maps (Peripheral Maps v1.0 series), and organ system
maps (Organ System Maps v1.0 series) provide full FQ decompositions,
silo analyses, and Rust struct implementations. This document
synthesizes the architecture and indexes into that map series.

### §2 — The Ten Primary Brain-Body Highways

The brain-body interface operates across ten bidirectional communication
highways. The original six recognized in clinical medicine are extended
here to ten, incorporating the musculoskeletal-exercise axis, the
metabolic-insulin axis, the cardiovascular-baroreflex axis, and the
renal-fluid-electrolyte axis — all of which carry direct brain-body
coupling signals not adequately captured in the classic hormonal or
vagal frameworks.

|                                      |                            |                                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                                                                                                                                            |
|--------------------------------------|----------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Highway**                          | **Direction**              | **Primary Carriers**                                                                                                                                                                                                                                                        | **Clinical Consequence of Disruption**                                                                                                                                                                                                                                                                                                                     |
| Vagus Nerve (CN X) \[1,2\]           | ~80% afferent (body→brain) | Afferent: gut mechanoreceptors, chemoreceptors, immune cytokine signals, baroreceptors, pulmonary stretch. Efferent: parasympathetic tone to heart, lungs, gut, liver, pancreas.                                                                                            | Vagal tone loss → inflammatory escalation, IBS, cardiac arrhythmia, gastroparesis. Pre-motor Parkinson’s spreads via vagus. Vagal nerve stimulation treats epilepsy, depression, RA via anti-inflammatory efferent.                                                                                                                                        |
| HPA Axis \[10\]                      | Bidirectional              | Down: CRH (PVN) → ACTH (pituitary) → cortisol (adrenal). Up: cortisol → hippocampal GR → HPA suppression via subiculum.                                                                                                                                                     | Chronic stress → cortisol chronically elevated → hippocampal LTP suppression → memory impairment + immune suppression simultaneously. Depression, PTSD, Cushing’s all involve disrupted HPA feedback.                                                                                                                                                      |
| HPG Axis \[11,12\]                   | Bidirectional              | Down: GnRH (arcuate) → FSH/LH (pituitary) → E2/T/P4 (gonads). Up: gonadal hormones → hypothalamic/pituitary negative feedback. Neurosteroids synthesized locally in brain.                                                                                                  | Gonadal hormone loss (menopause, andropause) directly impairs hippocampal plasticity, PFC function, pain thresholds, mood stability, sleep architecture, and cardiovascular protection simultaneously.                                                                                                                                                     |
| HPT Axis \[22,23\]                   | Bidirectional              | Down: TRH (PVN) → TSH (pituitary) → T3/T4 (thyroid). Up: T3 feedback. D2 in brain (tanycytes, astrocytes) converts T4 to T3 locally — brain T3 regulation is regionally heterogeneous.                                                                                      | Chronic cortisol suppresses D1/D2 → local T3 depletion even with normal TSH. Explains cognitive/mood symptoms in chronic stress with “normal” thyroid panels. T3 deficiency before age 3: irreversible intellectual disability.                                                                                                                            |
| Immune-Brain Axis \[8\]              | Bidirectional              | Body→Brain: IL-1β, IL-6, TNF-α → microglial activation → neuroinflammation. Brain→Body: HPA cortisol → immune suppression; vagal anti-inflammatory reflex; ANS → splenic NE.                                                                                                | Sickness behavior is programmed brain response — not a symptom to suppress. Depression comorbid with inflammatory conditions shares this mechanism. Neuroinflammation: shared pathway in MDD, Alzheimer’s, chronic pain, MS progressive phase.                                                                                                             |
| Gut-Brain Axis \[3,7\]               | Bidirectional              | Vagal afferents from gut (80–90% afferent). ENS: 500M neurons; Meissner’s + Auerbach’s plexuses. Microbiome: SCFA production, tryptophan metabolism, serotonin precursors. Portal circulation: gut-derived signals to liver then systemic.                                  | ENS-CNS disconnection: IBS, functional dyspepsia, gastroparesis. Microbiome disruption: reduced tryptophan availability → 5-HT synthesis ↓. 90% of body’s serotonin is peripheral (enterochromaffin) and does NOT cross BBB — tryptophan crosses via LAT1.                                                                                                 |
| Metabolic-Insulin Axis \[30\]        | Bidirectional              | Brain insulin: crosses BBB via receptor-mediated transcytosis. Targets: hippocampus (LTP), hypothalamus (satiety), cortex (neuroprotection). Leptin/ghrelin/GLP-1: parallel metabolic signals with direct brain receptor expression.                                        | Brain insulin resistance (T2D, obesity) → hippocampal LTP impaired → memory failure. T2D patients: 2× Alzheimer’s risk. GLP-1 receptor agonists: brain GLP-1R activation suppresses hunger (hypothalamus ARC) and may reduce neuroinflammation.                                                                                                            |
| Musculoskeletal-Exercise Axis        | Primarily body→brain       | Myokines (irisin, IL-6-exercise, BDNF-muscle, FGF21) and bone hormones (osteocalcin → GPR158, FGF23). Four parallel channels to hippocampus: osteocalcin/GPR158, irisin/αVβ5, peripheral BDNF/TrkB, lactate/HCAR1. All activated by exercise; all suppressed by inactivity. | Physical inactivity simultaneously suppresses all four brain-protective channels. Exercise is the only known intervention activating all four simultaneously. Sedentary aging cascade: AMPK under-stimulation → sarcopenia → osteocalcin ↓ → hippocampal BDNF ↓ → DG neurogenesis ↓ → cognitive decline (Tier A individual steps; Tier C unified program). |
| Cardiovascular-Baroreflex Axis \[4\] | Bidirectional              | Baroreceptors (carotid sinus, aortic arch) → CN IX/X → NTS → CVLM/RVLM → SNS/PSNS balance. HRV: non-invasive real-time proxy for vagal-brain integration state. Cardiac afferents include ischemic pain (C-fibers), BNP (wall stress), MAP.                                 | Baroreflex failure → uncontrolled hypertension. Right insular cortex lesions → cardiac arrhythmias — the brain directly regulates cardiac rhythm. HRV reduction precedes both cardiovascular events and psychiatric disorders; shared autonomic substrate.                                                                                                 |
| Renal-Fluid-Electrolyte Axis         | Bidirectional              | Osmoreceptors (hypothalamus SFO/OVLT) → ADH/AVP → renal AQP2 → water retention. RAAS: Ang II → AT1R at SFO/OVLT → thirst + SNS. RVLM: primary sympathetic outflow to renal nerves. Aldosterone: mineralocorticoid effects at brain (MR on hippocampus).                     | RAAS over-activation: hypertension, fluid retention, and concurrent hippocampal MR over-activation → HPA sensitization. Hypernatremia/hyponatremia: acute neurological emergencies with direct osmotic brain effects. Chronic kidney disease: uremic toxins cross BBB → cognitive impairment.                                                              |

Table 1. The ten primary brain-body highways. For detailed signal
inventories, bidirectional feedback loops, and failure modes see
individual system sections (§8–§13).

### §3 — Neurotransmitter and Hormone Origin-Destination-Function Map

The table below lists the primary signaling molecules of the brain-body
system with their origin, brain targets, peripheral targets, and key
computational parameters. Molecules are grouped by class. For full
receptor pharmacology and silo analyses see NeurochemFormula v1.6.
‘Tier’ designations follow the evidence tiers defined in §1 of
individual system papers.

<table>
<colgroup>
<col style="width: 17%" />
<col style="width: 12%" />
<col style="width: 21%" />
<col style="width: 21%" />
<col style="width: 27%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Signal</strong></td>
<td><strong>Origin</strong></td>
<td><strong>Brain Targets &amp; Effect</strong></td>
<td><strong>Peripheral Role</strong></td>
<td><strong>Key Computational Parameters</strong></td>
</tr>
<tr class="even">
<td colspan="5"><strong>Classical Neurotransmitters</strong></td>
</tr>
<tr class="odd">
<td><strong>Acetylcholine (ACh)</strong></td>
<td>Nucleus Basalis (global cortical); Medial Septum (hippocampus). PNS:
NMJ; vagal efferent; autonomic ganglia.</td>
<td>Mode switch: ACh HIGH = encoding mode (CA3 suppressed); ACh LOW =
retrieval mode (CA3 open). Global cortical learning rate. Theta
coherence in hippocampus.</td>
<td>NMJ: neuromuscular transmission. Heart rate (M2 = chronotropy ↓). GI
motility (M3). Glandular secretion. First NT depleted in
Alzheimer’s.</td>
<td><p>learning_rate_global = f(ACh_tone)</p>
<p>encoding_mode = ACh_tone &gt; threshold</p>
<p>theta_coherence[hippocampus]</p>
<p>NMJ_transmission = f(ACh_vesicle_release)</p></td>
</tr>
<tr class="even">
<td><strong>Norepinephrine (NE)</strong></td>
<td>Locus Coeruleus (brain). Adrenal medulla (blood). Sympathetic
postganglionic (periphery).</td>
<td>Phasic: novelty/threat salience tag; LTP threshold lowering at CA1.
Tonic: arousal baseline; SNR sharpening (inverted-U). Delays melatonin
onset (does not suppress). NE_tonic ↓ during sleep → glymphatic
clearance → microglial pruning.</td>
<td>Fight-or-flight: HR ↑, BP ↑, bronchodilation, hepatic glucose ↑.
Splenic NE → cholinergic anti-inflammatory brake modulation. Immune cell
β2-AR: acute priming.</td>
<td><p>NE_phasic = novelty/threat signal</p>
<p>NE_tonic = arousal_baseline</p>
<p>SNR_sharpening = f(NE_tonic) [inverted-U]</p>
<p>melatonin_onset_delay = f(NE_tonic)</p>
<p>glymphatic_clearance when NE_tonic ↓</p></td>
</tr>
<tr class="odd">
<td><strong>Serotonin (5-HT)</strong></td>
<td>Dorsal Raphe Nucleus (brain). Enterochromaffin cells (gut, 90% of
body 5-HT — does NOT cross BBB; tryptophan crosses via LAT1).</td>
<td>Mood stability; impulse control; pain modulation (descending via
dorsal horn). E2 → ERβ on raphe → 5-HT synthesis ↑; MAO-B inhibition →
5-HT clearance ↓.</td>
<td>GI motility (5-HT3/4 on ENS). Platelet aggregation (5-HT uptake →
release at injury). Pulmonary vasoconstriction (5-HT2A). Peripheral 5-HT
does not reach brain.</td>
<td><p>5HT_synthesis_rate = f(tryptophan_BBB, IDO_activity⁻¹)</p>
<p>descending_analgesia_efficiency</p>
<p>mood_stability_parameter</p></td>
</tr>
<tr class="even">
<td><strong>Dopamine (DA)</strong></td>
<td>VTA (mesolimbic/mesocortical). SNpc (nigrostriatal). Arcuate
(tuberoinfundibular).</td>
<td>Reward prediction error (phasic). Motivation (tonic). Working memory
gating (D1 in PFC). Motor sequence execution (nigrostriatal). D2R:
inhibitory autoreceptor + striatal gate.</td>
<td>Tuberoinfundibular: inhibits prolactin. Renal: D1 on proximal tubule
→ Na⁺ excretion. Adrenal: DA precursor to NE.</td>
<td><p>RPE = DA_phasic_burst - prediction</p>
<p>D1_PFC_gain = f(DA_mesocortical)</p>
<p>motor_sequence_fidelity</p>
<p>DA_tonic[VTA] = f(leptin, opioid_tone, E2)</p></td>
</tr>
<tr class="odd">
<td><strong>GABA</strong></td>
<td>Local interneurons everywhere. Projection: striatum → GPe/SNr; BNST
→ amygdala output.</td>
<td>Primary inhibitory. DG: tonic GABA-A (δ-subunit) = sparsity gate;
ALLO-modulated (allopregnanolone). PFC: interneurons gate working memory
loading. Amygdala: ITC cells = fear extinction gate.</td>
<td>None systemically — does not cross BBB. Peripheral GABA receptors on
immune cells (immunomodulatory, poorly characterized).</td>
<td><p>GABA_tonic_inhibition[DG] = f(ALLO_level)</p>
<p>ITC_gate_strength[amygdala]</p>
<p>interneuron_E/I_ratio[PFC]</p></td>
</tr>
<tr class="even">
<td><strong>Glutamate</strong></td>
<td>All excitatory neurons (dominant CNS excitatory NT).</td>
<td>AMPA: fast depolarization. NMDA: coincidence detector for plasticity
(requires pre+post simultaneous). mGluR: modulatory. CA3 recurrent,
Schaffer collateral, perforant path.</td>
<td>Peripheral: enteric sensory neurons. Retinal photoreceptors
(glutamate onto bipolar cells). Taste (umami via mGluR4).</td>
<td><p>NMDA_gate = plasticity_enable condition</p>
<p>Δw = η · NMDA_gate · NE_phasic · (pre·post)</p>
<p>kynurenine_load → QUIN → NMDA_excitotoxicity_risk</p></td>
</tr>
<tr class="odd">
<td colspan="5"><strong>Hormones with Primary Brain
Targets</strong></td>
</tr>
<tr class="even">
<td><strong>Cortisol / GR</strong></td>
<td>Adrenal cortex (zona fasciculata). HPA axis.</td>
<td>GR densest in hippocampus. Acute: LTP threshold ↑, encoding
impaired. Chronic: CA3 dendritic retraction, DG neurogenesis ↓, HPA
brake failure (subiculum GR downregulation → runaway).</td>
<td>Anti-inflammatory (acutely). Gluconeogenesis ↑. Immune suppression.
Protein catabolism (muscle UPS). Bone resorption ↑ (cortisol →
osteoblast suppression).</td>
<td><p>plasticity_suppression[hpc] = cortisol · GR_sensitivity</p>
<p>θ_pre += cortisol · stress_factor</p>
<p>DG_neurogenesis_rate ↓ under chronic cortisol</p></td>
</tr>
<tr class="odd">
<td><strong>Estradiol (E2)</strong></td>
<td>Ovaries (cyclic premenopausal). Adipose aromatase. Brain aromatase
(hippocampus, hypothalamus).</td>
<td>CA1: 1.5–3× LTP gain via ERα/ERβ → AMPA trafficking + spine growth.
DG: BDNF expression ↑ → neurogenesis ↑. Raphe: 5-HT synthesis ↑, MAO-B
↓. vlPAG: descending analgesia efficiency ↑. Amygdala: BLA reactivity
modulation.</td>
<td>Cardiovascular protection (endothelial NO, vasodilation). Bone: OPG
↑ + RANKL ↓ (resorption brake). Immunostimulatory (B-cell, NK cell).
Lipid profile: HDL ↑, LDL ↓.</td>
<td><p>LTP_gain[CA1] = f(E2_level, DHEA_level,
cortisol_suppression⁻¹)</p>
<p>DG_neurogenesis_rate += f(E2→BDNF)</p>
<p>5HT_synthesis_rate ↑ via raphe ERβ</p>
<p>vlPAG_efficiency = f(E2·ERβ)</p></td>
</tr>
<tr class="even">
<td><strong>Testosterone (T)</strong></td>
<td>Testes. Ovaries (partial). Adrenal. Brain aromatase → local E2.</td>
<td>Via aromatase → local E2: hippocampal LTP, CA1 spine density. Direct
AR: spatial memory circuits (parietal, hippocampal geometry), DA
synthesis (T → DA pathway), neuroprotection.</td>
<td>Anabolic: muscle mTOR → protein synthesis; satellite cell
activation. Bone: osteoblast activation. Cardiovascular: RBC production
↑, vasodilation. Immunosuppressive at physiological levels.</td>
<td><p>CA1_spine_density = f(T_level, E2_local)</p>
<p>DA_synthesis_rate[SNpc] partially T-dependent</p>
<p>mTOR_anabolic_gate ↑ under T</p></td>
</tr>
<tr class="odd">
<td><strong>Osteocalcin (ucOC)</strong></td>
<td>Osteoblasts (bone). Undercarboxylated form (ucOC) = bioactive. Rises
with exercise and mechanical loading.</td>
<td>GPR158 on hippocampal neurons: BDNF ↑, monoamine synthesis ↑ (DA,
5-HT, NE). Memory circuits and cognitive function. GPR158 on LC:
potentially modulates NE synthesis (mouse data). Sedentary aging →
osteocalcin ↓ → all four downstream pathways ↓.</td>
<td>GPRC6A on skeletal muscle → mitochondrial gene expression ↑,
exercise capacity ↑. GPRC6A on β-cells → insulin secretion ↑. Energy
metabolism. 2024 MR study: causal link to AD risk via energy
metabolism.</td>
<td><p>osteocalcin_input[hpc] = f(ucOC_circulating)</p>
<p>BDNF_hippocampus += f(GPR158_activation)</p>
<p>monoamine_synthesis ↑ via GPR158</p>
<p>DG_neurogenesis_rate indirect via BDNF</p></td>
</tr>
<tr class="even">
<td><strong>Irisin</strong></td>
<td>Skeletal muscle (FNDC5 cleavage during exercise). Requires Hsp90α
for αVβ5 receptor activation.</td>
<td>αVβ5 integrin on hippocampal neurons → neuroplasticity, resistance
to neurodegeneration. Cryo-EM confirmed 2023. Human observational: lower
in AD and MDD. Tier B mechanism, Tier C clinical causation.</td>
<td>αVβ5 on bone osteocytes → sclerostin modulation → WNT pathway.
Adipose: white-to-beige browning → BAT thermogenesis. Glucose
metabolism. Myokine released proportional to exercise.</td>
<td><p>irisin_input[hpc] = f(irisin_circulating)</p>
<p>hippocampal_neuroplasticity += f(αVβ5_activation)</p>
<p>sclerostin_level[bone] modulated by irisin</p>
<p>adipose_browning = f(irisin)</p></td>
</tr>
<tr class="odd">
<td><strong>Insulin</strong></td>
<td>Pancreatic β-cells. Released in response to blood glucose, GLP-1,
CCK.</td>
<td>Hippocampus: AMPA trafficking, synaptic plasticity, neuroprotection.
Hypothalamus: satiety (overlaps leptin signaling, ARC). Cortex: energy
supply via GLUT4. Brain insulin resistance: LTP impaired, memory
failure.</td>
<td>Primary: glucose uptake into muscle and adipose (GLUT4). Hepatic
glycogen synthesis. Fat storage. Protein synthesis (via mTOR, AMPK
opposition).</td>
<td><p>LTP_gain[hpc] partially gated by brain_insulin_signaling</p>
<p>brain_insulin_resistance_index</p>
<p>AMPA_trafficking_rate = f(insulin)</p>
<p>ARC_satiety_signal (overlaps leptin)</p></td>
</tr>
<tr class="even">
<td><strong>Leptin</strong></td>
<td>Adipose tissue (proportional to fat mass).</td>
<td>Hypothalamus ARC: satiety (POMC activation, NPY/AgRP suppression).
Hippocampus: LTP enhancement, antidepressant effect. VTA: DA tone.
Amygdala: mood regulation.</td>
<td>Satiety signaling to brain — primary role. Reproductive axis:
permissive for GnRH pulsatility (leptin threshold required for puberty
onset). Immune: lymphocyte proliferation ↑.</td>
<td><p>ARC_satiety = f(leptin_level, leptin_resistance_index)</p>
<p>LTP_gain[hpc] partially enhanced by leptin</p>
<p>DA_tone[VTA] = f(leptin_signaling)</p></td>
</tr>
<tr class="odd">
<td><strong>Opioid peptides (β-EP, enkephalin, dynorphin)</strong></td>
<td>Hypothalamus (β-endorphin). Adrenal medulla. Interneurons
throughout. Released by exercise.</td>
<td>vlPAG: μ-opioid → descending analgesia (disinhibit vlPAG → 5-HT/NE
descending). Hypothalamus: GnRH suppression (high opioid load → HPG
shutdown — athlete amenorrhea). Reward: NAcc μ-opioid → hedonic
value.</td>
<td>Immune: opioid receptors on T/B cells, NK cells. Gut: μ-opioid on
ENS → motility ↓ (constipation). Cardiac: brief ischemic preconditioning
via δ-opioid.</td>
<td><p>vlPAG_efficiency = f(E2·ERβ, opioid_tone)</p>
<p>GnRH_pulse_frequency ↓ when opioid_load ↑</p>
<p>NAcc_hedonic_value += f(μ-opioid_activation)</p></td>
</tr>
<tr class="even">
<td><strong>FGF23</strong></td>
<td>Osteocytes (bone). Released in response to phosphate load and high
calcitriol.</td>
<td>No direct GPR in hippocampus confirmed. Indirect: FGF23 → renal
calcitriol suppression → Ca2+/D3 brain effects. Potential direct FGF
receptor in hypothalamus (not fully characterized).</td>
<td>Kidney: suppresses 1α-hydroxylase → calcitriol ↓ → intestinal
Ca2+/phosphate absorption ↓. Renal phosphate excretion ↑. Endocrine
coupling with PTH and vitamin D.</td>
<td><p>FGF23_level = f(phosphate_load, calcitriol_level)</p>
<p>calcitriol_synthesis = f(1α-hydroxylase, FGF23⁻¹)</p>
<p>phosphate_excretion ↑ under FGF23</p></td>
</tr>
<tr class="odd">
<td><strong>GLP-1</strong></td>
<td>L-cells (gut, ileum/colon). Proglucagon-derived. Released by
fat+carbohydrate.</td>
<td>Hypothalamus ARC: suppresses NPY/AgRP (hunger) and activates POMC
(satiety) simultaneously. Vagal afferents: GLP-1R on nodose ganglion →
satiety to NTS. Potential anti-inflammatory and neuroprotective effects
(Tier C in humans).</td>
<td>Pancreatic β-cells: insulin secretion ↑ (glucose-dependent).
α-cells: glucagon ↓. Gastric emptying ↓. Cardiac: cardioprotective in
RCTs (LEADER, SUSTAIN-6). GLP-1R agonists: lean mass loss 25–40% of
weight lost.</td>
<td><p>ARC_satiety += f(GLP-1R_activation)</p>
<p>vagal_satiety_signal = f(nodose_GLP1R)</p>
<p>insulin_secretion = f(GLP1, glucose)</p></td>
</tr>
</tbody>
</table>

Table 2. Signal origin-destination-function map (selected). For full NT
formulas, receptor pharmacology, and parameter ranges see
NeurochemFormula v1.6.

### §4 — The Hormonal Brain: Two Timescales of Action

Hormones act on the brain through two fundamentally different mechanisms
operating on distinct timescales, and confusing them accounts for many
misunderstandings of hormonal brain effects in clinical medicine.

Fast membrane effects (minutes): Many steroids — E2, progesterone,
cortisol, DHEA, testosterone, and their metabolites — act directly on
membrane receptors including ligand-gated ion channels (GABA-A: ALLO is
a positive allosteric modulator), G-protein-coupled receptors
(GPR30/GPER for E2), and receptor tyrosine kinases. These produce
effects within seconds to minutes: E2 can potentiate NMDA receptor
currents within 5 minutes via non-genomic ERβ → PI3K → AMPA insertion.
Cortisol can raise the LTP threshold within 15–30 minutes via
membrane-bound GR. ALLO produces immediate anxiolytic and sedative
effects by potentiating GABA-A tonic conductance at the δ-subunit
\[11\].

Slow genomic effects (hours to days): Classical steroid receptor
signaling — receptor binds ligand in cytoplasm, translocates to nucleus,
binds hormone response elements, modulates gene expression — produces
structural synaptic changes over hours to days. E2-driven CA1 spine
density changes require 12–24 hours. Cortisol-driven CA3 dendritic
retraction requires days to weeks of sustained elevation. BDNF
upregulation via E2-ERα binding to BDNF promoter requires hours \[12\].
This is why acute hormone changes (e.g., post-surgical ovariectomy)
produce immediate cognitive and mood effects through the fast pathway,
while chronic hormone deprivation produces progressive structural brain
changes through the slow pathway.

Clinical implication: Standard endocrinology measures are optimized for
the genomic pathway — they measure hormone levels sufficient for
reproductive organ effects, which require genomic signaling. Brain
fast-pathway effects may occur at lower concentrations and with
different receptor sensitivity than peripheral reproductive effects.
This means normal-range hormone levels for gynecological purposes may
not be adequate for brain function in all individuals \[11,12\].

### §5 — Neurosteroids: The Brain’s Internal Hormone Factory

The brain is not merely a target for peripheral hormones — it
synthesizes steroid hormones (neurosteroids) independently of the gonads
and adrenal glands, from cholesterol, using the same enzymatic machinery
as peripheral endocrine organs. This local synthesis provides a second,
regionally heterogeneous hormone source that standard blood panels
cannot measure \[13,14\].

The neurosteroid synthesis cascade begins with StAR protein importing
cholesterol into inner mitochondrial membrane → CYP11A1 converts to
pregnenolone → branching into multiple downstream steroids via
region-specific enzyme expression. Key brain-synthesized steroids:
allopregnanolone (ALLO) from progesterone via 5α-reductase + 3α-HSD;
DHEA and DHEA-S from pregnenolone via CYP17A1; estradiol from
testosterone via aromatase (expressed in hippocampus, hypothalamus,
amygdala, cortex in both sexes); T from androstenedione via 17β-HSD.

ALLO: The most potent positive allosteric modulator of GABA-A receptors
in the brain. Acts specifically at the extrasynaptic δ-subunit (tonic
conductance) in the dentate gyrus — this subunit is insensitive to
benzodiazepines. ALLO collapse (postpartum: acute progesterone
withdrawal; perimenopause: progesterone decline) → DG hyperexcitability
→ pattern separation degrades → anxiety, intrusive memory risk.
Brexanolone (synthetic ALLO IV) is FDA-approved for postpartum
depression and targets this mechanism directly \[37\].

DHEA and DHEA-S: Act as endogenous partial anti-glucocorticoid buffers
in hippocampus (DHEA partially offsets GR-mediated LTP suppression).
DHEA also acts via NMDA receptor facilitation and σ1 receptor. Peak at
age 25, decline to 10–20% of peak by age 70 — the most consistent aging
biomarker in the endocrine system. Brain DHEA is partially independent
of adrenal DHEA, meaning peripheral DHEA-S measurement may not reflect
local brain DHEA levels \[17\].

Local E2 from brain aromatase: Hippocampal aromatase produces E2 within
synaptic terminals in response to NMDA activation —
experience-dependent, rapid, and completely invisible to serum E2
panels. Brain-local E2 may explain why cognitive benefits of HRT are
formulation-, timing-, and dose-sensitive: the brain’s own E2 production
is not captured by standard monitoring \[13\].

## Part II — The Peripheral Architecture

### §6 — The Endocrine System: Five Coupled Feedback Axes

The endocrine system operates as five coupled negative-feedback axes
(HPA, HPG, HPT, HPA-metabolic, and somatotropic/IGF-1) whose cross-axis
interactions are frequently more clinically significant than any
single-axis failure. Complete FQ decompositions and cross-axis coupling
diagrams are in EndocrineSystem v1.1.

|                            |                                                                                                                                                                                                                        |                                                                                                                                                                                                                                                                     |                                                                                                                                                                                                                                                            |
|----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Axis**                   | **Architecture**                                                                                                                                                                                                       | **Brain Interface**                                                                                                                                                                                                                                                 | **Key Cross-Axis Coupling**                                                                                                                                                                                                                                |
| **HPA**                    | PVN → CRH → anterior pituitary → ACTH → adrenal cortex → cortisol; feedback via hippocampus GR (subiculum brake) + pituitary GR.                                                                                       | GR most dense in hippocampus; LTP suppression, CA3 dendritic retraction, DG neurogenesis suppression under chronic activation. PVN receives amygdala (threat), hippocampus (context), PFC (cognitive appraisal) inputs.                                             | Cortisol → HPT: suppresses D1/D2 (T4→T3 conversion) → local brain T3 ↓ despite normal TSH. Cortisol → HPG: GnRH pulse suppression at high levels. Cortisol → Metabolic axis: hepatic gluconeogenesis ↑, insulin resistance ↑.                              |
| **HPG**                    | GnRH pulse (arcuate kisspeptin neurons) → FSH/LH → gonads → E2/T/P4/inhibin; ovarian E2 surges → LH surge (positive feedback). Frequency-encoded: slow pulses → FSH; fast → LH.                                        | E2/T → hippocampal LTP, CA1 spine density, DG neurogenesis. P4/ALLO → DG GABA tonic (sparsity gate). Raphe ERβ → 5-HT synthesis. vlPAG ERβ → descending analgesia. Amygdala: OTR sensitivity (9th arm of E2 withdrawal cascade).                                    | HPG → immune: E2 immunostimulatory, T immunosuppressive — explains female autoimmune preponderance. HPG → HPA: sex hormones modulate GR sensitivity. HPG → cardiovascular: E2 endothelial protection.                                                      |
| **HPT**                    | TRH (PVN) → TSH (anterior pituitary) → T4 (thyroid) → peripheral D1 or brain D2 (regionally heterogeneous) → T3 active. D3 inactivates T3 to rT3 (inactive).                                                           | T3 is the active form — brain D2 converts T4 to T3 locally in tanycytes, astrocytes. Each brain region has independent T3 regulated by local deiodinase expression. T3 deficiency: cognitive slowing, depression, psychomotor impairment. Critical for myelination. | HPA → HPT: sustained cortisol suppresses D1/D2 → T3 ↓ even with normal TSH and T4. DIO1 polymorphism (T92A): impaired T4→T3 → suboptimal brain T3 on levothyroxine monotherapy; T3/T4 combination may benefit carriers.                                    |
| **Metabolic / Pancreatic** | Blood glucose → β-cell Ca2+ oscillation (KATP channel mechanism) → pulsatile insulin secretion. GLP-1, GIP (incretins) potentiate glucose-stimulated insulin release. Glucagon (α-cells) opposes.                      | Brain insulin: hippocampal LTP, AMPA trafficking (neuroprotective), satiety signaling (ARC). Brain insulin resistance: LTP impairment, memory failure. T2D patients: 2× AD risk — both share amyloid precursor processing via insulin-degrading enzyme.             | Insulin → HPG: insulin required for normal GnRH pulsatility (PCOS: hyperinsulinemia → androgen excess → HPG dysregulation). Insulin → HPA: cortisol → hepatic gluconeogenesis ↑; insulin resistance and cortisol elevation co-occur in metabolic syndrome. |
| **Somatotropic / IGF-1**   | GHRH/somatostatin (hypothalamus) → GH (anterior pituitary, pulsatile overnight) → IGF-1 (liver primary; also brain, muscle, bone local synthesis). GH/IGF-1 peaks in adolescence; declines 14% per decade from age 30. | IGF-1 crosses BBB via LRP1/receptor-mediated transcytosis. Hippocampus: DG neurogenesis (exercise-dependent IGF-1 rise → BDNF expression). Neuroprotection: insulin/IGF-1 signaling overlap. Muscle-brain: exercise → muscle IGF-1 → brain BDNF.                    | GH/IGF-1 → musculoskeletal: mTOR → muscle protein synthesis; osteoblast activation → bone formation. GH/IGF-1 decline with aging parallels sarcopenia, DG neurogenesis reduction, and osteocalcin decline — a coherent aging axis.                         |

Table 3. Five endocrine axes with brain interfaces and cross-axis
couplings. Full FQ decompositions, feedback equations, and failure
cascades in EndocrineSystem v1.1.

### §7 — The Peripheral Nervous System: ANS, ENS, and Somatic PNS

The peripheral nervous system divides into three functionally distinct
divisions, each with dedicated brain interfaces. Together they
constitute the physical wiring of the brain-body bidirectional highways.
Full FQ decompositions, sub-structure maps, and Rust struct
implementations in PeripheralMap_ANS_v1_0, PeripheralMap_ENS_v1_0, and
PeripheralMap_SomaticPNS_DRG_NMJ_v1_0.

**7.1 Autonomic Nervous System**

The ANS is the real-time bidirectional communication wire between the
brain and every organ. The sympathetic division (T1–L2 preganglionic →
paravertebral/prevertebral ganglia → all organs) drives the
fight-or-flight response and sets baseline organ tone via tonic NE
release. The parasympathetic division, dominated by the vagus nerve (CN
X), provides the primary afferent reporting pathway: 80–90% of vagal
fibers are afferent, carrying gut mechano/chemoreceptor signals,
baroreceptor input, pulmonary stretch, and immune cytokine signals to
the NTS (first brainstem relay). The ANS is not an axis in the HPA/HPG
sense — it operates in real time (milliseconds to seconds) without a
pituitary relay.

The cholinergic anti-inflammatory reflex: efferent vagal fibers release
ACh at the splenic nerve → catecholamine release from splenic T cells →
α7 nAChR on macrophages → TNF-α suppression. This is the brain’s primary
real-time immune modulation pathway. Vagal nerve stimulation
therapeutically activates this reflex in treatment-resistant RA and IBD.
Adrenal medulla = modified postganglionic SNS neuron: produces
epinephrine (80%) and NE (20%) directly into blood — the humoral arm of
the sympathetic stress response.

Heart rate variability (HRV) is the most accessible non-invasive measure
of real-time ANS balance and brain-body integration state. Low HRV =
reduced parasympathetic tone = impaired cholinergic anti-inflammatory
reflex + impaired emotional regulation + impaired baroreflex
flexibility. HRV reduction precedes both cardiovascular events and
psychiatric decompensation, reflecting shared autonomic substrate.

**7.2 Enteric Nervous System**

The ENS contains approximately 500 million neurons organized in two
plexuses: Meissner’s (submucosal; secretion and blood flow) and
Auerbach’s (myenteric; motility). It operates with substantial autonomy
from the CNS via local reflex arcs, but communicates bidirectionally
with the brain via vagal afferents (gut state → NTS), spinal afferents
(pain, nociception via DRG), and the portal circulation (gut-derived
metabolites and hormones). The ENS is embryologically derived from vagal
and sacral neural crest cells (the same neural crest population that
generates all peripheral ganglia, distinct from the neuroepithelium of
the neural tube that generates CNS neurons) — it is a true second
nervous system, not peripheral sensory organs. Gut 5-HT (90% of body
total, from enterochromaffin cells) acts on intrinsic ENS reflexes and
vagal afferents but does not cross the BBB; tryptophan (serotonin
precursor) does cross via LAT1 transporter, and is the rate-limiting
step for brain 5-HT synthesis.

**7.3 Somatic Peripheral Nervous System**

The somatic PNS provides motor output (lower motor neurons → NMJ →
skeletal muscle) and sensory input (DRG → dorsal horn →
spinothalamic/DCML tracts → thalamus → sensory cortex). Dorsal root
ganglia (DRG) are the primary cell bodies for all peripheral sensory
modalities: nociception (Aδ/C fibers), proprioception (Ia/Ib/II fibers),
mechanoreception (Aβ fibers), and thermoreception. Substance P and CGRP
from DRG neurons drive neurogenic inflammation — the peripheral arm of
the pain amplification cascade. The NMJ is not merely a relay; it is a
bidirectional synaptic junction where retrograde signals (NGF, CNTF)
flow from muscle to motor neuron, regulating motor neuron survival and
plasticity.

## Part III — Body Systems: Architecture and Brain Interface

Each organ system section below provides: the system’s primary
computational role, its brain interface (signals in/out and primary
brain targets), key coupling parameters, and cross-reference to the
detailed map. These sections are synthesis entries, not full system
treatments. Full FQ decompositions, failure cascades, and Rust struct
implementations are in the individual Organ System maps
(OrganSystem\_\*.md v1.0 series) and the system papers
(CardiovascularRenal v1.3, MetabolicGut v1.1, Immunological v0.8,
Respiratory v1.2, Musculoskeletal v1.0).

### §8 — Cardiovascular-Renal System

<table>
<colgroup>
<col style="width: 19%" />
<col style="width: 80%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Cardiovascular-Renal — §8</strong></td>
<td></td>
</tr>
<tr class="even">
<td><strong>Computational role</strong></td>
<td>Pressure regulation (MAP homeostasis via baroreflex),
volume-electrolyte balance (RAAS-renal axis), and cardiac output
optimization. Dual endocrine organs: heart (BNP/ANP = natriuretic
peptides), kidney (renin = RAAS initiator; erythropoietin; calcitriol
activation).</td>
</tr>
<tr class="odd">
<td><strong>Brain interface (body → brain)</strong></td>
<td><p>MAP (baroreceptors: carotid sinus, aortic arch) → CN IX/X → NTS →
CVLM/RVLM: real-time cardiovascular regulation; primary input to
autonomic balance</p>
<p>BNP (cardiac wall stress) → circumventricular organs → diuresis and
natriuresis signaling</p>
<p>Ang II (RAAS) → AT1R at SFO/OVLT → hypothalamus: thirst + SNS
activation; concurrent plasma Ang II rise → aldosterone → Na+/volume
retention</p>
<p>HRV: non-invasive real-time proxy for vagal-brain integration
state</p>
<p>Ischemic pain (cardiac C-fibers) → spinal → thalamus → insula
(interoceptive representation of cardiac state)</p></td>
</tr>
<tr class="even">
<td><strong>Brain output (brain → body)</strong></td>
<td><p>PVN → IML → stellate ganglion (SNS cardiac drive: HR ↑,
contractility ↑)</p>
<p>PAG → nucleus ambiguus (vagal modulation of cardiac rate)</p>
<p>HPA cortisol → adrenal medulla → epinephrine (humoral stress
response)</p>
<p>Hypothalamus osmoreceptors → ADH/AVP → renal AQP2 → water
reabsorption</p>
<p>RVLM: primary sympathetic outflow to renal nerves (renal vascular
tone, renin secretion)</p></td>
</tr>
<tr class="odd">
<td><strong>Key parameters</strong></td>
<td><p>MAP: target setpoint maintained by baroreflex reflex arc (RVLM
gain ±10 mmHg); renal autoregulation extends 60–180 mmHg</p>
<p>HRV: LF/HF ratio = sympathovagal balance; SDNN = overall ANS
flexibility</p>
<p>RAAS activation index = f(renin, Ang II, aldosterone)</p>
<p>vagal_tone = f(HRV, RSA amplitude)</p>
<p>RIGHT insular cortex lesion → cardiac arrhythmias (direct cardiac
autonomic control)</p></td>
</tr>
<tr class="even">
<td><strong>Cross-reference</strong></td>
<td><p>CardiovascularRenal v1.3 (system paper);
OrganSystem_Cardiovascular_v1_0.md (detailed map)</p>
<p>BrainMap_RVLM_preBotC_SCN_RapheMedullary (cardiovascular control
center)</p>
<p>BrainMap_NTS (first relay for all cardiovascular afferents)</p>
<p>BrainMap_Insula (interoceptive representation)</p></td>
</tr>
</tbody>
</table>

### §9 — Metabolic-Gut System

<table>
<colgroup>
<col style="width: 19%" />
<col style="width: 80%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Metabolic-Gut — §9</strong></td>
<td></td>
</tr>
<tr class="even">
<td><strong>Computational role</strong></td>
<td>Blood glucose homeostasis (pancreatic islet oscillation, hepatic
glucose production/storage, muscle GLUT4 uptake), gut-derived satiety
and hunger signaling, and hepatic detoxification + metabolic processing.
The metabolic system is simultaneously a fuel-supply system and a
brain-state signaling system.</td>
</tr>
<tr class="odd">
<td><strong>Brain interface (body → brain)</strong></td>
<td><p>L-cell GLP-1 + K-cell GIP (postprandial) → vagal nodose ganglion
GLP-1R → NTS → satiety; also direct BBB-crossing at ARC</p>
<p>Ghrelin (gastric fundus, fasting) → ARC/VTA/hippocampus: hunger, food
craving, DG neurogenesis ↑ at moderate levels</p>
<p>Leptin (adipose, proportional to fat mass) → ARC POMC/NPY → satiety;
hippocampus LTP ↑; VTA DA tone</p>
<p>Insulin (pancreatic β-cells) → hippocampus: AMPA trafficking, LTP;
ARC: satiety signal overlap with leptin</p>
<p>Gut microbiome → SCFA production → vagal afferents; tryptophan
metabolism → BBB LAT1 → raphe 5-HT synthesis</p>
<p>Hepatic vagal afferents → NTS: glucose and lipid sensing from portal
circulation</p></td>
</tr>
<tr class="even">
<td><strong>Brain output (brain → body)</strong></td>
<td><p>Hypothalamus ARC NPY/AgRP: orexigenic drive → food-seeking
behavior</p>
<p>VTA DA → hedonic eating reward (D2R downregulation with chronic junk
food → overconsumption cycle)</p>
<p>HPA cortisol → hepatic gluconeogenesis ↑; insulin resistance ↑</p>
<p>Vagal efferents → pancreas (parasympathetic → insulin secretion at
cephalic phase); gut motility regulation</p></td>
</tr>
<tr class="odd">
<td><strong>Key parameters</strong></td>
<td><p>ARC_satiety = f(leptin, insulin, GLP-1, ghrelin⁻¹)</p>
<p>brain_insulin_resistance_index (T2D → elevated → hippocampal LTP
impaired)</p>
<p>DA_tonic[VTA] = f(leptin, opioid_tone, E2)</p>
<p>DG_neurogenesis_rate += f(ghrelin_moderate)</p>
<p>tryptophan_availability[BBB] = f(microbiome_health,
IDO_activity⁻¹)</p></td>
</tr>
<tr class="even">
<td><strong>Cross-reference</strong></td>
<td><p>MetabolicGut v1.1 (system paper); OrganSystem_GI_v1_0.md;
OrganSystem_HepaticMetabolic_v1_0.md</p>
<p>BrainMap_Hypothalamus (ARC: hunger/satiety circuits)</p>
<p>BrainMap_VTA (DA: hedonic eating, D2R downregulation)</p>
<p>PeripheralMap_ENS_v1_0 (enteric nervous system detail)</p></td>
</tr>
</tbody>
</table>

### §10 — Immune System

<table>
<colgroup>
<col style="width: 19%" />
<col style="width: 80%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Immune System — §10</strong></td>
<td></td>
</tr>
<tr class="even">
<td><strong>Computational role</strong></td>
<td>Pathogen detection and elimination (innate: pattern recognition via
TLRs/NLRs; adaptive: T/B cell clonal expansion), tissue damage
surveillance (complement, mast cells), and cancer immunosurveillance. In
the CNS context: microglia (CNS macrophages) + perivascular macrophages
+ astrocyte reactivity constitute the neuroimmune compartment.</td>
</tr>
<tr class="odd">
<td><strong>Brain interface (body → brain)</strong></td>
<td><p>IL-1β, TNF-α, IL-6 (peripheral cytokines) → two routes:
circumventricular organs (area postrema, SFO — outside BBB) OR vagal
C-fibers → NTS → brainstem; both → sickness behavior (programmed,
adaptive)</p>
<p>PGE2 (peripheral COX-2 → prostaglandins) → hypothalamus EP3/4
receptors → body temperature setpoint ↑ (fever generation)</p>
<p>Kynurenine pathway: IDO activation (inflammation) → tryptophan →
kynurenine → QUIN (NMDA excitotoxicity) vs KYNA (neuroprotective); net
ratio determines hippocampal damage risk</p>
<p>Immune-to-brain via LC: NE surge from LC → acute inflammatory
priming; chronic microglial activation downstream</p></td>
</tr>
<tr class="even">
<td><strong>Brain output (brain → body)</strong></td>
<td><p>HPA cortisol → systemic immunosuppression (glucocorticoid
receptor on every immune cell)</p>
<p>Cholinergic anti-inflammatory reflex: vagal efferents → splenic nerve
→ α7 nAChR on macrophages → TNF-α suppression</p>
<p>SNS → splenic NE → acute immune priming (stress immune response)</p>
<p>Hypothalamus fever center: PVN CRH → ANS → thermogenesis; PAG →
vasodilation/constriction</p></td>
</tr>
<tr class="odd">
<td><strong>Key parameters</strong></td>
<td><p>cytokine_load = f(IL-1β, TNF-α, IL-6)</p>
<p>sickness_behavior = f(cytokine_load, PGE2, vagal_activation)</p>
<p>kynurenine_load → QUIN → NMDA_excitotoxicity_risk[hippocampus]</p>
<p>microglial_M1_M2_ratio (DAM = TREM2-dependent neuroprotective; DIM =
inflammatory)</p>
<p>activation_ceiling[cortex] ↓ during immune activation (metabolic
redirection)</p></td>
</tr>
<tr class="even">
<td><strong>Cross-reference</strong></td>
<td><p>Immunological v0.8 (system paper); OrganSystem_Immune_v1_0.md
(detailed map)</p>
<p>BrainMap_Glymphatic_BBB_Oligodendrocytes_CSF (microglia, BBB,
neuroinflammation)</p>
<p>BrainMap_Hypothalamus (fever center, HPA-immune axis)</p>
<p>BrainMap_LC (NE → immune modulation)</p></td>
</tr>
</tbody>
</table>

### §11 — Respiratory System

<table>
<colgroup>
<col style="width: 19%" />
<col style="width: 80%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Respiratory System — §11</strong></td>
<td></td>
</tr>
<tr class="even">
<td><strong>Computational role</strong></td>
<td>Gas exchange (O2/CO2 at alveoli), acid-base regulation (primary
CO2/pH buffer), and arousal-state coupling (respiratory rhythm is the
master pacemaker for brainstem oscillations in non-REM sleep). The
respiratory system has direct mechanical coupling to brain state:
respiratory rate and depth modulate cortical oscillatory activity via
brainstem → ascending arousal systems.</td>
</tr>
<tr class="odd">
<td><strong>Brain interface (body → brain)</strong></td>
<td><p>Carotid body chemoreceptors (PaO2 ↓, PaCO2 ↑, pH ↓) → CN IX/X →
NTS; hypoxia → carotid body → NTS → preBötC → breathing depth/rate ↑</p>
<p>Pulmonary stretch receptors (Hering-Breuer reflex) → vagal afferents
→ NTS → inspiration terminated</p>
<p>Dyspnea: NTS → insula (interoceptive); parabrachial nucleus →
amygdala (affective component of breathlessness)</p>
<p>preBötzinger complex (RVLM master synthesis map): coupled to arousal
and sleep/wake state; breathing rhythm entrains cortical oscillations
(respiratory-cortical coupling documented 2017+)</p></td>
</tr>
<tr class="even">
<td><strong>Brain output (brain → body)</strong></td>
<td><p>preBötC → phrenic nerve (C3-C5) → diaphragm (primary driver)</p>
<p>Motor cortex: voluntary breathing override (bypasses preBötC for
speech, breath-holding, emotional sighing)</p>
<p>Hypothalamus: thermoregulatory hyperventilation; hypoxia → HPA
activation (altitude, apnea)</p>
<p>XII nucleus → genioglossus (upper airway patency): OSA
pathophysiology node</p></td>
</tr>
<tr class="odd">
<td><strong>Key parameters</strong></td>
<td><p>RR (respiratory rate): direct coupling to cortical oscillations
and arousal state</p>
<p>PaCO2_setpoint = RTN sensitivity (CO2 detector); CBF = f(PaCO2) — CO2
is primary cerebrovascular dilator</p>
<p>OSA: intermittent hypoxia → LC activation → NE_tonic ↑ → sleep
fragmentation; HIF-1α → inflammatory cascade</p>
<p>respiratory-cortical coupling: nasal breathing vs mouth breathing:
distinct cortical oscillation profiles (piriform/olfactory cortex
entrained by nasal airflow)</p></td>
</tr>
<tr class="even">
<td><strong>Cross-reference</strong></td>
<td><p>Respiratory v1.2 (system paper); OrganSystem_Respiratory_v1_0.md
(detailed map)</p>
<p>BrainMap_RVLM_preBotC (preBötzinger complex: respiratory rhythm
generator)</p>
<p>BrainMap_Insula (dyspnea interoception)</p>
<p>BrainMap_PAG (voluntary breathing, sighing)</p></td>
</tr>
</tbody>
</table>

### §12 — Musculoskeletal System: Exercise Endocrine Architecture

<table>
<colgroup>
<col style="width: 19%" />
<col style="width: 80%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Musculoskeletal System — §12</strong></td>
<td></td>
</tr>
<tr class="even">
<td><strong>Computational role</strong></td>
<td>Force generation and locomotion (primary function), plus endocrine
transduction of behavioral inputs (exercise, mechanical loading) into
distributed biological age signals. Skeletal muscle: largest metabolic
organ (30–40% body mass; 70% insulin-stimulated glucose uptake);
secretes myokines during contraction. Bone: endocrine organ secreting
osteocalcin (GPR158 in brain) and FGF23 (renal phosphate
regulation).</td>
</tr>
<tr class="odd">
<td><strong>Brain interface (body → brain)</strong></td>
<td><p>Osteocalcin (ucOC, bone osteoblasts) → GPR158 on hippocampal
neurons: BDNF ↑, monoamine synthesis ↑ (DA, 5-HT, NE), autophagy ↑.
Exercise → mechanical loading → osteocalcin ↑. Sedentary aging →
osteocalcin ↓ → hippocampal BDNF ↓. [Tier B mouse causal; Tier C human
clinical magnitude]</p>
<p>Irisin (muscle FNDC5 cleavage during exercise, requires Hsp90α for
αVβ5 receptor activation) → αVβ5 integrin on hippocampal neurons:
neuroplasticity, resistance to neurodegeneration. Cryo-EM confirmed
2023. Lower in AD and MDD observationally. [Tier B]</p>
<p>Peripheral BDNF (muscle pro-BDNF, type I fibers) → cleavage to mature
BDNF in circulation → BBB → TrkB on hippocampal/DG neurons:
neurogenesis, synaptogenesis, LTP. Lactate infusion augments this
response in humans (2024). [Tier B]</p>
<p>Lactate (high-intensity exercise, blood 4–10 mM) → MCT1/2 → BBB →
HCAR1: cerebral angiogenesis. Hippocampal neurons: SIRT1–PGC-1α–FNDC5 →
BDNF gene expression. Chronic training → cerebrovascular reserve ↑.
[Tier B acute; Tier C direct hippocampal causal]</p>
<p>AMPK under-stimulation (inactivity) → sarcopenia → reduced bone
mechanical loading → osteocalcin ↓ → GPR158 signaling ↓ (sedentary aging
cascade, Tier A individual steps)</p></td>
</tr>
<tr class="even">
<td><strong>Brain output (brain → body)</strong></td>
<td><p>Motor cortex + spinal cord: voluntary movement generation;
corticospinal tract. SMA: movement sequence planning</p>
<p>Cerebellum: motor coordination, error correction, timing; receives
proprioceptive input from DRG via spinocerebellar tracts</p>
<p>Hypothalamus: GH/IGF-1 pulsatile release (overnight) → muscle protein
synthesis + bone formation</p>
<p>D2R (striatum): motivational salience of exercise; D2R declines with
aging → reduced exercise motivation (Tier B; Volkow 1998 PET)</p></td>
</tr>
<tr class="odd">
<td><strong>Key parameters</strong></td>
<td><p>osteocalcin_input[hippocampus] = f(ucOC_circulating)</p>
<p>irisin_input[hippocampus] = f(irisin_circulating)</p>
<p>BDNF_peripheral = f(exercise_duration, muscle_type_I_fraction)</p>
<p>lactate_hippocampal = f(blood_lactate, exercise_intensity)</p>
<p>cerebrovascular_reserve (chronic training parameter; range
0.5–1.5)</p>
<p>DG_neurogenesis_rate = f(BDNF[all_sources], IGF1, cortisol⁻¹)</p>
<p>D2R_density[striatum] ↓ with aging →
exercise_motivation_modifier</p></td>
</tr>
<tr class="even">
<td><strong>Cross-reference</strong></td>
<td><p>Musculoskeletal v1.0 (system paper);
OrganSystem_Musculoskeletal_v1_0.md (organ map)</p>
<p>BrainMap_Hippocampus_v2_1.md (four-channel brain interface; DG
neurogenesis; SILO-HPC-7)</p>
<p>BrainMap_VTA (DA: exercise reward motivation)</p>
<p>BrainMap_Cerebellum (motor coordination)</p>
<p>§18 below: Exercise as Endocrine Architecture (dedicated
section)</p></td>
</tr>
</tbody>
</table>

### §13 — Integumentary, Hepatic, and Renal Supplementary Brain
Couplings

The integumentary, hepatic, and renal systems have brain couplings not
fully captured by the highway table. Brief summaries below; full
treatments in OrganSystem_Integumentary_v1_0.md,
OrganSystem_HepaticMetabolic_v1_0.md, and OrganSystem_Renal_v1_0.md.

**Integumentary System**

The skin is a peripheral HPA axis in its own right: keratinocytes
express CRH, ACTH, and POMC; local cortisol production modulates skin
barrier function and inflammatory responses independently of systemic
HPA. The skin-brain axis operates via: (1) sensory afferents (DRG →
dorsal horn → thalamus → S1/insula: touch, temperature, pain, itch); (2)
neurogenic inflammation (SP/CGRP from sensory neurons → mast cell
degranulation → local inflammatory cascade); (3) UV → vitamin D
synthesis in skin → systemic D3 → brain VDR (widespread expression;
neuroprotective). Stress → CRH → mast cell activation in skin: the
neurogenic inflammation link between psychological stress and
eczema/psoriasis exacerbations.

**Hepatic-Metabolic System**

The liver is the primary metabolic clearance and glucoregulation organ
with three brain interfaces: (1) hepatic vagal afferents detect portal
glucose and lipid levels → NTS → ARC satiety/hunger circuits
(pre-gastric satiety signaling); (2) cortisol → hepatic gluconeogenesis
↑ (PEPCK, G6Pase upregulation) — the primary mechanism of stress-induced
hyperglycemia; (3) bile acid signaling: FXR/TGR5 receptors on hepatic
vagal afferents modulate GLP-1 secretion and gut-brain signaling.
Ammonia (hepatic encephalopathy): BBB-crossing toxin → astrocyte
swelling → cerebral edema. Hepatic CYP450 enzymes metabolize neuroactive
steroids and drugs with CNS effects.

**Renal System**

Beyond the RAAS-brain axis (§2), the kidney–brain interface includes:
(1) erythropoietin (EPO) → EPO receptors in hippocampus and cortex
(neuroprotective signaling, separate from erythropoietic role — Tier B
in rodents, less characterized in humans); (2) FGF23 → renal
1α-hydroxylase suppression → calcitriol ↓ → vitamin D-VDR brain
signaling altered; (3) uremic toxins in CKD (indoxyl sulfate, p-cresol)
cross BBB → microglial activation → cognitive impairment; (4)
aldosterone (MR on hippocampus): while classically renal,
mineralocorticoid receptors in hippocampus regulate HPA sensitivity and
GR/MR ratio determines stress response set point.

## Part IV — Body State → Brain State

### §14 — Hormones Across the Lifespan: Brain Consequences at Every
Stage

<table>
<colgroup>
<col style="width: 17%" />
<col style="width: 26%" />
<col style="width: 56%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Stage</strong></td>
<td><strong>Hormonal Profile</strong></td>
<td><strong>Primary Brain Consequences</strong></td>
</tr>
<tr class="even">
<td>Fetal / Neonatal (conception – ~2 years)</td>
<td>Testosterone surge (male fetus, weeks 8–24). E2 from maternal
circulation + local aromatization. T3 critical from conception. Neonatal
T surge (male): weeks 1–6 postnatal. Allopregnanolone: high in fetal
brain.</td>
<td><p>T organizational effects: establishes sexually dimorphic
structures permanently (SDN-POA, BNST, amygdala, corpus callosum).
Irreversible after critical period.</p>
<p>ALLO in fetal brain: GABA is EXCITATORY in immature neurons (NKCC1
Cl⁻ transporter dominates over KCC2). ALLO drives trophic neuronal
growth and cortical migration. Switch from NKCC1 to KCC2 dominance
occurs around birth.</p>
<p>T3 deficiency before age 3: irreversible intellectual disability. No
catch-up. Newborn screening exists for this reason.</p></td>
</tr>
<tr class="odd">
<td>Childhood (2–10 years)</td>
<td>Low sex hormones (pre-adrenarche). Adrenarche begins ~6–9 years
(girls ~6–8, boys ~7–9): DHEA/DHEA-S rise from adrenal. GH/IGF-1 active
for growth. T3 for continued myelination.</td>
<td><p>DHEA rise from adrenarche: associated with improved executive
function and social cognition — neurosteroid maturation prior to gonadal
puberty.</p>
<p>Myelination ongoing through childhood; T3 deficiency continues to
impact WM development.</p>
<p>Critical period plasticity windows: language (Broca’s/Wernicke’s),
binocular vision (visual cortex), emotional regulation (PFC-amygdala
connectivity).</p></td>
</tr>
<tr class="even">
<td>Puberty (girls ~8–16; boys ~10–18)</td>
<td>GnRH pulses reactivate HPG: E2 rises in females, T rises in males.
Adrenal DHEA ↑. GH/IGF-1 surge (growth spurt). ALLO rises with
progesterone.</td>
<td><p>E2/T → hippocampal plasticity reorganization: spatial vs verbal
cognitive patterns emerge.</p>
<p>Adolescent brain is not merely an immature adult brain: PFC
development lags limbic maturation by ~10 years — peak limbic reactivity
before executive control is online. Reward sensitivity peaks (VTA/NAcc).
Peer social reward value peaks. Risk-taking behavior is normative, not
pathological.</p>
<p>Early-life adversity during puberty → accelerated hippocampal aging
(epigenetic mechanisms).</p></td>
</tr>
<tr class="odd">
<td>Peak reproductive years (20–40)</td>
<td>E2 cyclic (premenopausal females). T stable (males). P4/ALLO cyclic.
DHEA plateau then gradual decline from ~25. GH/IGF-1 peak then gradual
decline.</td>
<td><p>E2 cyclic variation: hippocampal encoding efficiency varies with
menstrual phase; verbal memory peaks at mid-cycle E2 maximum.</p>
<p>ALLO cyclic: DG GABA tonic varies across cycle; premenstrual DG
hyperexcitability correlates with PMDD in ALLO-sensitive
individuals.</p>
<p>Peak neuroplasticity, neurogenesis rates, and cognitive reserve. This
is when exercise, sleep, and stress management most efficiently build
long-term cognitive reserve.</p></td>
</tr>
<tr class="even">
<td>Perimenopause / Menopause (~40–55, female)</td>
<td>E2 erratic → near zero. P4 drops earlier (ovulatory cycles first to
fail). FSH rises. ALLO falls with P4. DHEA already declining since 25.
T: ovarian T declines ~50% at menopause.</td>
<td><p>Hippocampus: E2 withdrawal → LTP_gain[CA1] ↓. Memory complaints
at perimenopause are neurobiologically real. ALLO collapse → DG
hyperexcitability concurrent with cortisol elevation → dual DG
degradation (dual DG degradation documented in
BrainMap_Hippocampus_v2_1).</p>
<p>PFC: 5-HT destabilized (E2-dependent MAO-B inhibition removed).
Depression incidence peaks during perimenopause in women with no prior
history.</p>
<p>Sleep: P4/ALLO loss → GABA-A tone drops → insomnia, reduced NREM. Hot
flashes (hypothalamic thermoregulation destabilized) → sleep
fragmentation → glymphatic failure cascade.</p>
<p>Pain thresholds: E2 loss → vlPAG descending analgesia efficiency ↓ →
lower pain threshold systemwide. Fibromyalgia onset clusters at
perimenopause.</p>
<p>HRT timing hypothesis: HRT within 10 years of menopause onset shows
cognitive protection in observational + some RCT data. Initiated &gt;10
years post-menopause: does not show same benefit. Timing is a
neurological decision — evidence base still evolving; individual
risk-benefit assessment required.</p></td>
</tr>
<tr class="odd">
<td>Andropause (~40–60+, male)</td>
<td>T gradual decline (1–2%/year from ~35). Free T declines faster (SHBG
rises). Dihydrotestosterone (DHT) relative increase. GH/IGF-1 decline.
DHEA decline continues.</td>
<td><p>Gradual T decline vs acute E2 loss: different trajectory, less
acute neurological impact per unit time.</p>
<p>T → spatial memory, mood stability, motivation (via DA pathway),
libido. Decline: progressive cognitive changes, mood dysregulation,
reduced exercise motivation.</p>
<p>Brain aromatase: T → E2 locally in hippocampus continues;
aromatase-generated E2 in male brain is neuroprotective.</p>
<p>Sleep: T decline → sleep architecture changes (less deep NREM, more
REM fragmentation).</p></td>
</tr>
<tr class="even">
<td>Elderhood (70+ years)</td>
<td>E2 near zero (peripheral aromatase in adipose continues low-level).
T low. DHEA &lt;10–20% of peak. Neurosteroid synthesis reduced across
the board. GH/IGF-1 low. Osteocalcin: declining with physical
inactivity.</td>
<td><p>All sex-steroid-dependent neuroprotective mechanisms operate at
reduced capacity simultaneously: E2-mediated AMPA upregulation,
T-mediated spatial memory, ALLO-mediated GABA tone, DHEA
anti-glucocorticoid buffering.</p>
<p>Microglial senescence (SASP): senescent microglia produce
inflammatory cytokines chronically → neuroinflammation easier to
establish, harder to resolve.</p>
<p>Osteocalcin decline + irisin decline + peripheral BDNF decline =
simultaneous withdrawal of all four musculoskeletal-brain channels.
Exercise is the primary intervention to partially restore all four.</p>
<p>DHEA and pregnenolone supplementation in elderly: modest cognitive
benefits in RCTs, variable by baseline levels and population.</p></td>
</tr>
</tbody>
</table>

Table 4. Brain consequences of hormonal profile changes across the
lifespan.

### §15 — Sex Differences in Brain Function: The Hormonal Mechanisms

Sex differences in cognitive function, pain sensitivity, immune
reactivity, and mental health risk are substantially mediated by sex
hormones rather than fixed chromosomal architecture. The evidence base
from transgender individuals receiving hormone therapy confirms that
hormones — not chromosomes — drive the measurable differences, and that
the substrate is amenable to hormonal shifting.

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 32%" />
<col style="width: 46%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Domain</strong></td>
<td><strong>Observed Difference</strong></td>
<td><strong>Hormonal Mechanism</strong></td>
</tr>
<tr class="even">
<td>Spatial vs Verbal Cognition</td>
<td>Average male advantage: 3D mental rotation, targeting. Average
female advantage: verbal fluency, verbal memory, fine motor. Very large
individual overlap.</td>
<td><p>T organizational effect: neonatal T surge masculinizes spatial
circuits (parietal cortex, hippocampal geometry). Spatial advantage
correlates with prenatal T (2D:4D digit ratio).</p>
<p>E2 activational effect: verbal memory fluctuates with E2 cycle, peaks
at mid-cycle E2 max.</p>
<p>Transgender men (T administration): spatial performance improves.
Transgender women (E2 administration): spatial ↓, verbal memory ↑.
Hormones are causing the differences.</p></td>
</tr>
<tr class="odd">
<td>Immune Function &amp; Autoimmunity</td>
<td>Women: 80% of autoimmune disease burden (lupus 9:1 F, MS 3:1 F, RA
3:1 F, Hashimoto’s 7:1 F). Stronger vaccine responses. Lower infection
mortality for most pathogens.</td>
<td><p>E2 → ERα on immune cells → enhanced B-cell antibody production,
Th1/Th2 balance, NK cell activity. Female immune system is tuned to
respond more strongly.</p>
<p>T immunosuppressive at physiological levels (AR on immune cells).
Male: lower autoimmune risk but reduced vaccine response magnitude.</p>
<p>Pregnancy (high E2 + P4): immune balance toward tolerance → RA often
remits during pregnancy, flares postpartum.</p></td>
</tr>
<tr class="even">
<td>Pain Sensitivity</td>
<td>Women: lower pain thresholds for most pain modalities; higher
prevalence of fibromyalgia, IBS, TMD, migraine, chronic fatigue
syndrome.</td>
<td><p>vlPAG ERβ: E2 → descending analgesia efficiency ↑. E2 withdrawal
→ vlPAG efficiency ↓ → lower pain threshold systemwide.</p>
<p>Menstrual cycle pain threshold fluctuates: peaks at E2 maximum
(mid-cycle); lowest in late luteal phase.</p>
<p>Central sensitization susceptibility: E2 loss → vlPAG_efficiency⁻¹ →
descending inhibition fails → dorsal horn wind-up. This is the
fibromyalgia perimenopause cluster mechanism.</p></td>
</tr>
<tr class="odd">
<td>Mental Health Risk</td>
<td>Women: higher MDD, anxiety, PTSD, eating disorders. Men: higher
schizophrenia, ASD, externalizing disorders, completed suicide.
Different profile, not different burden.</td>
<td><p>E2 → raphe ERβ → 5-HT synthesis ↑, MAO-B inhibition: female mood
stability is partially E2-dependent → loss at perimenopause = new-onset
depression in previously resilient women.</p>
<p>ALLO: anxiolytic, DG pattern separation; ALLO collapse (PMDD, PPD,
perimenopause) → anxiety and intrusive memory risk.</p>
<p>T → DA synthesis, motivation, reduced depression risk: T
supplementation in men with hypogonadism shows antidepressant
effects.</p>
<p>Schizophrenia male preponderance: higher brain T may amplify DA
excess (the dopamine hypothesis of schizophrenia); female E2 may be
partly protective.</p></td>
</tr>
</tbody>
</table>

Table 5. Sex differences and their primary hormonal mechanisms.
Differences represent population averages with very large individual
overlap; they are not clinically useful predictors for individuals.

### §16 — Body State → Brain State: The Translation Table

The table below documents how peripheral body states are translated into
brain states. Each entry specifies the signal pathway, the brain state
produced, and the key simulation parameters affected. This table is the
operational interface between the peripheral system maps and the brain
structure maps.

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 23%" />
<col style="width: 23%" />
<col style="width: 31%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Body State</strong></td>
<td><strong>Pathway to Brain</strong></td>
<td><strong>Brain State Produced</strong></td>
<td><strong>Simulation Parameters Affected</strong></td>
</tr>
<tr class="even">
<td><strong>Acute infection / fever</strong></td>
<td>IL-1β, TNF-α, IL-6 → circumventricular organs OR vagal afferents →
brainstem → microglial activation. PGE2 → hypothalamus EP3/4 →
temperature setpoint ↑.</td>
<td>Sickness behavior: fatigue, anhedonia, social withdrawal, cognitive
slowing. Programmed adaptive response — metabolic resources redirected
to immune function. The feature, not a side effect.</td>
<td><p>activation_ceiling ↓</p>
<p>DA_tone[NAcc] ↓</p>
<p>cytokine_load ↑</p>
<p>microglial_M1_M2_ratio → DIM (acute)</p>
<p>metabolic_supply[cortex] ↓</p></td>
</tr>
<tr class="odd">
<td><strong>Chronic inflammation</strong></td>
<td>Persistent cytokine elevation → sustained microglial activation →
neuroinflammation. IDO activation → kynurenine → QUIN (excitotoxic) vs
KYNA (neuroprotective) imbalance.</td>
<td>Descending 5-HT/NE pathway impairment → pain amplification +
depression simultaneously. Hippocampal LTP suppression via QUIN → NMDA
excitotoxicity. BLA hyperactivation → anxiety.</td>
<td><p>5HT_synthesis_rate ↓ (IDO → QUIN dominates)</p>
<p>plasticity_suppression[hippocampus] ↑</p>
<p>BLA_reactivity ↑</p>
<p>descending_analgesia_efficiency ↓</p>
<p>NMDA_excitotoxicity_risk ↑</p></td>
</tr>
<tr class="even">
<td><strong>Acute psychological stress</strong></td>
<td>PVN → CRH → ACTH → cortisol (minutes-hours). LC NE burst (seconds).
Adrenal medulla EPI release (seconds). Simultaneous: HPA + SNS + LC
activated.</td>
<td>Amygdala hyperactivation (NE + CRH). PFC executive function reduced
(excess NE). Hippocampal encoding impaired (cortisol → LTP threshold ↑).
Fight-or-flight physiology prepared.</td>
<td><p>NE_phasic ↑ (BLA salience)</p>
<p>plasticity_suppression[hippocampus] ↑ (acute)</p>
<p>PFC_gain ↓ at high NE (inverted-U exceeded)</p>
<p>cortisol → gluconeogenesis ↑</p>
<p>HR ↑, MAP ↑ (SNS)</p></td>
</tr>
<tr class="odd">
<td><strong>Chronic psychological stress</strong></td>
<td>Sustained HPA activation → chronically elevated cortisol → GR
downregulation on hippocampus/subiculum → HPA brake failure. Concurrent:
HPG suppression, HPT suppression.</td>
<td>Hippocampal LTP suppression → memory impairment. CA3 dendritic
retraction. DG neurogenesis suppression. HPA feedback failure → cortisol
runaway. Depression, PTSD trajectories.</td>
<td><p>plasticity_suppression ↑ (chronic)</p>
<p>CA3_dendritic_integrity ↓</p>
<p>DG_neurogenesis_rate ↓</p>
<p>HPA_negative_feedback_strength ↓</p>
<p>GnRH_pulse_frequency ↓ (HPG suppression)</p></td>
</tr>
<tr class="even">
<td><strong>Exercise (acute high-intensity)</strong></td>
<td>Muscle BDNF → circulation → BBB → TrkB. Irisin (FNDC5 cleavage) →
αVβ5 integrin. Osteocalcin release ↑ (via mechanical loading). Lactate
4–10 mM → HCAR1. NE phasic ↑ (LC activation during exertion).</td>
<td>Acute BDNF rise → LTP threshold lowering. NE phasic → encoding
enhancement. Post-exercise: mild cortisol rise → acute LTP gating.
Lactate → cerebral angiogenesis signaling begins.</td>
<td><p>BDNF_peripheral ↑</p>
<p>NE_phasic_gate ↑ (encoding)</p>
<p>irisin_input[hippocampus] ↑</p>
<p>lactate_hippocampal ↑</p>
<p>DA_phasic[VTA] ↑ (reward feedback)</p></td>
</tr>
<tr class="odd">
<td><strong>Exercise (chronic training)</strong></td>
<td>Repeated exercise → cumulative osteocalcin rises → GPR158 BDNF ↑.
Mitochondrial biogenesis (PGC-1α). DG neurogenesis ↑ (BDNF, IGF-1).
Cerebrovascular reserve ↑ (HCAR1 angiogenesis). D2R density may be
maintained.</td>
<td>DG neurogenesis maintained → pattern separation quality preserved.
LTP_gain[CA1] supported. Cognitive resilience in aging. Depression risk
↓ (all four musculoskeletal-brain channels maintained).</td>
<td><p>DG_neurogenesis_rate ↑</p>
<p>cerebrovascular_reserve ↑ (chronic)</p>
<p>LTP_gain[CA1] supported via TrkB/BDNF pathway</p>
<p>osteocalcin_input[hippocampus] chronically ↑</p>
<p>D2R_density[striatum] maintained</p></td>
</tr>
<tr class="even">
<td><strong>Physical inactivity / sedentary aging</strong></td>
<td>AMPK under-stimulation → PGC-1α ↓ → myokines ↓. Mechanostat below
threshold → osteoblast activity ↓ → osteocalcin ↓. All four channels
(osteocalcin, irisin, peripheral BDNF, lactate) withdrawn
simultaneously.</td>
<td>DG neurogenesis rate falls. Hippocampal BDNF ↓. Pattern separation
degrades. Sarcopenia ↑. Insulin resistance ↑. Motivational substrate for
exercise reduces (D2R ↓ with aging).</td>
<td><p>osteocalcin_input[hippocampus] ↓</p>
<p>irisin_input[hippocampus] ↓</p>
<p>BDNF_peripheral ↓</p>
<p>DG_neurogenesis_rate ↓</p>
<p>insulin_resistance ↑ (GLUT4 ↓)</p>
<p>D2R_density[striatum] ↓ aging</p></td>
</tr>
<tr class="odd">
<td><strong>Sleep deprivation</strong></td>
<td>NE_tonic insufficient drop → microglial pruning inhibited (NE
actively suppresses microglial motility). Glymphatic clearance requires
NE_tonic near zero + aquaporin-4 on astrocyte endfeet. Adenosine
accumulates.</td>
<td>Synaptic clutter: CA1 SNR drops (insufficient pruning). Amyloid/tau
clearance impaired (glymphatic failure). Cortical excitability ↑
(insufficient ALLO/GABA normalization). Adenosine → activation_ceiling
↓.</td>
<td><p>complement_tagged[weak_edges]: pruning fails</p>
<p>amyloid_clearance ↓ (glymphatic)</p>
<p>adenosine_load ↑</p>
<p>activation_ceiling ↓</p>
<p>melatonin_synthesis ↓ if NE_tonic ↑ (screens/stress)</p></td>
</tr>
<tr class="even">
<td><strong>Menopause transition</strong></td>
<td>Erratic then absent E2 → LTP_gain[CA1] ↓. P4/ALLO collapse → DG GABA
tonic ↓. 5-HT destabilized (raphe ERβ deprived). vlPAG efficiency ↓.
Concurrent: DHEA declining, cortisol may be elevated.</td>
<td>Memory complaints (CA1 LTP ↓). DG hyperexcitability (ALLO collapse +
cortisol elevation simultaneous → SILO-HPC-3). New-onset depression.
Insomnia (ALLO/GABA ↓). Pain threshold ↓. Hot flashes (hypothalamic
thermostat destabilized).</td>
<td><p>LTP_gain[CA1] ↓ (E2 withdrawal)</p>
<p>GABA_tonic_inhibition[DG] ↓ (ALLO ↓)</p>
<p>5HT_synthesis_rate ↓ (raphe ERβ deprived)</p>
<p>vlPAG_efficiency ↓</p>
<p>HPA_negative_feedback_strength ↓ potential</p></td>
</tr>
<tr class="odd">
<td><strong>High pain load</strong></td>
<td>C-fiber nociceptors → DRG → dorsal horn → spinothalamic → thalamus →
S1 (sensory discrimination) + insula (affective component) + ACC
(suffering component). CGRP/SP: peripheral sensitization → central
sensitization.</td>
<td>Anterior insula activation → body state urgency in all decisions.
ACC → depressive ideation (pain-depression comorbidity). vlPAG
descending inhibition recruited. Opioid system engagement (acute).</td>
<td><p>descending_analgesia_efficiency = f(vlPAG, opioid_tone)</p>
<p>central_sensitization_susceptibility ↑ if chronic</p>
<p>DA_phasic[VTA] ↓ (anhedonia comorbidity)</p>
<p>body_state_urgency[insula] ↑</p></td>
</tr>
</tbody>
</table>

Table 6. Body state to brain state translation. For full pathway details
see individual Brain Maps (BrainMap\_\*.md v2.0 series) and Peripheral
Maps.

### §17 — Brain-Body Interface: Structure by Structure

The table below lists key brain structures with their primary body-state
inputs, outputs to peripheral systems, and key simulation parameters.
This is a condensed version of the full structure maps; for FQ
decompositions, sub-structure analyses, silo maps, and Rust struct
implementations see BrainMap\_\*.md v2.0 series.

<table>
<colgroup>
<col style="width: 17%" />
<col style="width: 23%" />
<col style="width: 23%" />
<col style="width: 35%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Structure</strong></td>
<td><strong>Primary Body Inputs</strong></td>
<td><strong>Primary Body Outputs</strong></td>
<td><strong>Key State Parameters</strong></td>
</tr>
<tr class="even">
<td><strong>Hippocampus (CA1, CA3, DG, Subiculum)</strong></td>
<td><p>Cortisol/GR: LTP suppression, DG neurogenesis ↓</p>
<p>E2/T: CA1 spine density ↑, LTP gain ↑</p>
<p>ALLO: DG GABA tonic gate</p>
<p>Osteocalcin → GPR158: BDNF ↑, monoamines ↑ [v2.0 new]</p>
<p>Irisin → αVβ5: neuroplasticity [v2.0 new]</p>
<p>Peripheral BDNF (muscle) → TrkB [v2.0 new]</p>
<p>Lactate → HCAR1: angiogenesis + SIRT1-BDNF [v2.0 new]</p>
<p>IGF-1: DG neurogenesis</p>
<p>Kynurenine → QUIN: NMDA excitotoxicity risk</p></td>
<td><p>Subiculum → PVN: HPA negative feedback brake</p>
<p>CA1 → vmPFC: safety memory for fear extinction</p>
<p>Fornix → hypothalamus, septal, mammillary bodies</p></td>
<td><p>LTP_gain[CA1] = f(E2, DHEA, cortisol⁻¹)</p>
<p>DG_neurogenesis_rate = f(BDNF_all_sources, IGF-1, cortisol⁻¹)</p>
<p>HPA_negative_feedback_strength</p>
<p>osteocalcin_input[hpc]</p>
<p>irisin_input[hpc]</p>
<p>cerebrovascular_reserve</p></td>
</tr>
<tr class="odd">
<td><strong>Hypothalamus (PVN, ARC, SCN, SON, LH)</strong></td>
<td>ALL systemic signals via circumventricular organs (SFO, OVLT, area
postrema). Blood osmolarity → AVP/thirst. Blood glucose → ARC hunger.
T/E2/cortisol feedback. Immune cytokines → fever.</td>
<td>CRH → HPA cascade. GnRH → HPG. TRH → HPT. ADH/AVP → renal water
retention. Orexin → LC → global arousal. ANS preganglionic neurons →
heart, gut, vasculature.</td>
<td><p>GnRH_pulse_frequency</p>
<p>CRH_release_rate</p>
<p>orexin_level</p>
<p>ARC_satiety = f(leptin, insulin, GLP-1, ghrelin⁻¹)</p>
<p>AVP_release_rate = f(blood_osmolarity)</p>
<p>circadian_phase (SCN output)</p></td>
</tr>
<tr class="even">
<td><strong>Amygdala (BLA, CeA, ITC, LA)</strong></td>
<td>Cortisol → GR: BLA sensitization. NE phasic → β-AR: threat encoding,
LTP threshold lowering. E2 → ERα on BLA: reactivity modulation. CRH from
PVN: BLA potentiation. Immune cytokines: BLA hyperactivation in chronic
inflammation.</td>
<td>CeA → PAG: threat response (freeze/fight/flight). CeA → PVN: HPA
activation. CeA → LC: NE surge. BLA → hippocampus: emotional context
tagging. CeA → lateral hypothalamus: sympathetic activation.</td>
<td><p>BLA_reactivity = f(NE_phasic, CRH, cortisol)</p>
<p>threat_response_threshold</p>
<p>ITC_gate_strength (fear extinction gate)</p>
<p>BNST_anxiety_state</p></td>
</tr>
<tr class="odd">
<td><strong>Locus Coeruleus (LC)</strong></td>
<td>Blood pressure via NTS → LC. Hypoxia → direct LC activation. IL-1β →
LC NE release. E2 → increased LC baseline firing. Immune CRH → LC.</td>
<td>NE broadcast to all cortical regions + brainstem + spinal cord. LC →
pineal (NE drives melatonin synthesis). LC → sympathetic preganglionic →
peripheral tone.</td>
<td><p>NE_tonic_baseline = f(E2_level, IL-1β, adenosine_load⁻¹,
orexin_level, baroreceptor_input, NPY_reserve)</p>
<p>NE_phasic_gain = f(novelty, threat_salience)</p>
<p>melatonin_onset_delay = f(NE_tonic)</p>
<p>glymphatic_clearance ↑ when NE_tonic ↓ (sleep)</p></td>
</tr>
<tr class="even">
<td><strong>PAG (dPAG, vlPAG)</strong></td>
<td>CeA threat signal → PAG. Peripheral opioid peptides from tissue
damage → vlPAG. E2 → ERβ on vlPAG → descending analgesia efficiency ↑.
E2 withdrawal → vlPAG efficiency ↓.</td>
<td>dPAG → sympathetic arousal + fight/flight. vlPAG → Raphe Magnus →
dorsal horn → descending analgesia. vlPAG → vagal cardioinhibitory.</td>
<td><p>vlPAG_efficiency = f(E2·ERβ, opioid_tone)</p>
<p>pain_threshold = f(vlPAG_efficiency,
descending_analgesia_efficiency)</p>
<p>central_sensitization_susceptibility = vlPAG_efficiency⁻¹</p></td>
</tr>
<tr class="odd">
<td><strong>Insula (posterior → anterior)</strong></td>
<td>ALL interoceptive signals: gut distension, cardiac rhythm,
respiratory rate, bladder, pain, temperature, nausea, hunger, thirst,
fatigue. Right insula: cardiac interoception (right insula lesions →
arrhythmia). Cortisol and NE amplify interoceptive salience.</td>
<td>Anterior insula → PFC/ACC: body state informs every decision.
Anterior insula → amygdala: body sensations amplify/suppress emotional
responses.</td>
<td><p>body_state_signal_strength (composite interoceptive)</p>
<p>interoceptive_salience = f(cortisol, NE_tonic)</p>
<p>aInsula_PFC_coupling</p>
<p>aInsula_BLA_coupling</p></td>
</tr>
<tr class="even">
<td><strong>VTA (mesolimbic DA)</strong></td>
<td>Leptin → DA tone ↑. Ghrelin → VTA DA phasic ↑ (food craving). Opioid
peptides → μ-opioid → DA release. Exercise → DA phasic (reward
feedback). Sex hormones: E2 + T both modulate DA synthesis and D1/D2
expression.</td>
<td>NAcc DA: reward encoding, motivated behavior, salience. PFC D1:
working memory gating. Striatum: motor learning. Mesolimbic: addiction
vulnerability.</td>
<td><p>RPE = DA_phasic - prediction</p>
<p>DA_tonic[VTA] = f(leptin, opioid_tone, E2)</p>
<p>D2R_density[striatum] = aging_modifier</p>
<p>hedonic_reward_threshold</p></td>
</tr>
<tr class="odd">
<td><strong>Raphe Nuclei (5-HT)</strong></td>
<td>E2 → ERβ on raphe: 5-HT synthesis ↑, MAO-B inhibition. T → 5-HT
modulation. IL-1β/IDO → tryptophan diversion → 5-HT synthesis rate ↓.
Gut tryptophan (LAT1 BBB transport) = rate-limiting substrate.</td>
<td>5-HT to all brain regions: mood stability, impulse control. Dorsal
horn (descending analgesia). GI motility (brain 5-HT to raphe spinal
pathway). BNST: anxiety tone.</td>
<td><p>5HT_synthesis_rate = f(tryptophan_BBB, IDO_activity⁻¹,
E2·ERβ)</p>
<p>descending_analgesia_efficiency (5-HT contribution)</p>
<p>mood_stability_parameter</p></td>
</tr>
</tbody>
</table>

Table 7. Key brain structures with peripheral body interfaces. For FQ
decompositions and full parameter inventories see individual Brain Maps
(v2.0 series). \[v2.0 new\] = additions from musculoskeletal re-pass and
peripheral system integrations completed in this version.

### §18 — Exercise as Endocrine Architecture: Four Parallel Brain
Channels

Exercise is not merely a lifestyle intervention with general health
benefits — it is a structured endocrine architecture in which skeletal
muscle and bone act as an exercise-transducing system producing four
parallel signals that converge on hippocampal neuroplasticity. This
architecture is now sufficiently characterized to document its
components, their mechanisms, and the critical silo gap: no human study
has simultaneously measured all four channels with hippocampal outcomes.

|                                     |                                                                                                                                                 |                                                                                                                                                                    |                                                                                                                                                       |                                                                                                                                                                              |
|-------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Channel**                         | **Source**                                                                                                                                      | **Mechanism**                                                                                                                                                      | **Hippocampal Target**                                                                                                                                | **Evidence Tier / Key Reference**                                                                                                                                            |
| **Osteocalcin / GPR158**            | Bone osteoblasts. Undercarboxylated ucOC released in proportion to mechanical loading and exercise.                                             | ucOC → GPR158 (GPCR) on hippocampal neurons → cAMP → CREB → BDNF gene expression + monoamine synthesis enzyme upregulation (TH, TPH, DBH).                         | BDNF ↑ → DG neurogenesis ↑. DA/5-HT/NE synthesis ↑ → monoamine tone supports encoding mode.                                                           | Tier B mouse causal (Khrimian et al. J Exp Med 2017). Tier C human clinical magnitude. 2024 MR study: causal link osteocalcin → AD risk (Guo et al. Transl Psychiatry 2024). |
| **Irisin / αVβ5 integrin**          | Skeletal muscle FNDC5 cleavage during exercise. Requires extracellular Hsp90α to activate αVβ5 integrin into high-affinity open state.          | Irisin → αVβ5 → FAK/PI3K downstream signaling → hippocampal neuroplasticity. Cryo-EM receptor mechanism confirmed 2023.                                            | Neuroplasticity and resistance to neurodegeneration. Lower circulating irisin in AD and MDD (human observational).                                    | Tier B — receptor cryo-EM confirmed (Kim et al. Mol Cell 2023). Human observational association. Tier C for clinical causation.                                              |
| **Peripheral BDNF / TrkB**          | Skeletal muscle type I fibers express pro-BDNF during exercise. Cleaved to mature BDNF in circulation. Lactate infusion augments this response. | Circulating mature BDNF crosses BBB → TrkB on DG granule cells + CA1 pyramidal neurons → LTP, synaptogenesis, neurogenesis.                                        | DG neurogenesis ↑ via TrkB on granule cell progenitors. LTP_gain\[CA1\] enhanced. Parallel pathway to IGF-1→BDNF chain (both active during exercise). | Tier B — pro-BDNF in human muscle confirmed (Edman et al. Function 2024). Lactate augments human BDNF response in same study.                                                |
| **Lactate / HCAR1 + SIRT1 pathway** | High-intensity exercise → blood lactate 4–10 mM. Crosses BBB via MCT1/2 monocarboxylate transporters.                                           | Acute: HCAR1 (GPCR) → Gi → cerebral angiogenesis. Hippocampal neurons: SIRT1 → PGC-1α → FNDC5 → BDNF gene expression. Chronic training: cerebrovascular reserve ↑. | Acute: BDNF ↑ augmentation via SIRT1-FNDC5 pathway. Chronic: cerebrovascular reserve ↑ → baseline hippocampal perfusion ↑.                            | Tier B acute (HCAR1 mechanism + human BDNF augmentation). Tier C for direct hippocampal BDNF causal chain. Müller et al. J Clin Med 2020; Edman et al. Function 2024.        |

Table 8. Four parallel musculoskeletal-to-hippocampus exercise channels.

SILO-HPC-7 (documented in BrainMap_Hippocampus_v2_1.md): All four
channels converge on DG_neurogenesis_rate and hippocampal plasticity.
All four are suppressed simultaneously by physical inactivity. All four
are restored simultaneously by exercise. No published human study has
measured all four channels simultaneously with hippocampal outcomes (DG
volume, LTP proxy, cognitive function). The four literatures do not
cross-cite. Magnitude: HIGH. This is the complete mechanistic basis for
exercise as antidepressant and cognitive aging intervention, and the
quantitative weighting of each channel remains uncharacterized.

Clinical implication: Single-channel pharmacological interventions
(osteocalcin supplementation, irisin analogues, BDNF infusion) each
activate one channel. Exercise activates all four simultaneously. This
convergence architecture is why no single pharmacological agent
currently activates as broadly as exercise across these pathways, to our
knowledge. Tier C for the clinical magnitude of this combined effect.

## Part V — Clinical Reclassification and Implications

### §19 — Conditions Reclassified Through the Integrated System

The following conditions appear single-system under the fragmented model
and multi-system under the integrated model. Each reclassification
identifies the clinical management gap that follows from treating them
as single-system disorders.

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 27%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Condition</strong></td>
<td><strong>Fragmented Model</strong></td>
<td><strong>Integrated Model + Management Gap</strong></td>
</tr>
<tr class="even">
<td><strong>Menopause</strong></td>
<td>Reproductive event. Manage hot flashes. HRT as risk/benefit re:
breast cancer and cardiovascular disease.</td>
<td><p>Whole-brain event: hippocampal LTP efficiency ↓; 5-HT synthesis
↓; sleep disrupts (ALLO loss); pain thresholds ↓; amyloid protection
reduces; HPA sensitization.</p>
<p>HRT timing hypothesis: within 10 years of menopause onset shows
cognitive protection. Timing is a neurological decision, not only
gynecological. Evidence base evolving; individual risk-benefit including
APOE4 status required.</p>
<p>Management gap: menopause neurological consequences managed by
neurologist/psychiatrist/pain specialist separately from
gynecologist/cardiologist. No integrated specialty.</p></td>
</tr>
<tr class="odd">
<td><strong>T2D / Metabolic Syndrome</strong></td>
<td>Endocrinologist. Blood glucose management. Insulin resistance is
peripheral.</td>
<td><p>T2D → brain insulin resistance → hippocampal LTP impaired →
memory failure. T2D → peripheral inflammation → neuroinflammation →
cognitive impairment. T2D → peripheral neuropathy → central
sensitization → chronic pain.</p>
<p>T2D + menopause: E2 loss removes insulin-sensitizing effect in
hippocampus → double vulnerability.</p>
<p>GLP-1 receptor agonists: brain GLP-1R suppresses hunger (ARC) +
potential neuroprotective effects; lean mass loss 25–40% requires
musculoskeletal management.</p>
<p>Management gap: no co-management of cognitive, pain, and metabolic
trajectories in T2D.</p></td>
</tr>
<tr class="even">
<td><strong>Depression (MDD)</strong></td>
<td>Psychiatry. Serotonin deficiency. SSRI/SNRI. May add
antipsychotic.</td>
<td><p>MDD has at least five mechanistically distinct subtypes with
different primary drivers: (1) HPA dysregulation (cortisol runaway →
hippocampal damage); (2) immune-inflammatory (IDO → kynurenine → QUIN +
BDNF ↓); (3) hormonal (E2 withdrawal, T deficiency, ALLO collapse); (4)
metabolic (brain insulin resistance, leptin resistance); (5)
circadian/sleep (NE_tonic ↑ → glymphatic failure → synaptic
clutter).</p>
<p>Antidepressants may work primarily via DG neurogenesis restoration
(BDNF induction), not 5-HT floor per se — the two are mechanistically
the same chain (5-HT → 5-HT1A on DG → neurogenesis).</p>
<p>Management gap: MDD treated as one disease. Subtype-specific
biomarkers (cortisol diurnal slope, IL-6, hormone panels, HRV) not
routinely measured.</p></td>
</tr>
<tr class="odd">
<td><strong>Chronic Pain</strong></td>
<td>Pain management. Analgesics, anticonvulsants, nerve blocks.
Psychological overlay.</td>
<td><p>Chronic pain = central sensitization: vlPAG descending inhibition
failure, C-fiber sensitization (CGRP/SP), and dorsal horn wind-up from
sustained nociceptive input.</p>
<p>Hormonal drivers: E2 loss → vlPAG efficiency ↓; cortisol chronic →
descending 5-HT/NE pathway impaired; inflammatory cytokines → kynurenine
→ NMDA sensitization.</p>
<p>Fibromyalgia onset clusters at perimenopause → vlPAG E2 deprivation
is a principal mechanism, not psychosomatization.</p>
<p>Management gap: chronic pain rarely addressed with hormonal or
anti-inflammatory strategies despite mechanistic relevance.</p></td>
</tr>
<tr class="even">
<td><strong>Alzheimer’s Disease</strong></td>
<td>Neurology. Amyloid hypothesis. Cholinesterase inhibitors. Emerging:
anti-amyloid mAbs.</td>
<td><p>Multi-system failure: ACh depletion (encoding mode fails) +
amyloid/tau (CA1 synaptic dysfunction) + insulin resistance (brain
insulin resistance → amyloid precursor processing via insulin-degrading
enzyme (IDE)) + immune-microglial (TREM2/DAM failure) + glymphatic
failure (sleep-dependent amyloid clearance) + osteocalcin decline
(GPR158 signaling ↓, 2024 MR study) + E2 loss (APOE4 women: accelerated
perimenopause amyloid accumulation).</p>
<p>HRT timing window: E2 neuroprotection in the decade around menopause
may represent a modifiable risk window.</p>
<p>Management gap: Alzheimer’s managed as neurological disease;
metabolic, hormonal, sleep, cardiovascular, and exercise-related risk
factors are managed by separate specialties if at all.</p></td>
</tr>
<tr class="odd">
<td><strong>Sarcopenia + Cognitive Decline</strong></td>
<td>Geriatrics. Muscle loss is physical. Cognitive decline is
neurological. Treated separately.</td>
<td><p>Same cascade: physical inactivity → AMPK under-stimulation →
sarcopenia → mechanostat below threshold → osteocalcin ↓ → GPR158 →
hippocampal BDNF ↓ → DG neurogenesis ↓ → cognitive decline. The
musculoskeletal-brain axis means sarcopenia and cognitive decline are
not parallel age-related processes — they share a common upstream
mechanism.</p>
<p>Resistance training: simultaneously reverses sarcopenia AND activates
all four musculoskeletal-hippocampal channels. Most mechanistically
complete anti-aging intervention currently characterized.</p>
<p>Management gap: physical and cognitive aging managed separately; no
clinical specialty integrates musculoskeletal health with cognitive
reserve.</p></td>
</tr>
</tbody>
</table>

Table 9. Conditions reclassified through the integrated system. Note
that the integrated model does not replace the fragmented model’s
validated interventions — it adds dimensions that the fragmented model
cannot see.

### §20 — Clinical Implications: What Changes When You See the System

The integrated brain-body model changes clinical practice in five areas.
These are not new treatments — the interventions already exist. The
change is recognizing that the same intervention operates across
multiple systems simultaneously, and that failure to intervene in one
domain accelerates failure in another.

**1. Hormone decisions are brain decisions:** Sex hormone prescribing
(HRT, testosterone therapy, hormonal contraception) affects brain
function directly and immediately. Decisions made without reference to
cognitive, mood, pain, and sleep consequences are incomplete. The
timing, formulation, and route of administration all affect brain
bioavailability differently from peripheral target tissues.

**2. Exercise is the most complete brain-body intervention:** No single
pharmaceutical agent simultaneously activates AMPK-PGC-1α (metabolic),
BDNF-TrkB (hippocampal), osteocalcin-GPR158 (bone-brain), irisin-αVβ5
(muscle-brain), and descending analgesia (PAG) pathways. Exercise does,
to our knowledge. The mechanistic breadth of exercise is not
motivational framing — it is an architectural fact. Physical inactivity
creates a multi-channel deficiency state that no currently available
drug addresses comprehensively.

**3. Sleep is maintenance infrastructure, not recovery:** Deep sleep is
the only time the brain performs required maintenance operations:
microglial pruning (NE_tonic drop required), glymphatic amyloid/tau
clearance (aquaporin-4 on astrocyte endfeet + NE_tonic drop), CA3 memory
replay and CA1→cortex consolidation, and DG granule cell integration.
Disruption is not "suboptimal" — it is deferred maintenance on brain
infrastructure, with cumulative consequences for amyloid load, synaptic
clutter, and cognitive performance.

**4. Inflammation is a brain state, not just an immune state:**
Persistent systemic inflammation (chronic infection, obesity-associated,
autoimmune) is not contained within the immune system. IL-1β, TNF-α, and
IDO-driven kynurenine are brain state modulators. The cognitive and mood
consequences of chronic inflammation are mechanistically direct, not
merely "comorbidities." Treating the source of inflammation is treating
a brain condition.

**5. Autonomic tone is a readout of brain-body integration:** HRV
measures the brain-body integration state in real time. Low HRV is not
just a cardiac risk factor — it indicates reduced cholinergic
anti-inflammatory tone, impaired emotional regulation, and compromised
baroreflex flexibility. HRV improvement from exercise, breathing
practices, or vagal nerve stimulation represents direct improvement in
brain-body coupling, not merely peripheral tone.

### §21 — Conclusion

The brain and body are one system. That statement has been true in the
biological literature for decades. It is now true in the map series that
supports this document: 44 individual structure and system maps
characterizing the brain structures, peripheral nervous systems,
endocrine systems, and organ systems with sufficient mechanistic detail
to implement in a biologically-grounded simulation.

v2.0 integrates three developments since v1.3: the peripheral nervous
system architecture (ANS, ENS, somatic PNS), the organ system brain
interfaces (cardiovascular, metabolic-gut, immune, respiratory,
musculoskeletal, integumentary, hepatic, renal), and the
musculoskeletal-hippocampal exercise architecture (four parallel
channels now individually confirmed and collectively forming
SILO-HPC-7). The highway model has been extended from six to ten axes.
The NT/hormone table has been expanded to include osteocalcin, irisin,
GLP-1, and FGF23 as characterized brain signaling molecules.

The literature silos documented throughout this paper are not minor gaps
— they are systematic features of how the fragmented medical system has
studied the fragmented human body. LTP_gain\[CA1\] is governed by three
variables (E2, DHEA, cortisol) studied by three literatures that rarely
cite each other. DG neurogenesis is governed by five inputs (IGF-1,
cortisol, ALLO, microglial BDNF, E2) studied by five literatures without
combined experiments. The four exercise-brain channels converge on the
same downstream parameter (DG_neurogenesis_rate) but have never been
measured simultaneously in a single human study. These are not failures
of individual researchers — they are failures of the fragmented model
that required each system to be studied in isolation.

The next phase of this project: Tier 6 limbic re-passes (hippocampus
complete, hypothalamus, amygdala, ACC, insula pending), full BrainBody
merge integrating all maps into the unified simulation architecture.
Simultaneous release of all papers in the series when complete.

**References**

\[1\] Berthoud HR & Neuhuber WL. Functional and chemical anatomy of the
afferent vagal system. Auton Neurosci 85 (2000) 1–17.

\[2\] Tracey KJ. The inflammatory reflex. Nature 420 (2002) 853–859.

\[3\] Furness JB. The enteric nervous system and neurogastroenterology.
Nat Rev Gastroenterol Hepatol 9 (2012) 286–294.

\[4\] Guyton AC & Hall JE. Textbook of Medical Physiology. 13th ed.
Elsevier (2016).

\[5\] Xie L et al. Sleep drives metabolite clearance from the adult
brain. Science 342 (2013) 373–377.

\[6\] Dantzer R et al. From inflammation to sickness and depression:
when the immune system subjugates the brain. Nat Rev Neurosci 9 (2008)
46–56.

\[7\] Cryan JF & Dinan TG. Mind-altering microorganisms: the impact of
the gut microbiota on brain and behaviour. Nat Rev Neurosci 13 (2012)
701–712.

\[8\] Nalbandian G & Kovats S. Understanding sex biases in immunity.
Immunol Res 40 (2008) 201–210.

\[9\] Pavlov VA & Tracey KJ. Neural regulation of immunity: molecular
mechanisms and clinical translation. Nat Neurosci 20 (2017) 156–166.

\[10\] McEwen BS. Stress, adaptation, and disease: allostasis and
allostatic load. Ann NY Acad Sci 840 (1998) 33–44.

\[11\] Micevych PE & Mermelstein PG. Membrane estrogen receptors acting
through metabotropic glutamate receptors. J Neuroendocrinol 20 (2008)
196–204.

\[12\] Woolley CS. Estrogen-mediated structural and functional synaptic
plasticity in the female rat hippocampus. Horm Behav 34 (1998) 140–148.

\[13\] Baulieu EE. Neurosteroids: a novel function of the brain.
Psychoneuroendocrinology 23 (1998) 963–987.

\[14\] Mellon SH & Griffin LD. Neurosteroids: biochemistry and clinical
significance. Trends Endocrinol Metab 13 (2002) 35–43.

\[15\] Maguire J & Salpekar JA. Stress, seizures, and
hypothalamic–pituitary–adrenal axis targets for the treatment of
epilepsy. Epilepsy Behav 26 (2013) 352–362.

\[16\] Bhatt DL et al. (editors). Hurst’s The Heart. 14th ed.
McGraw-Hill (2017). \[Cardiovascular reference\]

\[17\] Labrie F et al. DHEA and its transformation into androgens and
estrogens in peripheral target tissues. Front Neuroendocrinol 22 (2001)
185–212.

\[18\] Compagnone NA & Mellon SH. Pregnenolone transport via plasma
membrane vesicles involves binding proteins. Proc Natl Acad Sci USA 95
(1998) 4678–4683.

\[19\] Wolf OT & Kirschbaum C. Actions of dehydroepiandrosterone and its
sulfate in the central nervous system: effects on cognition and emotion
in animals and humans. Brain Res Rev 30 (1999) 264–288.

\[20\] Woolley CS & McEwen BS. Estradiol mediates fluctuation in
hippocampal synapse density during the estrous cycle in the adult rat. J
Neurosci 12 (1992) 2549–2554.

\[21\] Khrimian L et al. Gpr158 mediates osteocalcin’s regulation of
cognition. J Exp Med 214 (2017) 2859–2873.

\[22\] Kim H et al. Irisin acts through its integrin receptor in a
two-step process involving extracellular Hsp90α. Mol Cell 83 (2023)
2150–2163.

\[23\] Refetoff S & Dumitrescu AM. Syndromes of reduced sensitivity to
thyroid hormone. Mol Cell Endocrinol 322 (2007) 72–81.

\[24\] Melzack R & Wall PD. Pain mechanisms: a new theory. Science 150
(1965) 971–979.

\[25\] Henderson VW & Brinton RD. Menopause and mitochondria: windows
into estrogen effects on Alzheimer’s disease risk and therapy. Prog
Brain Res 192 (2011) 77–96.

\[26\] Whitmer RA et al. Timing of hormone therapy and dementia: the
critical window theory revisited. Ann Neurol 69 (2011) 163–169.

\[27\] Woolley CS. Acute effects of estrogen on neuronal physiology.
Annu Rev Pharmacol Toxicol 47 (2007) 657–680.

\[28\] Joffe H et al. Epidemiology of perimenopausal depression.
Menopause 14 (2007) 374–380.

\[29\] Mosconi L et al. Amyloid and metabolic PET imaging of cognitively
normal adults with Alzheimer’s parents. Neurobiol Aging 34 (2013) 22–34.

\[30\] de la Monte SM. Type 3 diabetes is sporadic Alzheimer’s disease:
mini-review. Eur Neuropsychopharmacol 24 (2014) 1954–1960.

\[31\] Edman S et al. Pro-brain-derived neurotrophic factor (BDNF), but
not mature BDNF, is expressed in human skeletal muscle. Function 5
(2024) zqae005.

\[32\] Guo X et al. Causal effect of blood osteocalcin on the risk of
Alzheimer’s disease. Transl Psychiatry 14 (2024) 205.

\[33\] Müller P et al. Lactate and BDNF: key mediators of exercise
induced neuroplasticity? J Clin Med 9 (2020) 1136.

\[34\] Volkow ND et al. Association between age and striatal dopamine D2
receptors: a PET study. J Neurosci 18 (1998) 1032–1038.

\[35\] Benveniste H et al. The glymphatic pathway: waste removal from
the CNS via cerebrospinal fluid transport. Neuroscientist 23 (2017)
454–468.

\[36\] Collaer ML & Hines M. Human behavioral sex differences: a role
for gonadal hormones during early development? Psychol Bull 118 (1995)
55–77.

\[37\] Meltzer-Brody S et al. Brexanolone injection in post-partum
depression: two multicentre, double-blind, randomised,
placebo-controlled, phase 3 trials. Lancet 392 (2018) 1058–1070.

*All papers in this series are unpublished drafts. Not yet peer
reviewed. Internal reference document.*
