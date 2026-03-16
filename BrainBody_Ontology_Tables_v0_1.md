### Table 1 — Signals

21 signals: 15 core (starter pack) + 6 additions from map series
(kynurenine_quin, dhea_neurosteroid, thyroid_t3_brain, bdnf_peripheral,
d2r_aging_motivation, opioid_vlpag). Tier colors: green=A, light
green=A/B, amber=B/C, orange=C. Status colors: green=High,
blue=Medium-high, yellow=Medium. SILO annotations in Notes column
reference documented gaps in BrainMap series.

<table>
<colgroup>
<col style="width: 7%" />
<col style="width: 5%" />
<col style="width: 6%" />
<col style="width: 7%" />
<col style="width: 5%" />
<col style="width: 4%" />
<col style="width: 8%" />
<col style="width: 6%" />
<col style="width: 7%" />
<col style="width: 5%" />
<col style="width: 4%" />
<col style="width: 9%" />
<col style="width: 3%" />
<col style="width: 5%" />
<col style="width: 5%" />
<col style="width: 7%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Signal_ID</strong></td>
<td><strong>Signal_Class</strong></td>
<td><strong>Source</strong></td>
<td><strong>Trigger</strong></td>
<td><strong>Route</strong></td>
<td><strong>Direction</strong></td>
<td><strong>Brain_Targets</strong></td>
<td><strong>Peripheral_Targets</strong></td>
<td><strong>Receptor_or_Interface</strong></td>
<td><strong>Effect_Sign</strong></td>
<td><strong>Timescale_Onset</strong></td>
<td><strong>State_Variables_Affected</strong></td>
<td><strong>Tier</strong></td>
<td><strong>Measurement_Proxy</strong></td>
<td><strong>Model_Status</strong></td>
<td><strong>Notes</strong></td>
</tr>
<tr class="even">
<td><strong>cortisol_hpa</strong></td>
<td>Hormone</td>
<td>Adrenal cortex</td>
<td>HPA activation, stress, threat appraisal</td>
<td>Blood</td>
<td>Body→brain</td>
<td><p>Hippocampus</p>
<p>Amygdala</p>
<p>Hypothalamus</p>
<p>PFC</p></td>
<td><p>Liver</p>
<p>Immune</p>
<p>Gonads</p>
<p>Muscle</p></td>
<td>GR, MR</td>
<td>Modulatory; chronic suppressive</td>
<td>Minutes–hours</td>
<td><p>cortisol_load</p>
<p>hpa_feedback_strength</p>
<p>ltp_gain_ca1</p>
<p>threat_bias</p>
<p>plasticity_suppression_hpc</p></td>
<td><strong>A</strong></td>
<td>Serum/salivary cortisol; diurnal slope</td>
<td>High priority</td>
<td><p>Separate cortisol_pulse (acute) from cortisol_load (chronic)</p>
<p>GR densest in hippocampus</p>
<p>HPA brake via subiculum GR</p></td>
</tr>
<tr class="odd">
<td><strong>vagal_afferent</strong></td>
<td>Afferent stream</td>
<td>Gut, lung, heart, viscera via vagus</td>
<td>Distension, stretch, inflammation, nutrient state</td>
<td>Vagus / NTS</td>
<td>Body→brain</td>
<td><p>NTS</p>
<p>Insula</p>
<p>Hypothalamus</p>
<p>Parabrachial</p></td>
<td>None (afferent only)</td>
<td>Mechanoreceptors, chemoreceptors, vagal C-fibers</td>
<td>Informational, state-reporting</td>
<td>Milliseconds–seconds</td>
<td><p>body_state_signal_strength</p>
<p>satiety_signal</p>
<p>vagal_tone</p>
<p>interoceptive_salience</p></td>
<td><strong>A</strong></td>
<td>HRV; gastric signals; respiration measures</td>
<td>High priority</td>
<td><p>80–90% of vagal fibers are afferent</p>
<p>Core backbone for whole-body state estimation</p>
<p>SILO: gut/cardiac/lung afferents studied separately</p></td>
</tr>
<tr class="even">
<td><strong>insulin_brain</strong></td>
<td>Hormone</td>
<td>Pancreatic β-cells</td>
<td>Blood glucose rise, incretins (GLP-1, GIP)</td>
<td>Blood / BBB receptor-mediated transcytosis</td>
<td>Body→brain</td>
<td><p>Hippocampus</p>
<p>Hypothalamus ARC</p>
<p>Cortex</p></td>
<td><p>Muscle</p>
<p>Adipose</p>
<p>Liver</p></td>
<td>Insulin receptor (IR, InsR)</td>
<td>Modulatory, trophic, satiety</td>
<td>Minutes–hours</td>
<td><p>brain_insulin_signal</p>
<p>brain_insulin_resistance_index</p>
<p>arc_satiety</p>
<p>ltp_gain_hpc</p>
<p>ampa_trafficking_rate</p></td>
<td><strong>A/B</strong></td>
<td>Fasting insulin; HOMA-IR; clamp-derived proxies</td>
<td>High priority</td>
<td><p>Keep central insulin separate from peripheral action</p>
<p>Brain insulin resistance: T2D → 2× AD risk</p>
<p>SILO: brain IR studied separately from peripheral IR</p></td>
</tr>
<tr class="odd">
<td><strong>leptin_adiposity</strong></td>
<td>Hormone</td>
<td>Adipose tissue</td>
<td>Fat mass, energy stores</td>
<td>Blood</td>
<td>Body→brain</td>
<td><p>Hypothalamus ARC</p>
<p>VTA</p>
<p>Hippocampus</p>
<p>Amygdala</p></td>
<td><p>Reproductive axis</p>
<p>Immune system</p></td>
<td>Leptin receptor (LepR, ObR)</td>
<td>Modulatory, satiety/permissive</td>
<td>Hours–days</td>
<td><p>leptin_signal</p>
<p>leptin_resistance_index</p>
<p>da_tonic_vta</p>
<p>arc_satiety</p>
<p>ltp_gain_hpc</p></td>
<td><strong>A/B</strong></td>
<td>Serum leptin</td>
<td>High priority</td>
<td><p>Model resistance separately from absolute level</p>
<p>Leptin threshold required for puberty onset (GnRH
permissive)</p></td>
</tr>
<tr class="even">
<td><strong>ghrelin_hunger</strong></td>
<td>Hormone</td>
<td>Gastric fundus</td>
<td>Fasting, energy deficit</td>
<td>Blood / vagal afferent</td>
<td>Body→brain</td>
<td><p>ARC</p>
<p>VTA</p>
<p>Hypothalamus</p>
<p>Hippocampus</p></td>
<td><p>GI tract</p>
<p>Pituitary</p></td>
<td>GHSR (growth hormone secretagogue receptor)</td>
<td>Excitatory to hunger/motivation</td>
<td>Minutes–hours</td>
<td><p>hunger_drive</p>
<p>da_food_salience</p>
<p>meal_initiation_threshold</p>
<p>dg_neurogenesis_rate</p></td>
<td><strong>A/B</strong></td>
<td>Serum ghrelin</td>
<td>Medium</td>
<td><p>DG neurogenesis ↑ at moderate ghrelin (fasting-state
plasticity)</p>
<p>Counterweight to leptin and GLP-1</p></td>
</tr>
<tr class="odd">
<td><strong>glp1_gut_satiety</strong></td>
<td>Hormone</td>
<td>Gut L-cells (ileum/colon)</td>
<td>Nutrient intake (fat + carbohydrate)</td>
<td>Blood / vagal afferent (nodose GLP-1R)</td>
<td>Body→brain</td>
<td><p>ARC</p>
<p>NTS</p>
<p>Brainstem</p></td>
<td><p>Pancreas</p>
<p>Stomach</p>
<p>Cardiac</p></td>
<td>GLP-1R</td>
<td>Satiety-promoting; glucose-dependent insulin support</td>
<td>Minutes–hours</td>
<td><p>arc_satiety</p>
<p>gastric_emptying_rate</p>
<p>meal_termination_signal</p>
<p>insulin_secretion</p></td>
<td><strong>A/B</strong></td>
<td>GLP-1 assays; drug exposure (agonists)</td>
<td>High priority</td>
<td><p>Keep endogenous GLP-1 and agonist drug exposure distinct</p>
<p>GLP-1R agonists: lean mass loss 25–40% (Tier A observation)</p></td>
</tr>
<tr class="even">
<td><strong>il1b_immune_alarm</strong></td>
<td>Cytokine</td>
<td>Immune cells (macrophages, microglia)</td>
<td>Infection, inflammation, tissue injury</td>
<td>Blood / humoral / vagal C-fibers</td>
<td>Body→brain</td>
<td><p>Hypothalamus</p>
<p>Amygdala</p>
<p>LC</p>
<p>Microglia-linked circuits</p></td>
<td>Immune system</td>
<td>IL-1R</td>
<td>Excitatory to sickness-state signaling</td>
<td>Minutes–hours</td>
<td><p>sickness_behavior_state</p>
<p>neuroinflammation_load</p>
<p>lc_tonic_gain</p>
<p>cytokine_load</p></td>
<td><strong>A/B</strong></td>
<td>Cytokine panel (IL-1β, IL-6, TNF-α)</td>
<td>High priority</td>
<td><p>Pair with TNF-α or IL-6 in later pass</p>
<p>SILO: separate literatures for vagal vs humoral routes</p></td>
</tr>
<tr class="odd">
<td><strong>il6_contextual</strong></td>
<td>Cytokine/myokine</td>
<td>Immune cells and exercising skeletal muscle</td>
<td>Inflammation OR exercise (different functions)</td>
<td>Blood</td>
<td>Body→brain</td>
<td><p>Hypothalamus</p>
<p>Hippocampus</p>
<p>Immune-brain pathways</p></td>
<td><p>Liver</p>
<p>Immune</p>
<p>Bone</p></td>
<td>IL-6R (gp130 signaling)</td>
<td>Context-dependent (pro/anti-inflammatory)</td>
<td>Minutes–hours</td>
<td><p>exercise_recovery_signal</p>
<p>inflammatory_load</p>
<p>fatigue_signal</p></td>
<td><strong>B</strong></td>
<td>IL-6 serum levels</td>
<td>Medium</td>
<td><p>Consider il6_exercise and il6_inflammatory as DISTINCT
signals</p>
<p>Anti-inflammatory in exercise context; pro-inflammatory in obesity/RA
context</p></td>
</tr>
<tr class="even">
<td><strong>osteocalcin_ucoc</strong></td>
<td>Hormone</td>
<td>Bone osteoblasts</td>
<td>Exercise load, mechanical loading, bone remodeling</td>
<td>Blood</td>
<td>Body→brain</td>
<td><p>Hippocampus (GPR158)</p>
<p>LC (possible)</p></td>
<td><p>Muscle (GPRC6A)</p>
<p>β-cells (GPRC6A)</p></td>
<td>GPR158 (brain); GPRC6A (muscle, β-cells)</td>
<td>Modulatory, pro-plasticity</td>
<td>Hours–days</td>
<td><p>osteocalcin_input_hpc</p>
<p>bdnf_support_hpc</p>
<p>monoamine_synthesis_rate</p>
<p>dg_neurogenesis_rate</p></td>
<td><strong>B/C</strong></td>
<td>Serum osteocalcin (ucOC fraction)</td>
<td>Medium-high</td>
<td><p>SILO-HPC-7: four exercise channels never co-measured in
humans</p>
<p>2024 MR study: causal link to AD risk via energy metabolism</p>
<p>Sedentary aging → osteocalcin ↓ (mechanostat below
threshold)</p></td>
</tr>
<tr class="odd">
<td><strong>irisin_exercise</strong></td>
<td>Myokine</td>
<td>Skeletal muscle (FNDC5 cleavage during exercise)</td>
<td>Exercise, muscle contraction; requires Hsp90α for receptor
activation</td>
<td>Blood</td>
<td>Body→brain</td>
<td>Hippocampus (αVβ5)</td>
<td><p>Bone osteocytes</p>
<p>Adipose</p></td>
<td>αVβ5 integrin (Hsp90α-activated)</td>
<td>Modulatory, pro-plasticity</td>
<td>Minutes–hours</td>
<td><p>irisin_input_hpc</p>
<p>hippocampal_plasticity_support</p>
<p>bone_wnt_support</p>
<p>adipose_browning</p></td>
<td><strong>B/C</strong></td>
<td>Circulating irisin (mass spectrometry validated)</td>
<td>Medium-high</td>
<td><p>Cryo-EM receptor mechanism confirmed 2023 (Kim et al.)</p>
<p>Lower in AD + MDD observationally</p>
<p>Keep translational uncertainty explicit; Tier C for clinical
causation</p></td>
</tr>
<tr class="even">
<td><strong>lactate_exercise</strong></td>
<td>Metabolite</td>
<td>Skeletal muscle (high-intensity exercise)</td>
<td>Moderate/high-intensity exercise; blood lactate 4–10 mM</td>
<td>Blood / MCT1/2 BBB transport</td>
<td>Body→brain</td>
<td><p>Hippocampus (HCAR1)</p>
<p>Cerebrovascular angiogenesis</p></td>
<td><p>Liver (Cori cycle)</p>
<p>Heart</p></td>
<td>HCAR1; MCT1/2 transporters; SIRT1-PGC-1α-FNDC5 pathway</td>
<td>Modulatory, energetic + signaling</td>
<td>Minutes (acute); months (chronic reserve)</td>
<td><p>lactate_signal</p>
<p>cerebrovascular_reserve</p>
<p>bdnf_support_hpc</p>
<p>hcar1_angiogenic_drive</p></td>
<td><strong>B/C</strong></td>
<td>Blood lactate; exercise intensity proxy</td>
<td>High priority</td>
<td><p>Good exercise-intensity carrier signal</p>
<p>Acute: BDNF augmentation (Tier B). Chronic: cerebrovascular reserve ↑
(Tier B). Direct hippocampal BDNF causal chain: Tier C</p>
<p>SILO-HPC-7: four exercise channels never co-measured</p></td>
</tr>
<tr class="odd">
<td><strong>baroreceptor_pressure</strong></td>
<td>Afferent stream</td>
<td>Carotid sinus, aortic arch (baroreceptors)</td>
<td>BP and pulse pressure changes</td>
<td>CN IX/X to NTS</td>
<td>Body→brain</td>
<td><p>NTS</p>
<p>LC</p>
<p>Insula</p>
<p>RVLM</p>
<p>Autonomic circuits</p></td>
<td><p>Heart</p>
<p>Vasculature</p></td>
<td>Stretch receptors (mechanoreceptors)</td>
<td>Fast corrective/homeostatic</td>
<td>Milliseconds–seconds</td>
<td><p>map_input</p>
<p>baroreflex_gain</p>
<p>autonomic_balance</p>
<p>hrv_proxy</p></td>
<td><strong>A</strong></td>
<td>BP; HRV; baroreflex sensitivity (BRS)</td>
<td>High priority</td>
<td><p>Right insular cortex lesions → cardiac arrhythmias</p>
<p>Core real-time cardiovascular stability signal</p>
<p>HRV = non-invasive brain-body integration proxy</p></td>
</tr>
<tr class="even">
<td><strong>osmolarity_ovlt_sfo</strong></td>
<td>Mechanical/chemical state</td>
<td>Blood plasma osmoreceptors (OVLT, SFO)</td>
<td>Hyperosmolarity, dehydration, sodium changes, Ang II</td>
<td>Circumventricular organs (outside BBB)</td>
<td>Body→brain</td>
<td><p>Hypothalamus (SON/PVN)</p>
<p>OVLT</p>
<p>SFO</p></td>
<td>Kidney via AVP output</td>
<td>Osmoreceptors; AT1R-linked (Ang II branch)</td>
<td>Homeostatic, thresholded</td>
<td>Seconds–minutes</td>
<td><p>osmotic_load</p>
<p>thirst_drive</p>
<p>avp_release_rate</p>
<p>raas_activation_index</p></td>
<td><strong>A</strong></td>
<td>Serum sodium; osmolality; AVP/copeptin</td>
<td>High priority</td>
<td><p>Tie closely to renal module</p>
<p>RAAS: Ang II → SFO/OVLT → thirst + SNS (concurrent with aldosterone →
Na⁺ retention)</p></td>
</tr>
<tr class="odd">
<td><strong>sex_steroid_e2_t</strong></td>
<td>Hormone</td>
<td>Gonads; brain aromatase (hippocampus, hypothalamus, amygdala)</td>
<td>HPG state, menstrual cycle, age, HRT/therapy</td>
<td>Blood and local brain synthesis</td>
<td>Body→brain (+ local)</td>
<td><p>Hippocampus CA1</p>
<p>Amygdala BLA</p>
<p>Raphe</p>
<p>vlPAG</p>
<p>LC</p></td>
<td><p>Bone</p>
<p>Muscle</p>
<p>Cardiovascular</p>
<p>Immune</p></td>
<td>ERα, ERβ, AR; membrane GPR30/GPER; non-genomic pathways</td>
<td>Modulatory, state-setting; dual timescale</td>
<td>Minutes (non-genomic); hours–days (genomic)</td>
<td><p>ltp_gain_ca1</p>
<p>ca1_spine_density</p>
<p>pain_threshold</p>
<p>raphe_5ht_support</p>
<p>da_tonic_vta</p>
<p>vlpag_efficiency</p></td>
<td><strong>A/B</strong></td>
<td>Serum E2/T + local brain synthesis (latent estimate)</td>
<td>Medium-high</td>
<td><p>Separate circulating from local brain aromatase synthesis</p>
<p>LTP_gain[CA1] = f(E2, DHEA, cortisol⁻¹) — three isolated
literatures</p>
<p>E2 loss → vlPAG efficiency ↓ (fibromyalgia perimenopause
mechanism)</p></td>
</tr>
<tr class="even">
<td><strong>allo_neurosteroid</strong></td>
<td>Neurosteroid</td>
<td>Brain-local (5α-reductase + 3α-HSD from progesterone); peripheral
progesterone</td>
<td>Progesterone state, stress, postpartum/perimenopause shifts</td>
<td>Local brain synthesis / blood</td>
<td>Body↔︎brain</td>
<td><p>Dentate gyrus</p>
<p>Amygdala</p>
<p>Cortical inhibitory networks</p></td>
<td>Limited peripheral relevance</td>
<td>GABA-A δ-subunit (extrasynaptic, tonic; NOT
benzodiazepine-sensitive)</td>
<td>Inhibitory/anxiolytic; DG sparsity gate</td>
<td>Seconds–minutes</td>
<td><p>dg_gaba_tonic_gate</p>
<p>anxiety_gain</p>
<p>pattern_separation_stability</p>
<p>gaba_tonic_inhibition_dg</p></td>
<td><strong>A/B</strong></td>
<td>Hard to measure directly; latent estimate from P4/ALLO assays;
brexanolone response</td>
<td>Medium-high</td>
<td><p>ALLO collapse (PPD, perimenopause) → DG hyperexcitability →
pattern separation degrades</p>
<p>Brexanolone (FDA-approved for PPD) targets this mechanism
directly</p>
<p>SILO-HPC-3: ALLO × cortisol × E2 during perimenopause — three
literatures, zero combined studies</p></td>
</tr>
<tr class="odd">
<td><strong>kynurenine_quin</strong></td>
<td>Metabolite (inflammatory)</td>
<td>IDO-activated tryptophan catabolism (immune cells, microglia)</td>
<td>Inflammation, chronic infection, stress + immune activation</td>
<td>Blood / brain IDO</td>
<td>Body→brain</td>
<td><p>Hippocampus (NMDA)</p>
<p>Cortex</p>
<p>BLA</p></td>
<td>Immune system</td>
<td>NR2B-containing NMDA receptors (excitotoxic agonist)</td>
<td>Excitatory, damaging (NMDA overdrive)</td>
<td>Hours–days (chronic)</td>
<td><p>kynurenine_load</p>
<p>nmda_excitotoxicity_risk_hpc</p>
<p>neuroinflammation_load</p>
<p>5ht_synthesis_rate</p></td>
<td><strong>B</strong></td>
<td>Serum kynurenine:tryptophan ratio; QUIN/KYNA ratio</td>
<td>Medium</td>
<td><p>Opposes cortisol: cortisol raises NMDA threshold; QUIN lowers it
— simultaneous = unpredictable net NMDA state</p>
<p>SILO-HPC-4: stress × inflammation NMDA literatures don’t
cross-cite</p>
<p>IDO → tryptophan diversion → 5-HT synthesis ↓ (same chain as
serotonin deficiency in MDD)</p></td>
</tr>
<tr class="even">
<td><strong>dhea_neurosteroid</strong></td>
<td>Neurosteroid</td>
<td>Adrenal zona reticularis; brain-local synthesis (CYP17A1)</td>
<td>Circadian rhythm (morning peak); age-dependent decline from ~25</td>
<td>Blood / local brain synthesis</td>
<td>Body→brain</td>
<td><p>Hippocampus</p>
<p>Amygdala</p>
<p>PFC</p></td>
<td>Peripheral AR/ER (weak)</td>
<td>σ1 receptor; NMDA facilitation (direct); partial GR antagonism</td>
<td>Partial anti-glucocorticoid; NMDA facilitatory; neuroprotective</td>
<td>Hours–days</td>
<td><p>ltp_gain_ca1</p>
<p>plasticity_suppression_offset</p>
<p>nmda_facilitation_dhea</p></td>
<td><strong>B</strong></td>
<td>Serum DHEA-S (may not reflect local brain DHEA)</td>
<td>Medium</td>
<td><p>Peak at age 25; ≤10–20% of peak by age 70 — most consistent aging
endocrine biomarker</p>
<p>LTP_gain[CA1] = f(E2, DHEA, cortisol⁻¹) — DHEA is middle term; rarely
co-measured</p>
<p>Peripheral DHEA-S measurement may not reflect local brain DHEA
levels</p></td>
</tr>
<tr class="odd">
<td><strong>thyroid_t3_brain</strong></td>
<td>Hormone (neurotropic)</td>
<td>Thyroid (T4) → brain D2 deiodinase (tanycytes, astrocytes) → T3
local</td>
<td>HPT axis; cortisol suppresses D1/D2; DIO1 T92A polymorphism</td>
<td>Blood T4 → BBB → regional D2 conversion</td>
<td>Body→brain</td>
<td><p>Hypothalamus (tanycytes)</p>
<p>Hippocampus</p>
<p>Cortex</p>
<p>Cerebellum</p></td>
<td><p>Heart (cardiac T3)</p>
<p>Liver</p></td>
<td>TRα, TRβ (nuclear thyroid hormone receptors)</td>
<td>Modulatory, metabolic rate, myelination</td>
<td>Hours–days</td>
<td><p>brain_t3_level</p>
<p>myelination_support</p>
<p>cognitive_metabolic_rate</p>
<p>creatine_phosphate_supply</p></td>
<td><strong>A/B</strong></td>
<td>TSH + free T4 (brain T3 not directly measurable; D2 activity
inferred)</td>
<td>Medium</td>
<td><p>Brain T3 regulation is REGIONALLY HETEROGENEOUS — each region has
independent D2 expression</p>
<p>Chronic cortisol suppresses D1/D2 → local T3 ↓ even with normal TSH
(explains cognitive/mood symptoms in chronic stress with “normal”
thyroid)</p>
<p>DIO1 T92A polymorphism → suboptimal brain T3 on levothyroxine
monotherapy</p></td>
</tr>
<tr class="even">
<td><strong>bdnf_peripheral</strong></td>
<td>Neurotrophin (peripheral)</td>
<td>Skeletal muscle type I fibers (pro-BDNF during exercise)</td>
<td>Exercise; lactate infusion augments</td>
<td>Blood (pro-BDNF cleavage → mature BDNF) / BBB</td>
<td>Body→brain</td>
<td><p>Hippocampus DG</p>
<p>CA1 (TrkB)</p></td>
<td>Motor neurons (retrograde NMJ)</td>
<td>TrkB (high-affinity); p75NTR (low-affinity, pro-apoptotic)</td>
<td>Pro-neurogenic, pro-plastic</td>
<td>Minutes (acute rise); weeks (structural)</td>
<td><p>bdnf_peripheral_circulating</p>
<p>dg_neurogenesis_rate</p>
<p>ltp_gain_ca1</p></td>
<td><strong>B</strong></td>
<td>Serum BDNF (partially reflects peripheral; brain BDNF not
accessible)</td>
<td>High priority</td>
<td><p>Separate from brain-synthesized BDNF and from IGF-1→BDNF
chain</p>
<p>Lactate infusion augments circulating mature BDNF response (Edman
2024, human)</p>
<p>SILO-HPC-7: four exercise channels never co-measured; this is Channel
3</p></td>
</tr>
<tr class="odd">
<td><strong>d2r_aging_motivation</strong></td>
<td>Receptor state (neuromodulatory)</td>
<td>Striatum (endogenous D2R expression; dopaminergic tone)</td>
<td>Aging (progressive decline ~1–2% per year); exercise may
attenuate</td>
<td>Endogenous receptor density (not a blood signal)</td>
<td>Internal (brain parameter)</td>
<td><p>Striatum (caudate/putamen)</p>
<p>NAcc</p></td>
<td>None</td>
<td>D2R (dopamine D2 receptor density)</td>
<td>Motivational salience of exercise and reward; declines with age</td>
<td>Years (slow accumulation)</td>
<td><p>d2r_density_striatum</p>
<p>exercise_motivation_modifier</p>
<p>reward_threshold_shift</p></td>
<td><strong>B</strong></td>
<td>PET [11C]raclopride (Volkow 1998 + follow-up studies)</td>
<td>Medium</td>
<td><p>D2R ↓ with aging → reduced motivational salience of exercise →
further inactivity (behavioral feedback loop)</p>
<p>Sedentary aging cascade: D2R decline is part of the motivation
arm</p>
<p>Not a blood signal — model as slowly-updating internal
parameter</p></td>
</tr>
<tr class="even">
<td><strong>opioid_vlpag</strong></td>
<td>Neuropeptide</td>
<td>Hypothalamus (β-endorphin); interneurons; adrenal medulla; released
by exercise</td>
<td>Pain, injury, intense exercise; HPG opioid tone</td>
<td>Local CNS; blood (peripheral)</td>
<td>Bidirectional</td>
<td><p>vlPAG</p>
<p>μ-opioid on NAcc</p>
<p>Hypothalamus (GnRH suppression)</p></td>
<td><p>ENS (motility ↓)</p>
<p>Immune (NK cells, T/B cells)</p></td>
<td>μ-, δ-, κ-opioid receptors</td>
<td>Analgesic, hedonic, HPG-suppressive at high load</td>
<td>Minutes (acute)</td>
<td><p>vlpag_efficiency</p>
<p>pain_threshold</p>
<p>gnrh_pulse_frequency_modifier</p>
<p>nacc_hedonic_value</p></td>
<td><strong>A/B</strong></td>
<td>Naloxone challenge; endorphin assays (limited)</td>
<td>Medium</td>
<td><p>High opioid load → GnRH suppression (athlete amenorrhea
mechanism)</p>
<p>vlPAG_efficiency = f(E2·ERβ, opioid_tone) — E2 and opioid tone
together</p>
<p>Exercise → opioid release → NAcc hedonic signal (exercise reward
feedback)</p></td>
</tr>
</tbody>
</table>

