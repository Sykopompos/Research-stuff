# The Endocrine System as a Distributed Detection Architecture

*Axes, Cross-Axis Interactions, and the Integrated Hormonal Operating System*

**M. Finnegan** · v1.1 — March 2026 · *Unpublished draft, not yet peer reviewed*


> **Article Scope and Companion References:** Article Scope and Companion References: This paper is an integrative review proposing a functional framework for the endocrine system organized around five coupled feedback axes and their cross-axis interactions. Brain-interface effects of each hormone are covered in a companion reference (The Brain-Body System: A Unified Reference for Medicine, BrainBody v1.3) and cited here rather than duplicated. The five-operation decomposition (Propagation, Gating, Detection, Accumulation, Refinement) is used as an organizing device to locate control logic within each axis — it is an analytical scaffold, not a theoretical claim. Evidence confidence tiers are specified at the end of §1.


## Abstract

Endocrine physiology is routinely organized by anatomical source —
thyroid, adrenal, gonad, pancreas. This scheme identifies effector
organs but does not describe the control topology. Describing the
endocrine system as a set of independent glands obscures the feedback
architecture within each axis and the cross-axis coupling that
determines the actual hormonal operating state.

This paper proposes a five-axis functional framework: HPA, HPG, HPT,
metabolic (pancreatic islets), and circadian (SCN-pineal). Each axis is
analyzed as a negative feedback detection system using five operations —
propagation, gating, detection, accumulation, and refinement — used here
as an analytical scaffold rather than a theoretical claim. The five axes
share relay infrastructure and receptor populations, and regulate each
other's sensitivity through direct molecular mechanisms.

The paper's primary contribution is the cross-axis interaction map and
the identification of multi-axis failure cascades that emerge from
coupling. Clinical presentations that appear single-axis — functional
hypogonadism under chronic stress, euthyroid sick syndrome,
metabolic-cognitive decline — are shown to reflect propagation through
the interaction network rather than isolated axis failure. Evidence
confidence is tiered throughout; cross-axis mechanisms with only rodent
support and integrative cascade hypotheses are distinguished from
established consensus.

## §1 — The Endocrine System as Coupled Feedback Axes

The endocrine system is commonly described in terms of its anatomical
components: the thyroid gland produces thyroid hormone; the adrenal
gland produces cortisol; the gonads produce sex steroids. This
description accurately identifies the effector organs but does not
capture the control topology.

Three classical axes share a common organization: a hypothalamic
releasing hormone drives pituitary secretion, which drives peripheral
gland output, which feeds back to suppress the hypothalamic and
pituitary nodes. The effector gland is the output stage of the axis, not
the system itself \[1, 2\]. Two additional axes — the metabolic axis
(pancreatic islets) and the circadian axis (SCN-pineal) — implement the
same functional organization (sensor, error signal, effector, feedback)
through different anatomical substrates that bypass the pituitary
entirely.

The five axes covered here:

- HPA: CRH (PVN) → ACTH (corticotrophs) → cortisol (adrenal ZF) → GR
  feedback at hippocampus, PVN, and pituitary

- HPG: GnRH (ARC/AVPV) → LH/FSH (gonadotrophs) → sex steroids (gonad) →
  ER/AR feedback at hypothalamus and pituitary

- HPT: TRH (PVN) → TSH (thyrotrophs) → T4/T3 (thyroid follicular cells)
  → TR feedback at hypothalamus and pituitary

- Metabolic: Portal glucose → insulin/glucagon (pancreatic islets) →
  peripheral glucose uptake → blood glucose feedback to islets directly

- Circadian: Environmental light-dark → ipRGCs → SCN → sympathetic NE →
  melatonin (pineal) → MT1 feedback at SCN

These five axes share relay infrastructure (hypothalamus, pituitary,
hippocampus) and compete for the same receptor populations at multiple
sites. Perturbation of any single axis can propagate to others through
these shared nodes \[3, 4\].

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Evidence Tiers — Scope and Confidence of
Claims</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong>Note: These tiers reflect the confidence with which claims
are used within this review. They are not a formal evidence-grading
system (e.g., GRADE) and should not be read as one. Reviewers may
reasonably disagree on individual assignments.</strong></td>
</tr>
<tr class="even">
<td><p><strong>Tier A — Established consensus (well-replicated,
textbook-level):</strong></p>
<p>HPA negative feedback via hippocampal GR; cortisol inhibition of D1
deiodinase producing rT3; SHBG as HPG-HPT bridge; beta cell two-phase
insulin secretion with incretin amplification accounting for 50-70% of
oral glucose response; melatonin as photoperiod signal via SCN.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Tier B — Cross-axis mechanisms with direct experimental
support:</strong></p>
<p>Glucocorticoid suppression of Kiss1 in ARC KNDy neurons (mouse, [47])
— Tier A in mechanistic principle, Tier B in human translation;
estradiol modulation of hippocampal GR sensitivity (rodent and human);
brain-local estradiol synthesis via aromatase; estrous cycle effects on
hippocampal spine density (mouse in vivo, [14]); human MTL volume
changes across menstrual cycle (7T MRI, [13]); TPH2-E2 relationship in
raphe (non-human primate, [48]); ZI TRα1 modulation of glucocorticoid
output (mouse, [23]); alpha-to-beta islet paracrine loop (mouse and
human islets, [30]); brain insulin resistance in T2D and Alzheimer's
disease ([33]); CSF melatonin reduction in preclinical AD ([38,
39]).</p></td>
</tr>
<tr class="even">
<td><p><strong>Tier C — Emerging findings or integrative hypotheses
(preprint, single study, or extrapolated from animal
models):</strong></p>
<p>Pineal volume heritability and melatonin output (2025 preprint GWAS,
[35]); MT1-Slo1 BK channel mechanism for SCN hyperpolarization (2025
preprint, [36]); melatonin metabolite AMK facilitating memory
consolidation (mouse only, [40]); ZI TRα1 cross-axis link awaits human
validation [23]; the cross-axis failure cascade framework (§4) is an
integrative synthesis — each component is supported, but the cascades as
unified clinical patterns are proposed rather than directly
measured.</p></td>
</tr>
</tbody>
</table>