# Brain-Body Simulation Ontology Tables

## Signals · Brain Nodes · System Modules · Variable Schema

M. Finnegan · ORCID: 0009-0009-4921-7722 · v0.1 — March 2026 ·
Unpublished draft

This document is the typed ontology layer for the Brain-Body Unified
Reference (BrainBody v2.1). It defines three master tables — Signals,
Brain Nodes, and System Modules — plus a Variable Schema reference.
These tables will be exported as signals.csv, brain_nodes.csv, and
system_modules.csv when the full map series is complete. The
human-readable narrative layer is in
BrainBody_Unified_Reference_v2_1.docx and the full FQ decompositions are
in the individual Brain Maps and Organ System Maps.

Schema is based on the template developed in collaboration with ChatGPT
(March 2026) and extended with content from the Brain Map series (v2.0),
Peripheral Maps (v1.0), Organ System Maps (v1.0), and
Musculoskeletal_v1_0 paper. SILO gaps are annotated in the Notes column
where the map series has documented them.

### Variable Schema Reference

Every state variable in the model must conform to this schema. Apply to
all variables listed in the State_Variables_Affected and Internal_State
columns above.

<table>
<colgroup>
<col style="width: 14%" />
<col style="width: 9%" />
<col style="width: 12%" />
<col style="width: 9%" />
<col style="width: 12%" />
<col style="width: 10%" />
<col style="width: 14%" />
<col style="width: 14%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Variable</strong></td>
<td><strong>Type</strong></td>
<td><strong>Units / Range</strong></td>
<td><strong>Timescale</strong></td>
<td><strong>Depends_On</strong></td>
<td><strong>Update_Form</strong></td>
<td><strong>Observable_Proxy</strong></td>
<td><strong>Status</strong></td>
</tr>
<tr class="even">
<td><strong>ltp_gain_ca1</strong></td>
<td>Latent</td>
<td>Normalized 0–3.0; setpoint ~1.0</td>
<td>Slow (hours–days)</td>
<td><p>E2_level</p>
<p>DHEA_level</p>
<p>cortisol_load</p></td>
<td>Weighted nonlinear; E2 and DHEA oppose cortisol</td>
<td>fMRI encoding proxy; memory task performance</td>
<td><strong>A/B</strong></td>
</tr>
<tr class="odd">
<td><strong>dg_neurogenesis_rate</strong></td>
<td>Latent</td>
<td>Normalized 0–1.0</td>
<td>Slow (weeks)</td>
<td><p>bdnf_total</p>
<p>igf1_signal</p>
<p>cortisol_load</p>
<p>allo_level</p>
<p>microglial_bdnf</p></td>
<td>Weighted nonlinear decay/growth</td>
<td>MRI DG volume proxy; serum BDNF correlate</td>
<td><strong>B/C</strong></td>
</tr>
<tr class="even">
<td><strong>hpa_feedback_strength</strong></td>
<td>Latent</td>
<td>Normalized 0–1.0</td>
<td>Slow (weeks–months)</td>
<td><p>cortisol_history</p>
<p>gr_sensitivity_subiculum</p>
<p>ca1_health</p></td>
<td>GR downregulation under chronic cortisol; partially reversible with
sleep</td>
<td>Cortisol diurnal slope; dexamethasone suppression test</td>
<td><strong>A</strong></td>
</tr>
<tr class="odd">
<td><strong>cortisol_load</strong></td>
<td>Estimated</td>
<td>nmol/L equivalent; normalized</td>
<td>Medium (hours)</td>
<td><p>cortisol_pulse</p>
<p>clearance_rate</p></td>
<td>Integrate cortisol_pulse over time with decay</td>
<td>Salivary cortisol AUC; diurnal slope</td>
<td><strong>A</strong></td>
</tr>
<tr class="even">
<td><strong>ne_tonic_baseline</strong></td>
<td>Latent</td>
<td>Normalized 0–1.0</td>
<td>Medium (minutes–hours)</td>
<td><p>E2_level</p>
<p>IL1b_load</p>
<p>adenosine_load</p>
<p>orexin_level</p>
<p>baroreceptor_input</p>
<p>NPY_reserve</p></td>
<td>Six-input weighted sum (all inputs siloed in literature)</td>
<td>HRV; pupillometry; skin conductance</td>
<td><strong>B</strong></td>
</tr>
<tr class="odd">
<td><strong>vagal_tone</strong></td>
<td>Estimated</td>
<td>Normalized; HRV-anchored</td>
<td>Fast (seconds) to slow (days)</td>
<td><p>baroreceptor_input</p>
<p>vagal_afferent_state</p>
<p>parasympathetic_drive</p></td>
<td>Real-time from HRV; slow component reflects training</td>
<td>HRV SDNN, RMSSD; RSA amplitude</td>
<td><strong>A</strong></td>
</tr>
<tr class="even">
<td><strong>arc_satiety</strong></td>
<td>Derived</td>
<td>Normalized 0–1.0</td>
<td>Medium (minutes–hours)</td>
<td><p>leptin_signal</p>
<p>insulin_signal</p>
<p>GLP1_signal</p>
<p>ghrelin_level</p></td>
<td>f(leptin, insulin, GLP-1, ghrelin⁻¹)</td>
<td>Self-reported satiety; food intake; indirect imaging</td>
<td><strong>A/B</strong></td>
</tr>
<tr class="odd">
<td><strong>brain_insulin_resistance_index</strong></td>
<td>Latent</td>
<td>0–1.0 (0=sensitive, 1=resistant)</td>
<td>Slow (months–years)</td>
<td><p>peripheral_insulin_resistance</p>
<p>bmi</p>
<p>inflammation_load</p>
<p>cortisol_load</p></td>
<td>Slow drift; partially reversible with exercise</td>
<td>HOMA-IR proxy; cognitive insulin sensitivity assays</td>
<td><strong>B</strong></td>
</tr>
<tr class="even">
<td><strong>vlpag_efficiency</strong></td>
<td>Latent</td>
<td>Normalized 0–1.0</td>
<td>Medium (hours–days)</td>
<td><p>E2_level</p>
<p>opioid_tone</p>
<p>descending_5ht_ne</p></td>
<td>f(E2·ERβ, opioid_tone)</td>
<td>Pain threshold testing; conditioned pain modulation (CPM)</td>
<td><strong>A/B</strong></td>
</tr>
<tr class="odd">
<td><strong>cerebrovascular_reserve</strong></td>
<td>Latent</td>
<td>0.5–1.5; setpoint 1.0</td>
<td>Slow (months–years)</td>
<td><p>lactate_chronic_exposure</p>
<p>exercise_frequency</p>
<p>aging</p></td>
<td>HCAR1-driven angiogenesis; slow growth with training; slow decay
with inactivity</td>
<td>fMRI CBF; cerebrovascular reactivity (CVR) testing</td>
<td><strong>B</strong></td>
</tr>
</tbody>
</table>