## §2 — Detection Architecture of Each Axis

Each axis is organized below using five operations: Propagation (what
transmits the signal), Gating (what controls passage or threshold),
Detection (what measures deviation or error), Accumulation (what
integrates over time or chronic state), and Refinement (what updates the
structure itself). This decomposition is used as an analytical scaffold
for locating control logic and identifying coupling points; it does not
represent a theoretical claim beyond the established biology described.
Tier A claims are established consensus; Tier B claims have direct
experimental support as noted; Tier C findings are flagged at point of
use.

## §2.1 — The HPA Axis

The HPA axis is a central stress-response detection system. Its sensor
is the paraventricular nucleus (PVN), which integrates threat signals
from the brainstem, amygdala, and sensory cortex. Its error signal is
CRH, which drives ACTH, which drives cortisol. Its feedback is
glucocorticoid receptor (GR) signaling at the hippocampus, PVN, and
pituitary, suppressing CRH and ACTH secretion when cortisol rises \[5\].

Propagation: CRH is released from PVN into the portal blood in pulses
synchronized to the circadian rhythm. ACTH is released from
corticotrophs in approximately 15-20 pulses per day, superimposed on a
diurnal peak at waking \[5, 6\].

Gating: The hippocampus provides a major inhibitory gate on HPA axis
activity via GR-mediated negative feedback. Hippocampal GR activation
suppresses PVN CRH expression. Hippocampal GR sensitivity is regulated
by estradiol (via ER-alpha) \[7\] and testosterone \[8\], making HPA
feedback gain dependent on HPG axis status. A cross-axis link from the
HPT axis to glucocorticoid output is described in §2.3 \[23\].

Detection: The HPA axis detects psychological threat (amygdala → PVN),
immune signals (IL-6, TNF-alpha → PVN), hypoglycemia (arcuate nucleus
glucose sensors → PVN), and circadian phase (SCN → PVN) \[9\] — a point
of convergence for multiple deviation signals.

Accumulation: Chronic stress produces lasting changes in GR density, CRH
mRNA expression, and hippocampal volume. A major accumulation state is
GR desensitization: chronic cortisol → GR downregulation → reduced
hippocampal feedback → HPA hyperactivation — a positive feedback loop
that sustains the chronic stress phenotype. Prolonged ACTH also drives
adrenal hypertrophy, increasing cortisol response capacity \[10\].

Refinement: The diurnal cortisol rhythm is calibrated nightly during
slow-wave sleep, when the circadian cortisol nadir coincides with the
melatonin window, allowing GR-mediated feedback sensitivity to recover
\[11, 34\]. Chronic sleep disruption prevents this recalibration and
progressively degrades HPA setpoint accuracy \[11\].

## §2.2 — The HPG Axis

The HPG axis regulates reproductive function and sex steroid production.
HPG-derived steroids also function as modulators of central nervous
system parameters: estradiol modulates hippocampal dendritic spine
density (20-30% variation across the estrous cycle in mice \[14\];
structural correlates across the menstrual cycle documented in humans
\[13\]) and glucocorticoid receptor sensitivity \[7\]; progesterone's
metabolite allopregnanolone (ALLO) modulates GABA-A tonic inhibition and
NREM sleep depth \[43\].

Propagation: GnRH is secreted from the arcuate nucleus (ARC) in pulses,
with pulse frequency encoding the LH/FSH ratio. High frequency
(approximately one pulse per hour) drives LH dominance; low frequency
drives FSH dominance. The KNDy neuron circuit in the ARC generates these
pulses: NKB initiates each pulse, dynorphin terminates it \[15\]. The
ovulatory LH surge is driven by positive feedback from AVPV kisspeptin
following sustained preovulatory estradiol elevation \[16\].

Gating: The primary gate is kisspeptin sensitivity to estradiol: at the
ARC, estradiol provides negative feedback to suppress GnRH pulse
frequency; at the AVPV, estradiol provides positive feedback to drive
the LH surge — opposite effects from the same hormone acting on
anatomically distinct kisspeptin populations \[16\]. In mouse models,
glucocorticoids suppress kisspeptin expression in hypothalamic KNDy
neurons \[47\], providing one mechanism through which chronic stress may
reduce GnRH pulsatility in humans \[3\].

Detection: The HPG axis detects body energy state (leptin acts via
upstream hypothalamic neurons, including kisspeptin populations, to
regulate GnRH pulsatility: leptin deficiency → suppressed GnRH
pulsatility and anovulation \[17\]), immune signals (cytokines suppress
GnRH pulsatility during illness \[18\]), and circadian phase (melatonin
duration encodes season in photoperiodic species; attenuated but present
in humans \[19\]).

Accumulation: The most clinically prominent accumulation event is
menopause: progressive follicle depletion reduces estradiol output,
initially with volatility (perimenopause) before collapse. Estradiol
variability during perimenopause is proposed as a contributor to the
depression risk window during this transition, with hormone volatility
rather than deficiency alone as a driver \[12, 50\]. In males, Leydig
cell decline produces andropause: a progressive reduction in
testosterone output beginning in the third decade and continuing at an
approximately age-invariant rate, with total testosterone declining
approximately 1% per year and free testosterone falling faster due to
rising SHBG \[20\].

Refinement: In females, the brain synthesizes estradiol via aromatase
expressed in hippocampus, hypothalamus, and limbic cortex. Brain-local
estradiol is not eliminated by gonadectomy, providing cycle-independent
hormonal tone that partially buffers the synaptic effects of peripheral
estradiol fluctuations \[45\].

## §2.3 — The HPT Axis

The HPT axis regulates metabolic rate and thermogenesis. Its brain
effects are mediated not by plasma T4 or T3 but by local T3 availability
set by cell-type-specific deiodinase expression — making thyroid
function a regionally heterogeneous property of the brain rather than a
single systemic parameter \[21, 22\].

Propagation: TRH drives TSH from thyrotrophs. TSH drives T4 synthesis
and release. T4 is the predominant circulating form (~90%); T3 is the
biologically active form. Conversion of T4 to T3 by D1 deiodinase occurs
peripherally (liver, kidney). In the brain, D2 (tanycytes, astrocytes)
converts T4 to T3 locally; D3 inactivates T3 to rT3 \[22\]. Each brain
region's T3 availability is therefore set by its local D2 activity, not
by plasma levels.

Gating: D2 heterogeneity means different brain regions operate under
different thyroid hormone states. Tanycytes in the hypothalamus have
high D2 activity; cortical astrocytes have lower. D3 in raphe nuclei and
immature amygdala provides local T3 inactivation. In rodent models,
TRalpha1 signaling in the zona incerta modulates glucocorticoid output:
inhibition of ZI TRalpha1 produces approximately 3-fold elevation of
serum corticosterone, indicating an HPT-to-HPA cross-axis link that
awaits human validation \[23\].

Detection: TSH responds to both free T4 and T3 with high sensitivity to
small changes near setpoint. The population TSH reference range spans
approximately one order of magnitude (0.4-4.0 mIU/L), while individual
setpoints cluster considerably more tightly within that range.
Population-level reference ranges may therefore not identify suboptimal
T3 delivery in individuals with low-normal setpoints \[24\].

Accumulation: Chronic cortisol inhibits D1 deiodinase activity,
redirecting T4 conversion toward rT3 (inactive) rather than T3 (active)
\[25, 26\]. This produces a functional hypothyroid state without TSH
changes — the euthyroid sick syndrome pattern — and represents a
cross-axis mechanism by which sustained HPA activation depletes brain T3
availability.

Refinement: The DIO2 Thr92Ala polymorphism was first characterized in
the context of insulin resistance \[27\] and is carried by approximately
12-15% of the population (at least one copy) \[28\]. Some studies show
impaired brain T3 restoration on levothyroxine monotherapy in carriers,
though evidence for clinical impact is mixed \[28\].

## §2.4 — The Metabolic Axis (Pancreatic Islets)

The pancreatic islets implement a glucose-to-hormone transduction system
with three cell types in a coordinated paracrine circuit. The standard
description — beta cells produce insulin, alpha cells produce glucagon,
the two oppose each other — does not fully capture the paracrine circuit
architecture. Evidence from mouse and human islet studies indicates that
alpha cell glucagon appears necessary for normal insulin secretion,
acting as a paracrine primer rather than solely an opposing hormone
\[29, 30\].

Propagation: Beta cell insulin secretion operates in two phases. Phase 1
(triggering) is driven by glucose-induced KATP closure, membrane
depolarization, and Ca2+ spike — a rapid burst within the first few
minutes of glucose stimulation. Phase 2 (amplifying) is driven by
metabolic amplification (pyruvate anaplerosis) and incretin
amplification: GLP-1 and GIP secreted by gut L-cells and K-cells account
for 50-70% of the total insulin response to oral glucose \[29\]. The gut
therefore forms an important component of the glucose detection circuit.

Gating: Alpha cell glucagon acts via GCG-R on beta cells to prime
insulin secretion via an intra-islet paracrine loop: alpha-to-beta cell
structural contacts increase under metabolic stress and their disruption
reduces beta cell Ca2+ coordination and insulin output \[30\].
Somatostatin from delta cells gates both alpha and beta cells via
SSTR2/5. The islet functions as a three-node paracrine circuit.

Detection: Beta cells detect glucose via KATP conductance (half-maximal
at approximately 3.5 mmol/L); GLP-1 shifts this detection threshold
leftward. Hub cells — a subpopulation of beta cells with high metabolic
activity and strong gap-junction coupling — coordinate Ca2+ oscillation
timing across the islet. Hub cell dysfunction in early T2D produces
desynchronized insulin pulses before beta cell mass is significantly
reduced \[31\].

Accumulation: Chronic hyperglycemia (glucotoxicity) combined with
lipotoxicity produces ER stress → UPR → CHOP-mediated beta cell
apoptosis. Beta cell mass can expand substantially in early compensatory
response before progressive decompensation — a characteristic dynamic of
T2D pathophysiology.

Refinement: Brain insulin resistance — failure of brain insulin
signaling despite peripheral hyperinsulinemia — develops from chronic
insulin receptor desensitization at the blood-brain barrier and in
hippocampal neurons. Brain insulin supports active synapse energy via
GLUT4 mobilization \[32\]; brain insulin resistance degrades AMPA
receptor trafficking, hippocampal LTP, and neurogenesis, linking
metabolic disease to cognitive aging and Alzheimer's disease risk
\[33\].

## §2.5 — The Circadian Axis (SCN-Pineal)

The SCN-pineal axis does not follow the hypothalamic-pituitary-gland
topology — it has no hypothalamic releasing hormone and no pituitary
relay. It is a photoperiod-to-melatonin transducer: environmental
light-dark signal → retinal ipRGCs (melanopsin) → retinohypothalamic
tract → SCN → sympathetic pathway → superior cervical ganglion →
norepinephrine → pineal AANAT activation → melatonin synthesis.
Melatonin is secreted into both blood and CSF (the pineal is adjacent to
the third ventricle and lacks a blood-brain barrier), distributing the
time signal to all cells simultaneously \[34\].