Types: Observed = directly measured; Estimated = inferred from measured
proxies; Latent = not directly measurable (inferred); Derived = computed
from other variables. Timescales: Fast = seconds–minutes; Medium =
minutes–hours; Slow = hours–months.

### Table 2 — Brain Nodes

Seven core brain nodes with body inputs, internal state variables,
outputs, and failure modes. Content from BrainMap v2.0 series. \[v0.1 =
starter set; additional nodes (ACC, BNST, basal ganglia, etc.) to be
added in v0.2+\]

<table>
<colgroup>
<col style="width: 12%" />
<col style="width: 8%" />
<col style="width: 16%" />
<col style="width: 14%" />
<col style="width: 14%" />
<col style="width: 12%" />
<col style="width: 11%" />
<col style="width: 5%" />
<col style="width: 3%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Node_ID</strong></td>
<td><strong>Node_Class</strong></td>
<td><strong>Primary_Function</strong></td>
<td><strong>Body_Inputs</strong></td>
<td><strong>Internal_State</strong></td>
<td><strong>Output_Variables</strong></td>
<td><strong>Failure_Modes</strong></td>
<td><strong>Tier</strong></td>
<td><strong>Status</strong></td>
</tr>
<tr class="even">
<td><strong>hippocampus_ca1_dg</strong></td>
<td>Memory / plasticity integrator</td>
<td>Converts endocrine, metabolic, exercise, and stress signals into
memory encoding quality and HPA feedback support</td>
<td><p>cortisol_hpa (GR ↓ LTP)</p>
<p>sex_steroid_e2_t (CA1 spine density)</p>
<p>allo_neurosteroid (DG GABA tonic)</p>
<p>osteocalcin_ucoc (GPR158 → BDNF)</p>
<p>irisin_exercise (αVβ5)</p>
<p>bdnf_peripheral (TrkB)</p>
<p>lactate_exercise (HCAR1)</p>
<p>insulin_brain (AMPA trafficking)</p>
<p>kynurenine_quin (NMDA excitotoxicity)</p>
<p>dhea_neurosteroid (LTP support)</p></td>
<td><p>ltp_gain_ca1</p>
<p>dg_neurogenesis_rate</p>
<p>stress_load_hpc</p>
<p>ca1_spine_density</p>
<p>gaba_tonic_inhibition_dg</p>
<p>hpa_negative_feedback_strength</p>
<p>nmda_excitotoxicity_risk</p>
<p>cerebrovascular_reserve</p></td>
<td><p>memory_encoding_quality</p>
<p>context_discrimination</p>
<p>hpa_feedback_strength (subiculum → PVN)</p>
<p>ca1_vmPFC_projection (safety memory)</p></td>
<td><p>Chronic cortisol → CA3 retraction, DG neurogenesis ↓</p>
<p>Inactivity → all 4 exercise channels ↓ simultaneously</p>
<p>Inflammation → QUIN → NMDA excitotoxicity</p>
<p>E2 loss → LTP_gain ↓; ALLO collapse → DG hyperexcitable</p>
<p>Alzheimer’s: ACh depletion → encoding mode fails</p></td>
<td><strong>A/B/C</strong></td>
<td>High priority</td>
</tr>
<tr class="odd">
<td><strong>hypothalamus_pvn_arc_scn</strong></td>
<td>Controller / homeostat</td>
<td>Integrates all blood-borne body state signals and issues endocrine
and autonomic commands to maintain homeostasis</td>
<td><p>osmolarity_ovlt_sfo (thirst, AVP)</p>
<p>insulin_brain (ARC satiety)</p>
<p>leptin_adiposity (POMC activation)</p>
<p>ghrelin_hunger (NPY/AgRP)</p>
<p>glp1_gut_satiety (ARC + NTS)</p>
<p>cortisol_hpa (CRH feedback)</p>
<p>il1b_immune_alarm (fever center)</p>
<p>sex_steroid_e2_t (HPG feedback)</p></td>
<td><p>crh_release_rate</p>
<p>arc_satiety</p>
<p>avp_release_rate</p>
<p>circadian_phase</p>
<p>orexin_level</p>
<p>gnrh_pulse_frequency</p></td>
<td><p>hpa_drive (CRH → ACTH → cortisol)</p>
<p>hpg_drive (GnRH)</p>
<p>hpt_drive (TRH)</p>
<p>thirst_drive</p>
<p>autonomic_setpoint (IML preganglionic)</p></td>
<td><p>Stress lock-in (CRH/cortisol runaway)</p>
<p>Obesity (leptin resistance → ARC dysregulation)</p>
<p>Sleep disruption (SCN/circadian decoupling)</p>
<p>E2 loss (menopausal thermostat instability)</p></td>
<td><strong>A</strong></td>
<td>High priority</td>
</tr>
<tr class="even">
<td><strong>amygdala_bla_cea_itc</strong></td>
<td>Salience / threat controller</td>
<td>Tags body and context signals with emotional threat or safety value;
gates fear learning and extinction</td>
<td><p>cortisol_hpa (BLA sensitization via GR)</p>
<p>il1b_immune_alarm (BLA hyperactivation)</p>
<p>sex_steroid_e2_t (ERα on BLA → reactivity)</p>
<p>opioid_vlpag (hedonic/threat modulation)</p></td>
<td><p>bla_reactivity</p>
<p>threat_response_threshold</p>
<p>itc_gate_strength</p>
<p>bnst_anxiety_state</p></td>
<td><p>threat_bias</p>
<p>hpa_activation_bias (CeA → PVN)</p>
<p>autonomic_defense_bias (CeA → PAG, LC)</p>
<p>hippocampus_context_tag (emotional memory)</p></td>
<td><p>Chronic stress + cortisol → BLA sensitization, ITC gate
failure</p>
<p>Inflammation → BLA hyperreactivity</p>
<p>E2 loss → amygdala reactivity ↑ (OTR sensitivity loss is 9th E2
withdrawal arm)</p>
<p>PTSD: over-encoded fear attractor in CA3</p></td>
<td><strong>A/B</strong></td>
<td>High priority</td>
</tr>
<tr class="odd">
<td><strong>insula_posterior_anterior</strong></td>
<td>Interoceptive state estimator</td>
<td>Builds running representation of whole-body state; outputs salience
and urgency to decision and emotion circuits</td>
<td><p>vagal_afferent (gut/cardiac/respiratory state)</p>
<p>baroreceptor_pressure (cardiac interoception)</p>
<p>pain afferents (C-fibers → spinothalamic)</p>
<p>cortisol + NE (amplify interoceptive salience)</p></td>
<td><p>body_state_signal_strength</p>
<p>interoceptive_salience</p>
<p>ainsula_pfc_coupling</p>
<p>ainsula_bla_coupling</p></td>
<td><p>body_state_summary (to PFC/ACC for decisions)</p>
<p>subjective_urgency</p>
<p>interoceptive_precision</p>
<p>cardiac arrhythmias (right insula lesion effect)</p></td>
<td><p>Panic amplification (interoceptive salience ↑ with threat
loop)</p>
<p>Low precision (alexithymia)</p>
<p>Autonomic misreadout (insula damage → cardiac arrhythmias)</p></td>
<td><strong>A/B</strong></td>
<td>High priority</td>
</tr>
<tr class="even">
<td><strong>locus_coeruleus</strong></td>
<td>Global arousal broadcaster</td>
<td>Converts body alarm signals and state uncertainty into NE tone and
phasic gain for all brain regions</td>
<td><p>baroreceptor_pressure (blood pressure via NTS)</p>
<p>il1b_immune_alarm (NE release)</p>
<p>sex_steroid_e2_t (E2 → increased LC baseline firing)</p>
<p>hypoxia (direct activation)</p>
<p>opioid_vlpag (opioid ↓ LC tone)</p></td>
<td><p>ne_tonic_baseline = f(E2, IL-1β, adenosine_load⁻¹, orexin,
baroreceptor, NPY_reserve)</p>
<p>ne_phasic_gain</p></td>
<td><p>global_arousal (NE broadcast to all cortical regions)</p>
<p>salience_gain (SNR sharpening, inverted-U)</p>
<p>melatonin_onset_delay = f(NE_tonic)</p>
<p>glymphatic_clearance ↑ when NE_tonic ↓ (sleep)</p>
<p>microglial pruning (NE_tonic ↓ permissive)</p></td>
<td><p>Hypervigilance (NE_tonic chronically elevated)</p>
<p>Sleep fragmentation (NE_tonic insufficient drop)</p>
<p>Inflammatory overdrive (IL-1β → LC chronically elevated)</p></td>
<td><strong>A/B</strong></td>
<td>High priority</td>
</tr>
<tr class="odd">
<td><strong>pag_vlpag_dpag</strong></td>
<td>Defense / pain coordinator</td>
<td>Couples threat state to fight-flight-freeze selection and descending
analgesia; E2-sensitive pain gate</td>
<td><p>sex_steroid_e2_t (ERβ on vlPAG → descending analgesia
efficiency)</p>
<p>opioid_vlpag (μ-opioid disinhibition)</p>
<p>pain afferents from periphery</p></td>
<td><p>vlpag_efficiency = f(E2·ERβ, opioid_tone)</p>
<p>pain_threshold</p>
<p>defense_mode</p></td>
<td><p>descending_analgesia (vlPAG → Raphe Magnus → dorsal horn)</p>
<p>defense_pattern (dPAG → fight/flight; vlPAG → freeze/submit)</p>
<p>cardioinhibitory_bias (vlPAG → vagal)</p></td>
<td><p>E2 loss → vlPAG efficiency ↓ → fibromyalgia, central
sensitization</p>
<p>Chronic pain → opioid tolerance → analgesia failure</p>
<p>Overdefense (CeA hyperactivation → PAG freeze locked)</p></td>
<td><strong>A/B</strong></td>
<td>Medium-high</td>
</tr>
<tr class="even">
<td><strong>vta_mesolimbic</strong></td>
<td>Motivation / reward node</td>
<td>Converts metabolic, hormonal, and experiential signals into
motivation, reward prediction error, and effort allocation</td>
<td><p>leptin_adiposity (DA tone ↑)</p>
<p>ghrelin_hunger (phasic DA ↑ food craving)</p>
<p>opioid_vlpag (μ-opioid → hedonic)</p>
<p>sex_steroid_e2_t (E2 + T modulate D1/D2)</p>
<p>d2r_aging_motivation (receptor density modifier)</p></td>
<td><p>da_tonic_vta = f(leptin, opioid_tone, E2)</p>
<p>reward_prediction_error_gain</p>
<p>motivational_drive</p>
<p>d2r_density_striatum</p></td>
<td><p>approach_bias (NAcc DA)</p>
<p>reward_salience</p>
<p>effort_willingness</p>
<p>exercise_reward_signal</p></td>
<td><p>Anhedonia (DA_tonic ↓; leptin resistance)</p>
<p>Addiction bias (D2R downregulation → reward threshold ↑ → more
needed)</p>
<p>Low exercise motivation (D2R ↓ aging + inactivity loop)</p></td>
<td><strong>A/B</strong></td>
<td>High priority</td>
</tr>
<tr class="odd">
<td><strong>raphe_5ht</strong></td>
<td>Mood stabilizer / descending modulator</td>
<td>Generates 5-HT tone for cortical mood stability, impulse control,
and descending pain modulation; E2-sensitive</td>
<td><p>sex_steroid_e2_t (ERβ → 5-HT synthesis ↑, MAO-B inhibition)</p>
<p>il1b_immune_alarm (IDO activation → tryptophan diversion → 5-HT
synthesis ↓)</p>
<p>kynurenine_quin (same IDO pathway)</p>
<p>gut tryptophan via LAT1 BBB transport (rate-limiting
substrate)</p></td>
<td><p>5ht_synthesis_rate = f(tryptophan_BBB, IDO_activity⁻¹,
E2·ERβ)</p>
<p>serotonin_reuptake_rate</p></td>
<td><p>mood_stability (cortical 5-HT)</p>
<p>descending_analgesia_efficiency (5-HT contribution via dorsal
horn)</p>
<p>gi_motility (raphe spinal pathway)</p>
<p>bnst_anxiety_tone</p></td>
<td><p>E2 withdrawal → 5-HT synthesis ↓ → new-onset depression at
perimenopause</p>
<p>Inflammation → IDO → tryptophan → QUIN (not 5-HT) → neuroinflammation
+ 5-HT floor</p>
<p>Peripheral 5-HT (enterochromaffin) does NOT contribute — tryptophan
is the actual substrate crossing BBB</p></td>
<td><strong>A</strong></td>
<td>High priority</td>
</tr>
</tbody>
</table>