Propagation: Melatonin is secreted only during the dark phase, with
onset approximately 2 hours before habitual sleep time (DLMO — dim-light
melatonin onset). Duration is season-dependent: approximately 8-10 hours
in summer and 10-12 hours in winter at mid-latitudes. Pineal volume
varies substantially between individuals and is estimated to be
approximately 19% heritable — individuals with smaller pineals tend to
have lower melatonin output and more daytime napping (Tier C: emerging
evidence from a 2025 preprint GWAS requiring replication \[35\]).

Gating: Melatonin acts on MT1 receptors on SCN neurons to hyperpolarize
them, reducing SCN firing and enabling the circadian transition to
sleep-phase physiology. Tier C: emerging evidence from a 2025 preprint
indicates this hyperpolarization is mediated via Slo1 BK channel
activation downstream of MT1 \[36\]. MT1 and MT2 receptors are expressed
on non-overlapping neuronal populations \[37\]. Melatonin contributes to
a multi-component sleep gate alongside orexin withdrawal and adenosine
accumulation \[49\]; the full consolidation gate architecture is
described in a companion reference.

Detection: The SCN clock is self-sustaining (CLOCK/BMAL1
transcriptional-translational feedback loop with ~24h period) but
requires daily light entrainment. Blue-spectrum light (460-480nm) via
melanopsin is the primary zeitgeber. Melatonin phase-shifts the SCN via
MT1, forming the mechanistic basis of chronotherapy for jet lag and
circadian sleep-wake disorders \[34\].

Accumulation: Pineal calcification increases with age, progressively
reducing pinealocyte mass and melatonin output amplitude. CSF melatonin
levels are substantially reduced in Alzheimer's disease compared to
age-matched controls \[38\], and this reduction is detectable at
preclinical Braak stages I-II, before cognitive symptoms appear —
suggesting melatonin may be an early biomarker of pathology \[39\].

Refinement: Tier C: Melatonin's metabolite AMK
(N1-acetyl-5-methoxykynuramine) has been shown to facilitate long-term
object memory consolidation in mice via nNOS inhibition, independent of
MT1/MT2 receptors \[40\]. Human replication is pending.

## §3 — The Cross-Axis Interaction Network

The endocrine axes share relay structures (hypothalamus, pituitary,
hippocampus), compete for receptor populations, and regulate each
other's sensitivity via direct molecular mechanisms. The cross-axis
interaction network helps determine the hormonal operating state — which
is often not well predicted by any single axis in isolation.

Table 1 maps the primary cross-axis interactions, showing each axis as
both a driver and a target. Rodent-derived mechanisms are noted where
human evidence is lacking.

| **Axis Driver**     | **→ HPA**                               | **→ HPG**                                        | **→ HPT**                    | **→ Metabolic**                                          | **Mechanism**                                    |
|---------------------|-----------------------------------------|--------------------------------------------------|------------------------------|----------------------------------------------------------|--------------------------------------------------|
| HPA (cortisol)      | —                                       | Kisspeptin ↓ → GnRH ↓ (B-rodent)                 | D1 inhibit → rT3 ↑, T3↓ (A)  | Hepatic glucose ↑, insulin demand ↑ (A)                  | GR → ARC KNDy; deiodinase block                  |
| HPG (E2/T)          | GR sensitivity ↑ E2 → HPA blunting (B)  | —                                                | SHBG change → free T3/T4 (B) | E2 → insulin sensitivity ↑ (B); T excess (PCOS) → IR (A) | ER-alpha hippocampus; SHBG liver                 |
| HPT (T3)            | ZI TRα1 → corticosterone ↑ (B-rodent)   | SHBG change → free E2/T (B)                      | —                            | Beta-cell sensitization; GLUT4 expression (B)            | ZI TRα1 pathway; Nuclear TR → GLUT4 gene         |
| Metabolic (insulin) | HPA axis compensatory demand ↑ (B)      | Beta-cell protection, E2 (B); PCOS, T excess (A) | Thyroid demand adapts (B)    | —                                                        | Cortisol → gluconeogenesis; insulin demand ↑ (A) |
| Melatonin (pineal)  | Nocturnal HPA nadir → recalibration (B) | Seasonal HPG modulation, minor in humans (B)     | Minor in humans (B)          | Indirect insulin sensitivity improvement (C)             | GR on pinealocytes; circadian gating             |

*Table 1. Cross-axis interaction network. Cells show downstream
consequence and primary molecular mechanism. Confidence markers: (A)
established consensus; (B) directly supported, may include rodent
evidence; (B-rodent) rodent-only, human translation pending; (C)
emerging/preprint/synthetic.*

## §3.1 — Cortisol as a Broad Cross-Axis Suppressor

Of the five axes, cortisol has broad cross-axis suppressive effects. Via
glucocorticoid-mediated suppression of kisspeptin expression in ARC KNDy
neurons (demonstrated in mouse models \[47\]), elevated cortisol reduces
GnRH pulse frequency and amplitude, producing functional hypogonadism in
chronic stress \[3\]. Via inhibition of D1 deiodinase activity, cortisol
redirects T4 conversion toward rT3, producing functional hypothyroidism
without TSH changes \[25, 26\]. Via glucocorticoid receptor activation
in liver and adipose tissue, cortisol increases hepatic glucose output
and peripheral insulin resistance, increasing metabolic demand on the
pancreatic islets \[41\].

The combined result is that sustained HPA activation produces a proposed
multi-axis pattern: blunted reproductive function, reduced T3
availability, elevated insulin demand, and disrupted melatonin onset
(inferred via sympathetic arousal pathway — see §3.4). This
constellation may contribute to recognizable patterns in burnout, PTSD,
and chronic illness, though it spans specialties that do not typically
communicate with each other — and the combined multi-axis framing is a
synthesis rather than an independently validated syndrome.

## §3.2 — Estradiol as HPA Feedback Gain Modulator

Estradiol modulates HPA axis sensitivity via ER-alpha on hippocampal
neurons that express glucocorticoid receptors. Estradiol increases GR
sensitivity in the hippocampus, strengthening the negative feedback
brake on the HPA axis \[7\]. The high-estradiol preovulatory phase is
associated with better HPA regulation; low-estradiol phases (menses,
perimenopause) are associated with more variable cortisol responses to
the same stressor.

This E2-GR relationship provides one pathway through which estradiol
loss or volatility may contribute to elevated rates of depression and
anxiety during menstrual transitions, perimenopause, and postpartum
\[12, 50\]. Serotonin changes (via E2 effects on TPH2 expression in
raphe neurons, demonstrated in non-human primate models \[48\]) and ALLO
withdrawal are likely parallel contributors, and the relative weights of
these mechanisms in humans are not established.

## §3.3 — SHBG as the HPG-HPT Bridge

Sex hormone-binding globulin (SHBG) is produced by the liver under
regulation from thyroid hormone. T3 increases SHBG production;
hypothyroidism reduces SHBG. Because only free (unbound) sex steroids
are biologically active, SHBG levels determine effective sex steroid
delivery to tissue receptors regardless of total circulating levels.
Hypothyroidism therefore produces elevated free sex steroids via SHBG
reduction, even when total levels appear normal — a mechanism that
contributes to the menstrual irregularity and altered androgen
sensitivity commonly observed in thyroid dysfunction \[42\].

## §3.4 — Melatonin as the Nocturnal Gating Signal

Melatonin onset gates the nocturnal recalibration of the HPA axis:
during the melatonin window, cortisol is at nadir and GR-mediated
feedback sensitivity recovers, re-establishing the HPA setpoint for the
following day during slow-wave sleep \[11\]. Disruption of melatonin
onset (chronic light exposure, shift work) prevents this recalibration.

Similarly, melatonin onset, by enabling the sleep window within which
NREM-dependent GnRH pulsatility occurs, supports morning testosterone
production in males. Sleep disruption reduces morning testosterone not
by directly affecting Leydig cells but by disrupting the nocturnal LH
pulse cascade that requires this NREM sleep window \[44\]. Melatonin's
partial suppression of HPA activity during the melatonin window also
reduces glucocorticoid-mediated kisspeptin suppression, allowing HPG
overnight recovery — a mechanistic inference chain (Tier C) based on the
individual links rather than a directly measured effect.

## §4 — Multi-Axis Failure Cascades

Each axis has characteristic failure modes that emerge from the
accumulation states described in §2. The following patterns are
integrative syntheses (Tier C): each component mechanism is supported at
the level indicated in the evidence tiers box, but the cascades as
unified clinical patterns are proposed based on the mechanistic
connections, not directly measured as unified syndromes.

## §4.1 — Chronic Stress Cascade

Chronic psychological or physiological stress initiates an HPA
activation state that, over months to years, can propagate to other axes
through the cross-axis links described in §3. Sustained cortisol: (1)
desensitizes hippocampal GR, reducing HPA feedback; (2) suppresses
kisspeptin (mouse evidence \[47\]), potentially reducing sex steroid
output; (3) suppresses D1 deiodinase, reducing T3 \[25, 26\]; (4)
increases hepatic glucose and insulin demand \[41\]; (5) may delay
melatonin onset via sympathetic arousal-driven NE elevation at the
pineal \[34\]. Each of these effects is individually supported; their
combined propagation as a unified cascade is an integrative hypothesis
\[3, 9\].

## §4.2 — The Perimenopause Multi-Axis Disruption

The perimenopause transition involves E2 volatility preceding E2 loss.
Fluctuating E2 is associated with: intermittent disruption of
hippocampal GR sensitivity (variable HPA regulation) \[7\]; intermittent
destabilization of serotonin synthesis via TPH2 expression changes in
raphe neurons (demonstrated in non-human primate models \[48\]);
intermittent changes in SHBG (altering free T3 and testosterone
delivery) \[42\]; and increasingly irregular allopregnanolone (ALLO)
fluctuations due to anovulatory cycles and variable progesterone output,
which may destabilize GABA-A tonic inhibition \[43\]. Each mechanism is
individually supported; their combination as a unified perimenopause
syndrome is a proposed synthesis \[12, 50\].

## §4.3 — Metabolic-Cognitive Cascade

Peripheral insulin resistance, if chronic, can produce brain insulin
resistance through BBB insulin transport saturation and receptor
desensitization. Brain insulin resistance is associated with reduced
AMPA receptor trafficking, reduced hippocampal neurogenesis, reduced PFC
glucose delivery via GLUT4 \[32\], and reduced suppression of excitatory
synaptic transmission onto VTA dopamine neurons — consistent with
elevated food reward salience reported under brain insulin resistance
\[46\]. These associations link T2D to accelerated hippocampal aging and
elevated Alzheimer's disease risk through identifiable molecular
pathways \[33\].

## §5 — The Integrated System

The five axes, their detection operations, and their cross-axis
couplings form a distributed endocrine operating system:

- HPA: a central threat and energy-state detector; outputs cortisol to
  mobilize resources; acutely suppresses HPG, HPT, and metabolic axis
  during threat response

- HPG: sex steroid and reproductive state manager; calibrates
  hippocampal plasticity, serotonin tone, and white matter
  microstructure \[51\] on 28-day and lifespan timescales

- HPT: metabolic rate setter; establishes brain T3 availability
  region-by-region via local deiodinase; cross-links to HPA via zona
  incerta TRα1 (rodent) and to HPG via SHBG

- Metabolic (islets): glucose state transducer; brain insulin signaling
  sets hippocampal encoding capacity and modulates dopaminergic food
  reward; incretin system links gut nutrient state to islet output

- Circadian (pineal): time-of-day and season encoder; gates the
  overnight recalibration window for other axes; contributes to
  consolidation gate control