### Table 3 — System Modules

Seven core body system modules with brain interface channels, endocrine
outputs, key brain-relevant variables, and major feedback loops. Content
from Organ System Maps v1.0 series.

<table>
<colgroup>
<col style="width: 12%" />
<col style="width: 9%" />
<col style="width: 17%" />
<col style="width: 13%" />
<col style="width: 12%" />
<col style="width: 11%" />
<col style="width: 8%" />
<col style="width: 8%" />
<col style="width: 5%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Module_ID</strong></td>
<td><strong>Biological_Scope</strong></td>
<td><strong>Sensors_to_Brain</strong></td>
<td><strong>Brain_to_System_Outputs</strong></td>
<td><strong>Endocrine_Outputs</strong></td>
<td><strong>Brain_Relevant_Variables</strong></td>
<td><strong>Major_Feedback_Loops</strong></td>
<td><strong>Coupling_Partners</strong></td>
<td><strong>Priority</strong></td>
</tr>
<tr class="even">
<td><strong>hpa_axis</strong></td>
<td>PVN-pituitary-adrenal stress axis</td>
<td><p>Cortisol blood-borne feedback (GR: hippocampus, pituitary)</p>
<p>Threat-state inputs via amygdala/PFC/hippocampus → PVN</p>
<p>IL-1β CRH activation (immune arm)</p></td>
<td><p>CRH-ACTH-cortisol secretion (HPA cascade)</p>
<p>HPA feedback modulation from hippocampus subiculum</p>
<p>NE amplifies cortisol at PVN (LC → PVN cross-axis)</p></td>
<td><p>Cortisol (glucocorticoid)</p>
<p>DHEA (concurrent adrenal; partial GC buffer)</p></td>
<td><p>cortisol_load</p>
<p>hpa_feedback_strength</p>
<p>crh_release_rate</p></td>
<td><p>Stress → cortisol → hippocampal GR → HPA brake (negative)</p>
<p>Chronic cortisol → hippocampal damage → brake fails → runaway
(positive failure loop)</p>
<p>Cortisol → HPT: D1/D2 suppression → T3 ↓ (cross-axis)</p></td>
<td>Immune, HPT, HPG, Metabolic, Musculoskeletal</td>
<td>High</td>
</tr>
<tr class="odd">
<td><strong>vagal_interoceptive</strong></td>
<td>Vagus nerve and NTS-centered afferent body reporting</td>
<td><p>Gut distension + chemoreceptors → NTS</p>
<p>Baroreceptors (cardiac/vascular) → NTS</p>
<p>Pulmonary stretch (Hering-Breuer) → NTS</p>
<p>Vagal immune-afferent (C-fibers from inflamed tissue) → NTS</p></td>
<td><p>Parasympathetic tone: heart (M2), gut (M3), liver, pancreas</p>
<p>Cholinergic anti-inflammatory reflex: vagal → splenic α7 nAChR →
TNF-α suppression</p></td>
<td><p>ACh (vagal efferent, peripheral)</p>
<p>No systemic hormones (neural only)</p></td>
<td><p>vagal_tone</p>
<p>body_state_signal_strength</p>
<p>baroreflex_gain</p></td>
<td><p>Body state → NTS/insula/hypothalamus → parasympathetic
correction</p>
<p>Inflammation → vagal afferent → sickness behavior (brain
response)</p>
<p>HRV as real-time readout of loop integrity</p></td>
<td>Cardiovascular, Gut, Immune, Respiratory</td>
<td>High</td>
</tr>
<tr class="even">
<td><strong>metabolic_insulin</strong></td>
<td>Pancreas, adipose, glucose-energy regulation (hepatic included)</td>
<td><p>Glucose/insulin → BBB → hippocampus/ARC (brain insulin)</p>
<p>Leptin (adipose signal) → ARC POMC/NPY</p>
<p>Ghrelin (gastric) → ARC/VTA</p>
<p>GLP-1 (L-cells) → vagal nodose + ARC</p>
<p>Hepatic vagal afferents → NTS (portal glucose sensing)</p></td>
<td><p>ARC NPY/AgRP: food-seeking behavior</p>
<p>HPA cortisol → hepatic gluconeogenesis ↑</p>
<p>Vagal efferents → pancreas (cephalic-phase insulin)</p>
<p>VTA DA → hedonic eating reward</p></td>
<td><p>Insulin</p>
<p>Glucagon</p>
<p>Leptin</p>
<p>Ghrelin</p>
<p>GLP-1/GIP (incretins)</p></td>
<td><p>brain_insulin_signal</p>
<p>arc_satiety</p>
<p>leptin_resistance_index</p>
<p>da_tonic_vta</p>
<p>brain_insulin_resistance_index</p></td>
<td><p>Energy state → hypothalamus/VTA → intake and endocrine
adjustment</p>
<p>T2D → brain insulin resistance → hippocampal LTP ↓ → memory failure
(no loop correction available)</p>
<p>VTA D2R downregulation → reward threshold ↑ →
overconsumption</p></td>
<td>HPA, HPG, Liver, VTA, Hippocampus, Cardiovascular</td>
<td>High</td>
</tr>
<tr class="odd">
<td><strong>immune_brain</strong></td>
<td>Peripheral immune signaling and neuroimmune coupling</td>
<td><p>IL-1β, TNF-α, IL-6 → circumventricular organs (outside BBB)</p>
<p>Vagal C-fibers → NTS (parallel immune reporting)</p>
<p>IDO activation → kynurenine → QUIN (NMDA arm)</p>
<p>PGE2 → hypothalamus EP3/4 (fever)</p></td>
<td><p>HPA cortisol → systemic immunosuppression (GR on all immune
cells)</p>
<p>Cholinergic anti-inflammatory reflex (via vagal module)</p>
<p>SNS → splenic NE → acute immune priming</p></td>
<td><p>IL-1β, IL-6, TNF-α (pro-inflammatory)</p>
<p>IL-10, TGF-β (anti-inflammatory)</p>
<p>PGE2 (fever mediator)</p></td>
<td><p>neuroinflammation_load</p>
<p>sickness_behavior_state</p>
<p>cytokine_load</p>
<p>kynurenine_load</p>
<p>microglial_m1_m2_ratio</p></td>
<td><p>Inflammation → brain sickness state → HPA/ANS immune modulation
(negative homeostatic)</p>
<p>Chronic inflammation → kynurenine → NMDA excitotoxicity + 5-HT ↓
(non-resolving positive damage loop)</p></td>
<td>HPA, LC, Amygdala, Hippocampus, Vagal</td>
<td>High</td>
</tr>
<tr class="even">
<td><strong>musculoskeletal_exercise</strong></td>
<td>Skeletal muscle, bone, exercise endocrine architecture</td>
<td><p>Proprioception (DRG → spinocerebellar/cortical)</p>
<p>Lactate (blood 4–10 mM → HCAR1 brain)</p>
<p>Exercise intensity (peripheral fatigue signals)</p>
<p>Osteocalcin ↑ (bone mechanostat activation)</p>
<p>Irisin ↑ (muscle FNDC5 cleavage)</p>
<p>Peripheral BDNF ↑ (muscle type I fibers)</p></td>
<td><p>Motor cortex + SMA: voluntary movement</p>
<p>Cerebellum: error correction</p>
<p>Hypothalamus: GH/IGF-1 pulsatile release → anabolic support</p>
<p>D2R (striatum): motivational reinforcement for future
exercise</p></td>
<td><p>Osteocalcin (ucOC)</p>
<p>Irisin</p>
<p>IL-6 (exercise context)</p>
<p>FGF21 (muscle)</p>
<p>Peripheral BDNF</p>
<p>IGF-1 (local muscle + systemic)</p></td>
<td><p>exercise_state</p>
<p>lactate_signal</p>
<p>osteocalcin_input_hpc</p>
<p>irisin_input_hpc</p>
<p>bdnf_peripheral_circulating</p>
<p>fatigue_signal</p>
<p>cerebrovascular_reserve</p>
<p>d2r_density_striatum</p></td>
<td><p>Exercise → endocrine support → hippocampal plasticity →
motivation preservation → future exercise capacity (positive health
loop)</p>
<p>Inactivity → all 4 brain channels ↓ simultaneously + D2R ↓ → further
inactivity (negative spiral loop)</p>
<p>SILO-HPC-7: four channels never co-measured in humans</p></td>
<td>Hippocampus, Metabolic, Cardiovascular, HPA, VTA</td>
<td>High</td>
</tr>
<tr class="odd">
<td><strong>cardiovascular_baroreflex</strong></td>
<td>Heart, vessels, pressure regulation; cardiac afferent reporting</td>
<td><p>Baroreceptors → CN IX/X → NTS (primary real-time signal)</p>
<p>BNP/ANP (cardiac wall stress) → circumventricular organs</p>
<p>Ischemic cardiac pain → C-fibers → spinal → thalamus → insula</p>
<p>HRV (non-invasive ANS balance readout)</p></td>
<td><p>PVN → IML → stellate ganglion (SNS cardiac drive)</p>
<p>PAG → nucleus ambiguus (vagal cardiac modulation)</p>
<p>HPA → adrenal medulla → epinephrine (humoral stress
response)</p></td>
<td><p>BNP/ANP (wall stress signal)</p>
<p>Epinephrine (adrenal medulla, stress)</p>
<p>Renin/Ang II (RAAS initiation)</p></td>
<td><p>map_input</p>
<p>baroreflex_gain</p>
<p>autonomic_balance</p>
<p>hrv_proxy</p>
<p>vagal_tone</p></td>
<td><p>BP change → baroreflex → autonomic correction (negative
homeostatic; setpoint ±10 mmHg)</p>
<p>Right insula damage → cardiac arrhythmias (brain → cardiac
coupling)</p></td>
<td>LC, Insula, Renal, Vagal, HPA</td>
<td>High</td>
</tr>
<tr class="even">
<td><strong>renal_osmotic</strong></td>
<td>Kidney-fluid-electrolyte control; RAAS; AVP axis</td>
<td><p>Osmoreceptors (OVLT/SFO) → hypothalamus (thirst, AVP)</p>
<p>Cardiopulmonary volume receptors → vagal → NTS → hypothalamus</p>
<p>Ang II → AT1R at SFO/OVLT (RAAS-brain coupling)</p>
<p>Aldosterone (MR on hippocampus: GR/MR ratio)</p></td>
<td><p>ADH/AVP → renal AQP2 → water reabsorption</p>
<p>RVLM: sympathetic outflow to renal nerves (renin secretion)</p>
<p>Thirst behavior (hypothalamus → water-seeking)</p></td>
<td><p>ADH/AVP</p>
<p>Aldosterone (mineralocorticoid)</p>
<p>Renin/Ang II</p>
<p>Erythropoietin (EPO; neuroprotective at brain EPO-R — Tier
B)</p></td>
<td><p>osmotic_load</p>
<p>thirst_drive</p>
<p>avp_release_rate</p>
<p>raas_activation_index</p></td>
<td><p>Osmotic change → thirst/AVP → renal correction (negative
homeostatic)</p>
<p>RAAS over-activation → aldosterone → hippocampal MR over-activation →
HPA sensitization (pathological positive loop in hypertension)</p></td>
<td>Hypothalamus, Cardiovascular, HPA, Vagal</td>
<td>Medium-high</td>
</tr>
</tbody>
</table>

All papers in this series are unpublished drafts. Not yet peer reviewed.
Internal reference document.