Coordinated cycling of all five axes is one useful way to conceptualize
normal endocrine function. These axes operate at different timescales —
diurnal (HPA, melatonin), monthly (HPG), slowly across decades
(andropause, menopause), and continuously in response to metabolic load
(islets) — yet are coupled through shared relay infrastructure and are
usefully understood as a system rather than as independent processes.

## §6 — Scope, Limitations, and Companion References

This paper proposes a functional framework for the endocrine system
organized around five coupled feedback axes. The framework's
contribution is the cross-axis interaction map and the identification of
multi-axis failure cascades — not the individual mechanistic findings,
which are established in the cited literature. Three limitations apply.

First, evidence confidence varies. The evidence tiers box in §1
separates established consensus from directly supported cross-axis
mechanisms from emerging or rodent-only findings. Readers should apply
those tiers when evaluating clinical implications.

Second, brain-interface effects are not covered here. Receptor
distributions, circuit-level hormone effects, and disease-specific brain
mechanisms are covered in the companion Brain-Body reference (BrainBody
v1.3) and in the Peripheral Organ Maps (Pituitary, Adrenal, Thyroid,
Pancreatic Islets, Gonads, Pineal — v1.0 series). Those documents
provide the parameter-level detail that complements the architectural
overview presented here.

Third, the failure cascades in §4 are integrative syntheses. Each
component mechanism is supported at the tier indicated; the cascades as
unified clinical patterns are proposed rather than directly measured.
They are intended to generate testable predictions about cross-axis
dysregulation patterns in burnout, perimenopause, and
metabolic-cognitive decline, not to substitute for direct clinical
evidence of those patterns.

### Integration target

This paper is designed to merge into the Brain-Body Unified Reference
(BrainBody) as its endocrine architecture component once the full
peripheral system map series is complete (Tier 5: Pituitary, Adrenal,
Thyroid, Pancreatic Islets, Gonads, Pineal — all at v1.0; Tier 6: limbic
re-pass pending). At that point, §2 (axis detection architectures)
merges with the Peripheral Maps into BrainBody §2; §3 (cross-axis
interactions) merges into BrainBody §3 (hormone-brain interface); §4
(failure cascades) feeds into the disease papers. The Appendix
simulation role table migrates with the merge and supersedes any
axis-level encoding guidance in earlier BrainBody drafts. Until the
merge, this document stands as the canonical endocrine architecture
reference.

## Appendix — Simulation Role Classification of Cross-Axis Links

Each cross-axis mechanism described in this paper is classified below
according to its recommended role in a computational brain-body
simulation. Classifications are based on the evidence tier assignments
in §1 and the species/preprint flags throughout the text.

Core Rule: Tier A consensus; safe to encode as baseline system behavior.
Supported Modifier: Tier B; directly supported but may rest on rodent
evidence or single-modality data — encode as a conditional modifier that
can be toggled. Hypothesis Layer: Tier C or inference chain; emerging,
preprint, or multi-step inference — treat as optional provisional
module, not baseline.

| **Cross-Axis Link**                                                 | **Tier**   | **Simulation Role** | **Notes**                                                                                                                                             |
|---------------------------------------------------------------------|------------|---------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
| Cortisol → D1 deiodinase inhibition → rT3 (HPA→HPT)                 | A          | Core Rule           | Well-replicated in humans; euthyroid sick syndrome is a validated clinical phenomenon \[25,26\]                                                       |
| Cortisol → hepatic gluconeogenesis → insulin demand (HPA→Metabolic) | A          | Core Rule           | Direct glucocorticoid receptor mechanism in liver; human validated \[41\]                                                                             |
| SHBG bridges HPT and HPG (T3 regulates free sex steroids)           | A/B        | Core Rule           | SHBG regulation by T3 is established; clinical consequences confirmed in thyroid dysfunction \[42\]                                                   |
| Beta cell two-phase insulin secretion with incretin amplification   | A          | Core Rule           | 50-70% of oral glucose response is incretin-driven; textbook-level \[29\]                                                                             |
| Melatonin as photoperiod signal via SCN-MT1 pathway                 | A          | Core Rule           | Mechanism well-established; DLMO as zeitgeber is clinical standard \[34\]                                                                             |
| HPA negative feedback via hippocampal GR                            | A          | Core Rule           | Foundational neuroendocrinology; GR-mediated suppression of CRH/ACTH is textbook \[5\]                                                                |
| E2 modulates hippocampal GR sensitivity (HPG→HPA feedback gain)     | B          | Supported Modifier  | Rodent and human evidence; ER-alpha mechanism confirmed \[7\]. Encode as E2-dependent scaling of HPA feedback gain.                                   |
| Cortisol → kisspeptin suppression → GnRH reduction (HPA→HPG)        | B (rodent) | Supported Modifier  | Kiss1 suppression confirmed in mouse ARC \[47\]; human translation inferred. Encode as conditional — activate under chronic stress state.             |
| Alpha-to-beta islet paracrine loop (glucagon primes insulin)        | B          | Supported Modifier  | Mouse and human islet evidence \[29,30\]. Encode as paracrine amplification factor on phase 1 insulin.                                                |
| Brain insulin resistance degrades hippocampal LTP and neurogenesis  | B          | Supported Modifier  | Well-supported mechanistic links \[33\]; encode as chronic metabolic state modifier on memory encoding parameters.                                    |
| E2/P4 variation → MTL volume changes across menstrual cycle         | B          | Supported Modifier  | Human 7T MRI \[13\]; Wolcott mouse in vivo \[14\]. Encode as 28-day cycling modifier on hippocampal parameters.                                       |
| CSF melatonin reduction in preclinical Alzheimer's disease          | B          | Supported Modifier  | Two post-mortem studies \[38,39\]; consistent with circadian disruption in AD. Encode as age-dependent melatonin output decay.                        |
| ZI TRα1 signaling → glucocorticoid output (HPT→HPA)                 | B (rodent) | Supported Modifier  | Mouse only \[23\]; human validation pending. Encode as optional HPT→HPA modifier, off by default.                                                     |
| E2 → WM diffusion anisotropy (HPG→white matter)                     | B          | Supported Modifier  | Single longitudinal study \[51\]; encode as a provisional HPG→WM structural modifier.                                                                 |
| Melatonin → nocturnal HPA recalibration window                      | B          | Supported Modifier  | Circadian cortisol nadir + GR recovery supported \[11,34\]; melatonin-specific contribution is partially inferred.                                    |
| Melatonin onset → NREM-dependent GnRH pulsatility → testosterone    | B          | Supported Modifier  | Sleep fragmentation → testosterone reduction confirmed \[44\]; melatonin as enabling gate is inferred.                                                |
| Pineal volume heritability → melatonin output variation             | C          | Hypothesis Layer    | 2025 preprint GWAS \[35\]; requires replication before encoding.                                                                                      |
| MT1-Slo1 BK channel mechanism for SCN hyperpolarization             | C          | Hypothesis Layer    | 2025 preprint \[36\]; mechanistic detail not yet peer-reviewed.                                                                                       |
| AMK metabolite → LTM consolidation via nNOS inhibition              | C          | Hypothesis Layer    | Mouse only \[40\]; no human data. Treat as optional module.                                                                                           |
| Melatonin suppression → less kisspeptin suppression → HPG recovery  | C          | Hypothesis Layer    | Three-step inference chain; no direct measurement. Flag as hypothesis layer in simulation \[§3.4\].                                                   |
| Chronic stress cascade as unified multi-axis syndrome               | C          | Hypothesis Layer    | Each component supported individually; cascade as unified pattern is proposed synthesis \[§4.1\]. Encode components separately, not as a single rule. |
| Perimenopause multi-axis disruption as unified syndrome             | C          | Hypothesis Layer    | Each mechanism supported; co-occurrence as unified syndrome is proposed synthesis \[§4.2\].                                                           |
| Metabolic-cognitive cascade (peripheral IR → brain IR → AD risk)    | C          | Hypothesis Layer    | Mechanistic links supported \[33\]; cascade sequence in humans is inferred. Encode as probabilistic risk modifier, not deterministic chain.           |

*Appendix Table. Simulation role classification of cross-axis links.
Core Rule = encode as baseline system behavior. Supported Modifier =
encode as conditional, can be toggled. Hypothesis Layer = optional
provisional module, not baseline.*

## References

\[1\] Chrousos, G.P. Stress and disorders of the stress system. Nat Rev
Endocrinol 5 (2009) 374-381.

\[2\] Boron, W.F. & Boulpaep, E.L. Medical Physiology, 3rd ed. Elsevier
(2017).

\[3\] Kalantaridou, S.N. et al. Stress and the female reproductive
system. J Reprod Immunol 62 (2004) 61-68.

\[4\] Kyrou, I. & Tsigos, C. Stress hormones: physiological stress and
regulation of metabolism. Curr Opin Pharmacol 9 (2009) 787-793.

\[5\] Herman, J.P. et al. Regulation of the HPA stress response. Compr
Physiol 6 (2016) 603-621.

\[6\] Weitzman, E.D. et al. Twenty-four hour pattern of the episodic
secretion of cortisol in normal subjects. J Clin Endocrinol Metab 33
(1971) 14-22.

\[7\] McEwen, B.S. & Alves, S.E. Estrogen actions in the central nervous
system. Endocr Rev 20 (1999) 279-307.

\[8\] Kerr, J.E. et al. Androgens modulate glucocorticoid receptor
binding in hippocampus. Neuroendocrinology 62 (1995) 227.

\[9\] Tsigos, C. & Chrousos, G.P. HPA axis, neuroendocrine factors and
stress. J Psychosom Res 53 (2002) 865-871.

\[10\] McEwen, B.S. Allostasis and allostatic load. Neuropsychopharmacol
22 (2000) 108-124.

\[11\] Vgontzas, A.N. et al. Sleep, the HPA axis, and cytokines. Sleep
Med Rev 5 (2001) 365-376.

\[12\] Freeman, E.W. et al. Associations of hormones and menopausal
status with depressed mood. Arch Gen Psychiatry 63 (2006) 375-382.

\[13\] Zsido, R.G. et al. Ultra-high-field 7T MRI reveals changes in
human medial temporal lobe volume during menstrual cycle. Nat Ment
Health 1 (2023) 761-771.

\[14\] Wolcott, N.S. et al. The estrous cycle modulates hippocampal
spine dynamics, dendritic processing, and spatial coding. Neuron 113(14)
(2025) 2297-2309.e7.

\[15\] Navarro, V.M. et al. Interactions between kisspeptin and
neurokinin B in the control of GnRH secretion. Am J Physiol Endocrinol
Metab 300 (2011) E202-E210.

\[16\] Herbison, A.E. Control of puberty onset and fertility by GnRH
neurons. Nat Rev Endocrinol 12 (2016) 452-466.

\[17\] Quennell, J.H. et al. Leptin indirectly regulates GnRH neuronal
function. Endocrinology 150 (2009) 2805-2812.

\[18\] Karsch, F.J. et al. Inflammatory cytokines suppress GnRH
pulsatility. Biol Reprod 52 (1995) 190-197.

\[19\] Pandi-Perumal, S.R. et al. Physiological effects of melatonin:
melatonin receptors and signal transduction. Prog Neurobiol 85 (2008)
335-353.

\[20\] Harman, S.M. et al. Longitudinal effects of aging on serum total
and free testosterone levels in healthy men. Baltimore Longitudinal
Study of Aging. J Clin Endocrinol Metab 86 (2001) 724-731.

\[21\] Gereben, B. et al. Cellular and molecular basis of
deiodinase-regulated thyroid hormone signaling. Endocr Rev 29 (2008)
898-938.

\[22\] Bianco, A.C. et al. Biochemistry and physiological roles of the
iodothyronine selenodeiodinases. Endocr Rev 23 (2002) 38-89.

\[23\] Maier, J. et al. Inhibition of thyroid hormone signaling in the
zona incerta alters basal metabolic rate, behavior, and serum
glucocorticoids in male mice. Thyroid 34 (2024) 1280-1291. \[Rodent;
human validation pending\]

\[24\] Gullo, D. et al. The same TSH threshold does not fit all
patients. J Clin Endocrinol Metab 96 (2011) e1727.

\[25\] Chopra, I.J. et al. Opposite effects of dexamethasone on serum
concentrations of reverse T3 and T3. J Clin Endocrinol Metab 41 (1975)
911-920.

\[26\] Fliers, E. et al. Thyroid function in critically ill patients.
Lancet Diabetes Endocrinol 3 (2015) 816-825.

\[27\] Mentuccia, D. et al. Association between a novel variant of the
human type 2 deiodinase gene Thr92Ala and insulin resistance. Diabetes
51 (2002) 880-883.

\[28\] Wouters, H.J.C.M. et al. No effect of the Thr92Ala polymorphism
of deiodinase-2 on thyroid hormone parameters or cognitive functioning
in a large population-based cohort. Thyroid 27 (2017) 147-155.

\[29\] Campbell, J.E. & Newgard, C.B. Mechanisms controlling pancreatic
islet cell function in insulin secretion. Nat Rev Mol Cell Biol 22
(2021) 142-158.

\[30\] Visa, M. & Berggren, P.O. Sex-dependent intra-islet structural
rearrangements affecting alpha-to-beta cell interactions. Diabetologia
67 (2024) 1663-1682.

\[31\] Rutter, G.A. & Benninger, R.K.P. Exploring pancreatic beta-cell
subgroups and their connectivity. Nat Metab 6 (2024) 2054-2073.

\[32\] Ashrafi, G. et al. GLUT4 mobilization supports energetic demands
of active synapses. Neuron 93 (2017) 606-615.

\[33\] Arnold, S.E. et al. Brain insulin resistance in type 2 diabetes
and Alzheimer disease. Nat Rev Neurosci 19 (2018) 63-76.

\[34\] Pandi-Perumal, S.R. et al. Physiological effects of melatonin.
FEBS J 273 (2006) 2813-2838.

\[35\] Xu, P. et al. GWAS of human pineal gland volume as proxy for
melatonin secretion. medRxiv (2025 Mar 11). Preprint — not yet peer
reviewed.

\[36\] Wang, Z.W. et al. Melatonin enhances sleep via MT1-driven
activation of Slo1 in SCN neurons. bioRxiv (2025). Preprint — not yet
peer reviewed.

\[37\] Klosen, P. Thirty-seven years of MT1 and MT2 melatonin receptor
localization in the brain. J Pineal Res 76 (2024) e12955.

\[38\] Liu, R.Y. et al. Decreased melatonin levels in postmortem CSF in
relation to aging, Alzheimer's disease, and apolipoprotein E-epsilon4/4
genotype. J Clin Endocrinol Metab 84 (1999) 323-327.

\[39\] Zhou, J.N. et al. Early neuropathological Alzheimer's changes are
accompanied by decreased CSF melatonin levels. J Pineal Res 35 (2003)
125-130.

\[40\] Iwashita, H. et al. Effects of endogenous and exogenous
N-acetyl-5-methoxykynuramine on object recognition memory in male C3H
mice. Horm Behav 150 (2023) 105329. \[Mouse only; human data pending\]

\[41\] Vegiopoulos, A. & Herzig, S. Glucocorticoids, metabolism and
metabolic diseases. Mol Cell Endocrinol 275 (2007) 43-61.

\[42\] Ott, J. et al. Thyroid function and risk of complications in
women undergoing IVF. Thyroid 21 (2011) 895-902.

\[43\] Bäckström, T. et al. Pathogenesis in menstrual cycle-linked CNS
disorders. Ann N Y Acad Sci 1317 (2014) 42-58.

\[44\] Luboshitzky, R. et al. Disruption of the nocturnal testosterone
rhythm by sleep fragmentation in normal men. J Clin Endocrinol Metab 86
(2001) 1134-1139.

\[45\] McCarthy, M.M. Estradiol and the developing brain. Physiol Rev 89
(2009) 909-959.

\[46\] Ferrario, C.R. & Reagan, L.P. Insulin-mediated synaptic
plasticity in the CNS: anatomical, functional and temporal contexts.
Neuropharmacology 136 (2018) 182-191.

\[47\] Kinsey-Jones, A.R. et al. Down-regulation of Kiss1 gene
expression in the mouse hypothalamus by central glucocorticoid receptor
signalling. J Neuroendocrinol 21 (2009) 1035-1040. \[Mouse\]

\[48\] Bethea, C.L. et al. Serotonin-related gene expression in female
monkeys with individual sensitivity to stress. Neuroscience 132 (2005)
151-166. \[Rhesus macaque\]

\[49\] Saper, C.B. et al. Sleep state switching. Neuron 68 (2010)
1023-1042.

\[50\] Kundakovic, M. & Rocks, D. Sex hormone fluctuation and increased
female risk for depression and anxiety disorders: from clinical evidence
to molecular mechanisms. Front Neuroendocrinol 66 (2022) 101010.

\[51\] Rizor, E.J. et al. Menstrual cycle-driven fluctuations in
oxytocin, estradiol, and luteinizing hormone co-vary with white matter
diffusion anisotropy: an exploratory 30-day longitudinal study. Hum
Brain Mapp 45 (2024) e26584.
