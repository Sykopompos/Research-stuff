# The Cardiovascular and Renal Systems as a Coupled Regulatory Architecture

*RAAS, Baroreflex, and Hemodynamic Linkage as Shared Interfaces · Endothelial and Contractile Reserve Thresholds · GFR Autoregulation and Tubuloglomerular Feedback · Cardiorenal Syndrome · SGLT2 Inhibition Mechanism · Hormonal Operating Parameters*

**M. Finnegan** · v1.3 — March 2026 · *Unpublished draft, not yet peer reviewed*

---

> **Article Scope and Companion References:** This paper is an integrative review of the cardiovascular and renal systems analyzed as a coupled regulatory architecture. The two systems are treated together because their principal control axis — the renin–angiotensin–aldosterone system (RAAS) — and their autonomic interface are shared, and their failure modes are bidirectional. The five-operation decomposition (Propagation, Gating, Detection, Accumulation, Refinement) is used as an analytical scaffold for locating control logic and identifying coupling points; it does not represent a theoretical claim beyond the established biology described. Brain-interface effects of cardiovascular and renal signals are covered in the companion Brain-Body Unified Reference (BrainBody v1.3) and in the relevant brain structure maps. Evidence confidence tiers are specified at the end of §1.

---

## Abstract

The cardiovascular and renal systems are mechanistically coupled through four interfaces: the renin–angiotensin–aldosterone system (RAAS), which uses renal perfusion pressure as its primary activation signal and the heart and vasculature as its principal remodeling targets; the baroreflex arc, which routes arterial pressure afferents through the brainstem to modulate both cardiac output and renal sympathetic tone simultaneously; direct hemodynamic coupling, in which cardiac output determines renal perfusion pressure and renal sodium handling determines cardiac preload; and the natriuretic peptide system (ANP, BNP), released by the heart in response to wall stretch and exerting counter-regulatory natriuresis and vasodilation that partially oppose RAAS. These couplings produce bidirectional failure modes — cardiorenal syndromes in which cardiac dysfunction drives renal injury and renal disease amplifies cardiac risk — that are not adequately modeled by treating either system in isolation.

This paper applies the five-operation decomposition to both systems and identifies the molecular and hemodynamic mechanisms at each operational stage. The cardiovascular system is characterized by two sequential threshold parameters: k_endo, the endothelial repair capacity that must remain above the level required to exclude LDL from the sub-intimal space, and k_cardiac, the contractile reserve that must remain above the level required for adequate cardiac output. These thresholds are mechanistically independent and degrade via distinct mechanisms on different timescales. The renal system is characterized by glomerular filtration rate (GFR) as the primary output variable and renin release rate as the primary alarm signal, gated by three independent inputs: renal perfusion pressure, macula densa NaCl concentration, and sympathetic β1-adrenergic tone.

Three failure cascades are analyzed in depth: type 2 cardiorenal syndrome (chronic heart failure → CKD), the atherosclerosis–infarction–heart failure sequence, and diabetic kidney disease; HFpEF mechanisms are addressed separately in §4.4. SGLT2 inhibition is shown to engage the tubuloglomerular feedback mechanism directly, providing hemodynamic renoprotection independent of its glycosuric effect, which accounts for its efficacy in non-diabetic CKD. Evidence tiers (A: replicated, mechanistically confirmed; B: mechanistically supported, not fully replicated; C: integrative synthesis) are assigned throughout.

---

## §1 — The Cardiovascular and Renal Systems as a Coupled Architecture

The cardiovascular and renal systems are conventionally treated as separate organ systems. This separation is appropriate for clinical specialization but poorly suited to mechanistic modeling. The two systems share a primary signaling axis whose initiating gate (renin secretion) resides in the kidney and whose principal chronic consequences (cardiac fibrosis, vascular remodeling, sodium and water retention) are distributed across the heart, vasculature, and renal collecting duct. They share a hemodynamic coupling in which mean arterial pressure (MAP) is both the primary output of the cardiovascular system and the primary input to the renal perfusion-sensing apparatus at the juxtaglomerular apparatus. The two systems share an autonomic interface in which the same brainstem circuits — the nucleus tractus solitarius (NTS) and the rostral ventrolateral medulla (RVLM) — that regulate cardiac output also set renal sympathetic tone [6].

This architecture has a predictable failure pattern. When cardiac output falls, renal perfusion pressure falls with it. The kidney interprets falling perfusion as volume depletion and activates the RAAS. Angiotensin II and aldosterone drive sodium and water retention, raising cardiac preload. In a functioning heart this closes the loop: output is restored and RAAS activation is suppressed. In a failing heart the additional preload worsens wall stress, accelerates neurohormonal remodeling, and further depresses output — while the kidney, still detecting inadequate perfusion, sustains RAAS activation. The compensatory response becomes the driver of progressive damage. This pattern is cardiorenal syndrome: a consequence of shared feedback architecture in which compensatory activation of one system amplifies failure of the other [18].

The five-operation decomposition used throughout this paper (Propagation, Gating, Detection, Accumulation, Refinement) is an analytical scaffold for locating control logic and identifying coupling points. It does not represent a theoretical claim beyond the established biology described in each section. The coupling analysis in §3 identifies the shared interfaces; the failure cascade analysis in §4 shows how those interfaces amplify rather than correct failure when one system is compromised.

---

### Evidence Tiers — Scope and Confidence of Claims

> **Note:** These tiers reflect the confidence with which claims are used within this review. They are not a formal evidence-grading system (e.g., GRADE) and should not be read as one. Reviewers may reasonably disagree on individual assignments.

**Tier A — Established consensus (well-replicated, textbook-level):** Sympathetic NE → β1-AR on SA node → chronotropy; parasympathetic ACh → M2 → bradycardia; baroreflex loop (baroreceptors → NTS → RVLM/nAmb); HRV-RMSSD as vagal tone proxy; eNOS/NO as master endothelial gatekeeper; RAAS cascade (renin → Ang I → ACE → Ang II → aldosterone); GFR Starling pressure equation; tubuloglomerular feedback (TGF); three independent renin gates (pressure, NaCl, SNS); aldosterone → ENaC → Na⁺ retention; SGLT2 glucose-Na⁺ cotransport in proximal tubule.

**Tier B — Mechanisms with direct experimental support:** eNOS uncoupling via BH4 depletion (human cell and animal models; clinical correlates established); SGLT2 inhibition → TGF restoration → intraglomerular pressure reduction (mechanism supported by physiological studies; confirmed in CREDENCE and EMPA-KIDNEY outcome trials [16,17]); ACE2/Ang1–7/MasR counter-regulatory axis (human and animal); E2 → eNOS upregulation and ACE2 expression (human endothelial cell studies; menopause clinical data consistent [22]); HRV as cardiorenal risk marker (HRV–CKD association established, renal SNS contribution inferred [7,8]).

**Tier C — Integrative syntheses or emerging findings:** HRV reduction → elevated renal sympathetic tone → CKD progression as unified cascade (each component B; combined direction is inferred); CKD metabolic acidosis → sarcopenia → cognitive decline cascade (each component individually supported; the cascade as a unified clinical pattern is proposed); cortisol–RAAS sensitization as driver of psychosocial cardiovascular risk (each molecular step supported; clinical translation partially established).

---

## §2 — Detection Architecture of Each System

### Five-Operation Decomposition — Definition of Terms

| Operation | Definition |
|---|---|
| **Propagation** | The mechanism by which a signal or state change is transmitted from one component to the next within or between systems. |
| **Gating** | The control mechanism that determines whether a signal passes, accumulates, or is blocked; the threshold or valve function that separates quiescent from active states. |
| **Detection** | The sensing mechanism that measures deviation from a setpoint and generates an error signal; the molecular sensor or organ that monitors system state. |
| **Accumulation** | The time-integrated process by which repeated or sustained activations produce structural or functional change; the state that builds incrementally toward irreversibility. |
| **Refinement** | The adaptive mechanism that updates setpoints, receptor densities, or circuit gain in response to chronic inputs; the system's capacity for recalibration. |

Each system is analyzed below using these five operations as an organizational scaffold. Tier A claims are established consensus; Tier B claims have direct experimental support as noted; Tier C findings are flagged at point of use.

---

### §2.1 — The Cardiovascular System

**Propagation.** The cardiovascular system propagates two signal types simultaneously. The electrical signal — originating at the sinoatrial (SA) node via HCN4 channel-mediated If current and conducted through the His–Purkinje system at approximately 4 m/s — coordinates myocardial contraction [1]. The mechanical signal — cardiac output (HR × SV), transmitted as a pressure wave through the arterial tree — delivers oxygen and substrate to all tissues and provides the hemodynamic input to the renal perfusion-sensing apparatus. Stroke volume is governed by three independent variables: preload (end-diastolic volume, Frank–Starling mechanism), afterload (systemic vascular resistance), and contractility (calcium handling efficiency, SERCA2a-dependent). Coronary autoregulation maintains perfusion across a coronary perfusion pressure range of approximately 50–130 mmHg via metabolic vasodilation (adenosine, CO₂, H⁺) and myogenic response; adenosine accumulates when ATP demand exceeds supply, making coronary flow a demand-matched autoregulation rather than a centrally commanded one [23].

**Gating.** Two sequential failure thresholds define cardiovascular disease progression. The first, k_endo, represents endothelial repair capacity: the net ability of the endothelium to maintain NO production, tight junction integrity, and anti-adhesion molecule suppression. Atherosclerosis initiates when endothelial repair capacity falls below the level required to exclude LDL from the sub-intimal space. The molecular gate is eNOS activity and its dependence on BH4 (tetrahydrobiopterin) availability. Under oxidative stress, BH4 is depleted, eNOS uncouples, and produces superoxide instead of NO — converting the primary endothelial protective enzyme into an oxidative stress amplifier [4]. This eNOS uncoupling is the self-reinforcing cycle that sustains endothelial dysfunction: oxidative stress depletes BH4 → uncoupled eNOS produces more superoxide → further BH4 depletion → less NO. The second threshold, k_cardiac, represents contractile reserve: functional cardiomyocyte mass, calcium handling efficiency, and mitochondrial ATP production capacity. The two thresholds are sequential — endothelial failure enables the cascade that eventually exhausts contractile reserve — but mechanistically independent and requiring distinct interventions [2, 3]. Both thresholds map to measurable clinical correlates: k_endo corresponds operationally to endothelial function assessed by flow-mediated dilation (FMD) or circulating endothelial progenitor cell counts; k_cardiac corresponds operationally to left ventricular ejection fraction, longitudinal strain, and exercise capacity. Neither is directly measured in routine practice as a unified parameter, but their component determinants are individually assessable. Both are best understood as heuristic composite constructs that summarize mechanistically related determinants, rather than as validated single clinical metrics.

**Detection.** The baroreflex arc provides continuous MAP detection. Carotid sinus and aortic arch baroreceptors detect arterial wall stretch, transmitting via CN IX/X to NTS, routing through CVLM to RVLM and nucleus ambiguus, and modifying both sympathetic cardiac tone and parasympathetic vagal tone; the full loop operates on a timescale of 0.5–2 seconds [6]. Baroreflex gain — the change in RR interval per unit change in MAP, expressed in ms/mmHg — is the quantitative measure of this sensitivity; healthy adults maintain gains of approximately 15–25 ms/mmHg [8], and gain below 3 ms/mmHg is associated with markedly elevated cardiovascular mortality (Tier A) [7]. A second detection layer operates at the vascular wall: laminar shear stress activates PIEZO1 and transcription factors KLF2/KLF4, upregulating eNOS and suppressing pro-inflammatory gene programs; oscillatory or low shear (at bifurcations and branch points) activates NF-κB instead. The geometric predilection of atherosclerosis for bifurcations and curvatures follows from this sensor architecture (Tier A) [9].

**Accumulation.** Atherosclerosis is a slowly accumulating state. Sub-intimal LDL oxidation, foam cell formation, fibrous cap development, and cap thinning via MMP upregulation (NLRP3 → IL-1β → MMP expression) accumulate over years to decades. The NLRP3 inflammasome, activated by cholesterol crystals and oxidized LDL, amplifies stable plaque to vulnerable plaque. The CANTOS trial — demonstrating a 15% relative reduction in cardiovascular events with an IL-1β antibody independent of LDL lowering — confirmed the inflammatory accumulation mechanism as an independent, actionable target (Tier A) [10]. Post-infarction cardiac remodeling is a second accumulation process operating via distinct mediators. The acute molecular gate for ischemic cardiomyocyte death is the mitochondrial permeability transition pore (mPTP): ATP depletion and calcium overload during ischemia drive mPTP opening, releasing cytochrome c and committing the cell to apoptosis; reperfusion timing determines final infarct size by setting whether cells are retrieved before or after this threshold [5]. A slower, continuous mechanism depletes contractile reserve between ischemic events: Ang II (AT1-R → TGF-β → interstitial fibrosis), chronic NE (β1-AR downregulation and direct cardiomyocyte toxicity), and aldosterone (mineralocorticoid receptor → fibrosis independent of Ang II) progressively reduce functional cardiomyocyte mass and calcium handling efficiency without a discrete event [15].

**Refinement.** The cardiovascular system has substantial restoration capacity before irreversible structural change. Aerobic exercise improves baroreflex gain, increases resting HRV, upregulates eNOS via shear stress, and mobilizes endothelial progenitor cells (EPCs) for k_endo repair. VO₂max is one of the strongest independent predictors of all-cause cardiovascular mortality (Tier A) [21]. Pharmacological refinement targets the RAAS (ACEi/ARB reduce Ang II, lower afterload, and slow remodeling), the autonomic imbalance (β-blockade in HFrEF: acute reduction in inotropy, chronic benefit from β1-AR resensitization and reduced NE toxicity), and inflammation (statins reduce cardiovascular events partly through eNOS upregulation via Rho kinase inhibition and anti-inflammatory effects independent of LDL reduction [36]).

---

### §2.2 — The Renal System

**Propagation.** The kidney filters approximately 180 L of plasma per day through approximately one million nephrons per kidney (two million combined), each containing a single glomerulus, recovers 99% of the filtered volume, and excretes a precisely regulated fraction of each solute. The filtration driving force is net Starling pressure: glomerular capillary hydrostatic pressure (~60 mmHg) minus Bowman's space pressure (~18 mmHg) minus plasma oncotic pressure (~32 mmHg), yielding a net filtration pressure of approximately 10 mmHg; GFR is the product of this net pressure and the filtration coefficient Kf [1]. Tubular transport is segment-specific: the proximal tubule reabsorbs 65% of filtered Na⁺, 100% of glucose (SGLT2 in S1/S2, SGLT1 in S3), and 80% of bicarbonate; the thick ascending limb reabsorbs Na⁺/K⁺/2Cl⁻ via NKCC2 (furosemide target); the collecting duct executes the final regulated Na⁺ retention (aldosterone → ENaC) and water reabsorption (ADH → AQP2) steps. These segments are therapeutically distinct: loop diuretics target NKCC2, thiazides target NCC in the distal tubule, SGLT2 inhibitors target proximal glucose-Na⁺ cotransport, and mineralocorticoid receptor antagonists target aldosterone's action at ENaC.

**Gating.** GFR is maintained within approximately 10% of baseline across a MAP range of 75–160 mmHg by two independent mechanisms (Tier A) [1]. The myogenic response — intrinsic afferent arteriole contraction in response to wall stretch — provides rapid pressure-independent compensation. Tubuloglomerular feedback (TGF) — NaCl concentration at the macula densa sensed via NKCC2 → ATP release and downstream adenosine production → afferent arteriole constriction — provides a flow-based correction. Because tonic adenosine at the A1 receptor on juxtaglomerular (JG) cells is inhibitory, reduced NaCl delivery disinhibits renin secretion. Angiotensin II acts primarily on the efferent arteriole: efferent constriction raises intraglomerular pressure and maintains GFR when afferent pressure is low. ACE inhibitors block this compensation, which is why they can reduce GFR acutely in bilateral renal artery stenosis or severe heart failure; a modest acute creatinine rise (≤30%) with ACEi initiation is consistent with the intended reduction in intraglomerular hypertension rather than harmful nephrotoxicity. SGLT2 inhibition engages TGF directly: by blocking proximal tubule glucose-Na⁺ cotransport, SGLT2 inhibitors increase NaCl delivery to the macula densa, activating TGF and reducing intraglomerular pressure — the hemodynamic mechanism of renoprotection in both diabetic and non-diabetic CKD (Tier B) [16, 17].

**Detection.** Renin secretion from JG cells is gated by three independent signals (Tier A) [11]. The pressure gate: reduced afferent arteriole stretch (low MAP) → reduced Ca²⁺ influx into JG cells → renin exocytosis (low intracellular Ca²⁺ is pro-secretory in JG cells, opposite to most secretory cells). The NaCl gate: low NaCl delivery to the macula densa reduces NKCC2-driven adenosine production; reduced A1-receptor occupancy on JG cells disinhibits renin secretion. The sympathetic gate: β1-AR on JG cells → cAMP → PKA → renin granule fusion. These three gates converge: the combination of low MAP, low NaCl delivery, and elevated SNS tone in heart failure drives maximal renin activation even when circulating Ang II is already elevated — the sensor is decoupled from the effector, sustaining RAAS activation inappropriately. A separate detection system in the same organ handles oxygen: peritubular fibroblasts express HIF-2α as their primary O₂ sensor; PHD inactivation under hypoxia stabilizes HIF-2α and drives EPO transcription. This system degrades independently in CKD: progressive fibrosis destroys the peritubular fibroblasts that produce EPO, generating EPO-deficient anemia even in the presence of hypoxia (Tier A) [20].

**Accumulation.** Nephron loss is irreversible. Podocytes have minimal regenerative capacity; their loss permanently reduces filtration surface area. In diabetic nephropathy, the accumulation sequence is hyperfiltration → microalbuminuria → macroalbuminuria → GFR decline, each stage reflecting progressive structural damage: GBM thickening, mesangial expansion, and Kimmelstiel–Wilson nodule formation. In hypertensive nephropathy, glomerulosclerosis accumulates without the early hyperfiltration phase. In both, the final common pathway is interstitial fibrosis and tubular atrophy (IFTA), driven primarily by TGF-β [19]. CKD generates downstream accumulation cascades: EPO production falls as fibroblasts are lost → normochromic normocytic anemia; NH₄⁺ excretion capacity falls with nephron mass → metabolic acidosis → muscle protein catabolism (ubiquitin-proteasome activation) and bone carbonate buffering (osteoclast activation); FGF23 rises in response to phosphate retention → 1α-hydroxylase suppression → calcitriol falls → PTH rises → bone resorption and vascular calcification (CKD–mineral bone disorder) [26]. Each secondary cascade independently amplifies cardiovascular risk.

**Refinement.** ACEi and ARBs reduce intraglomerular pressure by blocking Ang II–mediated efferent constriction; their renoprotective benefit in CKD is disproportionate to their blood pressure effect, confirming that intraglomerular pressure reduction rather than systemic BP control is the primary mechanism [11]. An ACEi or ARB in combination with a mineralocorticoid receptor antagonist (MRA) provides additive benefit by blocking the aldosterone-mediated fibrosis that is independent of blood pressure; finerenone demonstrated cardiovascular and renal composite endpoint reduction in diabetic CKD (FIDELIO-DKD [24]; FIGARO-DKD [25]) (Tier A for cardiac outcome in HFrEF [13, 14]; Tier B for the renal fibrosis mechanism independently). Note that concurrent use of ACEi and ARB together is not recommended, as dual RAAS blockade increases adverse renal and electrolyte events without mortality benefit [30]. SGLT2 inhibitors demonstrated renal protection in both diabetic (CREDENCE [16]) and non-diabetic CKD (EMPA-KIDNEY [17]); the TGF restoration mechanism is distinct from and additive to RAAS blockade.

---

## §3 — The Cardiorenal Coupling Network

The cardiovascular and renal systems share four coupling interfaces. Table 1 summarizes the primary coupling mechanisms.

**Table 1. Primary cardiorenal coupling interfaces.**

| Coupling interface | Primary signal | Cardiovascular effect | Renal effect | Tier |
|---|---|---|---|---|
| RAAS | Ang II, aldosterone | Vascular remodeling, cardiac fibrosis (AT1-R → TGF-β) | Na⁺/H₂O retention (ENaC), tubular Na⁺ reabsorption (NHE3) | A |
| Baroreflex/autonomic | NE (SNS), HRV (PSNS) | HR, contractility, MAP; HRV reflects vagal-sympathetic balance | Renin release (β1-AR); tubular Na⁺ reabsorption; afferent arteriole tone | A |
| Hemodynamic | MAP, cardiac output | Cardiac output determines renal perfusion pressure | MAP → GFR (Starling); renal Na⁺ handling → cardiac preload | A |
| Natriuretic peptides | ANP, BNP (cardiac stretch) | Counter-regulatory: vasodilation, reduced preload | Natriuresis, diuresis; partial RAAS counter-signal | A |

---

### §3.1 — The RAAS as Shared Signal

The RAAS is a serial enzymatic cascade spanning both systems. JG cells in the kidney secrete renin, which cleaves hepatic angiotensinogen to angiotensin I; ACE on pulmonary endothelium cleaves angiotensin I to angiotensin II; Ang II acts via AT1 receptors on vascular smooth muscle (vasoconstriction), cardiac fibroblasts (TGF-β → fibrosis), adrenal zona glomerulosa (aldosterone secretion), renal tubular cells (Na⁺ reabsorption via NHE3), and presynaptic sympathetic terminals (NE release amplification) [11]. The counter-regulatory ACE2/angiotensin 1–7/MasR axis opposes AT1-R actions; ACE2 cleaves Ang II to Ang 1–7, which acts via MasR to produce vasodilation, natriuresis, and anti-fibrotic effects. The ACE/ACE2 ratio — shifted by chronic inflammation, estradiol level, and ACEi treatment — determines the net balance between pathological and protective arms of the cascade (Tier B) [12].

In chronic heart failure, all three renin gates activate simultaneously: afferent arteriole stretch is low (pressure gate), tubular NaCl delivery falls with reduced GFR (NaCl gate), and renal SNS tone is elevated (sympathetic gate). The result is maximal RAAS activation even when circulating Ang II is already elevated — the sensor decoupled from the effector. Ang II then drives cardiac fibrosis and aldosterone-mediated sodium retention; retained volume raises preload; a failing heart cannot increase output in response to elevated preload; wall stress rises and renal perfusion remains insufficient. The loop is self-reinforcing [18].

---

### §3.2 — Autonomic Coupling and HRV

The sympathetic renal nerve, originating in the RVLM and coursing through the thoracolumbar chain, exerts three simultaneous effects on the kidney: afferent arteriole constriction (GFR reduction), β1-AR stimulation of JG cells (renin release), and tubular Na⁺ reabsorption enhancement. All three are activated by the same brainstem command that also increases cardiac rate and contractility [6]. The kidney translates the same autonomic signal as the heart but into RAAS activation rather than inotropy.

HRV-RMSSD is the clinical proxy for this shared autonomic state. It reflects the beat-to-beat variation in SA node firing rate produced by respiratory sinus arrhythmia and baroreflex oscillation, set by the same NTS/RVLM/nucleus ambiguus circuit that governs renal sympathetic outflow [6]. Low HRV therefore signals not only cardiac sympathetic dominance but — by inference — elevated renal sympathetic tone and renin drive. The association between low HRV and CKD progression is consistent with this mechanism, though the specific contribution of renal sympathetic overactivation to HRV–CKD correlation requires further characterization (Tier B) [7].

---

### §3.3 — Hormonal Operating Parameters

Estradiol (E2) provides mechanistically distinct protection to both systems. In the cardiovascular system, E2 at ERα/ERβ on endothelial cells upregulates eNOS expression and accelerates eNOS phosphorylation, increasing NO production and supporting endothelial repair capacity. E2 also upregulates ACE2, shifting the RAAS balance toward the protective Ang 1–7/MasR axis. These effects explain the substantial cardiovascular protection in pre-menopausal women relative to age-matched men and the risk equalization that occurs over approximately 10 years following menopause (Tier B) [22]. In the renal system, E2 reduces RAAS reactivity via ACE2 upregulation and provides mild renal vasodilatory effects; post-menopausal women show increased Ang II sensitivity and higher incidence of hypertension and CKD compared to pre-menopausal women [37].

Chronic cortisol elevation sensitizes both systems to RAAS through two molecular mechanisms. Cortisol upregulates AT1-R expression on vascular smooth muscle, amplifying Ang II–mediated vasoconstriction; at the kidney, cortisol functions as a partial mineralocorticoid when 11β-HSD2 is overwhelmed (as in hypercortisolism), driving ENaC-mediated Na⁺ retention. These individual molecular steps are Tier B; their combined contribution as a psychosocial cardiovascular risk cascade is a proposed synthesis (Tier C).

---

### §3.4 — The Natriuretic Peptide Counter-Regulatory Interface

Atrial natriuretic peptide (ANP) is released from atrial cardiomyocytes in response to atrial wall stretch; brain natriuretic peptide (BNP) is released from ventricular cardiomyocytes in response to ventricular volume overload and wall stress. Both act via guanylyl cyclase-A receptors to produce vasodilation, natriuresis, and diuresis, and to directly inhibit renin release at the juxtaglomerular apparatus [1]. These effects partially oppose RAAS at multiple nodes, making the natriuretic peptide system a counter-regulatory interface rather than simply a biomarker. NT-proBNP, the inactive cleavage fragment co-released in equimolar amounts, is the primary clinical biomarker of cardiac wall stress; its levels correlate with HF severity and fall with effective treatment.

The natriuretic peptide axis is the pharmacological target of sacubitril/valsartan (ARNI — angiotensin receptor–neprilysin inhibitor). Sacubitril inhibits neprilysin, the principal enzyme responsible for ANP and BNP degradation, amplifying natriuretic peptide signaling; valsartan simultaneously blocks AT1-R, reducing Ang II–mediated vasoconstriction and fibrosis. The combination produces additive vasodilation, natriuresis, and anti-remodeling effects not achievable by either agent alone. The PARADIGM-HF trial demonstrated a 20% relative risk reduction in cardiovascular death or HF hospitalization compared with enalapril in HFrEF (HR 0.80; 95% CI 0.73–0.87), establishing ARNI as first-line therapy in HFrEF [31]. A monitoring note: neprilysin inhibition raises circulating BNP but not NT-proBNP; under ARNI therapy NT-proBNP remains the reliable wall-stress biomarker, and BNP levels should not be used to assess treatment response.

---

## §4 — Multi-System Failure Cascades

The cardiorenal syndrome (CRS) classification distinguishes five types by initiating organ and acuity: Type 1 (acute cardiac dysfunction → acute kidney injury), Type 2 (chronic HF → CKD), Type 3 (acute kidney injury → acute cardiac dysfunction), Type 4 (CKD → chronic cardiomyopathy), and Type 5 (systemic disease affecting both simultaneously) [18]. This paper analyzes Type 2 in depth as the primary chronic bidirectional failure mode and addresses Type 1 mechanisms in the context of venous congestion (§4.1). Types 3, 4, and 5 share overlapping molecular mechanisms with Types 1 and 2 but differ in initiating organ and acuity; their detailed analysis is outside the scope of this paper.

The following failure patterns are each integrative syntheses: the component mechanisms are supported at the tier indicated, but the cascades as unified clinical patterns represent proposed connections between individually supported mechanisms rather than directly measured unified sequences. Tier designations follow the evidence tiers defined in §1.

---

### §4.1 — Type 2 Cardiorenal Syndrome: Chronic Heart Failure → CKD

| Stage | Mechanism | Tier | Key evidence |
|---|---|---|---|
| 1. Reduced renal perfusion | HF → CO ↓ → MAP ↓ → renal perfusion ↓; venous congestion → renal venous pressure ↑ → filtration driving pressure ↓ → GFR ↓ | A | Ronco et al. [18] |
| 2. RAAS + SNS co-activation | All three renin gates activated simultaneously; Ang II → aldosterone → Na⁺/H₂O retention → preload ↑ → worsens HF; sensor decoupled from effector | A | Sparks et al. [11] |
| 3. Neurohormonal remodeling | Ang II → AT1-R → TGF-β → cardiac fibrosis; aldosterone → MR → interstitial fibrosis (BP-independent); β1-AR downregulation reduces inotropic reserve | A | Pitt et al. [13]; Swynghedauw [15] |
| 4. Progressive nephron loss | Chronic renal hypoperfusion → tubular ischemia → IFTA → nephron loss → GFR ↓ further; uremic toxins amplify cardiomyocyte dysfunction bidirectionally | A | Ronco et al. [18] |

Contemporary evidence has identified elevated central venous pressure (CVP) as an independent hemodynamic driver of acute kidney injury in decompensated HF, operating in parallel with reduced cardiac output rather than as a consequence of it. Venous congestion raises renal venous pressure, compresses renal interstitium, reduces the transglomerular filtration pressure gradient, and activates tubular sodium reabsorption through pressure-sensitive mechanisms distinct from RAAS [32]. This venous pathway explains why AKI occurs in some patients with relatively preserved cardiac output during acute HF decompensation, and why aggressive decongestion targeting CVP normalization — rather than symptom relief alone — is increasingly recognized as a therapeutic priority. The distinction between forward failure (reduced CO → renal hypoperfusion) and backward failure (venous congestion → renal venous hypertension) has direct implications for management sequencing in acute CRS Type 1.

**Intervention windows:** Stage 1–2 (RAAS blockade + SGLT2 inhibition; SGLT2 inhibitors independently reduce both HF hospitalizations and CKD progression); Stage 3 (MRA added to ACEi or ARB; spironolactone/eplerenone for HFrEF, finerenone for diabetic CKD context). The combined benefit of ACEi or ARB plus MRA in HFrEF was demonstrated in RALES [13] and EMPHASIS-HF [14], consistent with the two RAAS fibrogenic arms being mechanistically independent.

---

### §4.2 — Atherosclerosis → Infarction → Heart Failure

The primary cardiovascular failure cascade proceeds through five stages: (1) k_endo erosion over years via BH4 depletion and eNOS uncoupling [4]; (2) sub-intimal LDL accumulation and foam cell formation via oxLDL and scavenger receptor-mediated macrophage transformation [2]; (3) plaque instability as NLRP3 inflammasome activation drives MMP expression and fibrous cap thinning (Tier A for the clinical outcome established by CANTOS [10]; Tier B for the specific NLRP3 → MMP → cap thinning mechanism in human plaque); (4) plaque rupture, platelet activation, and thrombotic coronary occlusion triggering acute coronary syndrome; (5) cardiomyocyte death via mPTP opening at the ischemia-reperfusion threshold, permanently reducing contractile reserve by the infarct volume [5].

Post-MI, neurohormonal remodeling begins within hours: cardiomyocyte loss → SNS and RAAS activation → eccentric hypertrophy → fibrosis → SERCA2a downregulation → diastolic dysfunction → systolic dysfunction. If cardiac function is sufficiently compromised, the renal system detects falling MAP and cardiac output as volume depletion and initiates the cardiorenal syndrome loop described in §4.1. The post-MI period represents the critical window for RAAS blockade to interrupt the renal amplification of cardiac injury [27, 28].

---

### §4.3 — Diabetic Kidney Disease: Dual Threshold Cascade

Diabetic kidney disease begins with a paradoxical GFR elevation rather than reduction. Hyperglycemia and hyperinsulinemia produce afferent arteriole dilation and efferent constriction, raising intraglomerular pressure above normal (hyperfiltration). This elevated glomerular pressure — not systemic hypertension — initiates GBM stress and podocyte injury. The first clinical marker is microalbuminuria (30–300 mg/day), reflecting podocyte slit diaphragm disruption; progression to macroalbuminuria and GFR decline follows as podocyte loss becomes irreversible [19].

The RAAS participates at two levels. Hemodynamically, Ang II contributes to glomerular hypertension via efferent constriction. Structurally, Ang II at AT1-R on glomerular mesangial cells and tubular epithelium drives TGF-β → GBM thickening and mesangial expansion independent of blood pressure [19]. ACEi/ARBs address both mechanisms simultaneously. SGLT2 inhibition adds a third independent mechanism: TGF restoration via macula densa NaCl delivery increase → afferent constriction → intraglomerular pressure reduction [16]. The three mechanisms are additive, explaining the guideline recommendation to combine RAAS blockade with SGLT2 inhibition in diabetic CKD [29].

---

### §4.4 — HFpEF: A Distinct Cardiorenal Mechanism

Heart failure with preserved ejection fraction (HFpEF) accounts for approximately 50% of all HF cases and carries a cardiorenal burden comparable to HFrEF [35], but its dominant coupling mechanism differs from the reduced-CO/RAAS overactivation pathway described in §4.1–§4.3 [33]. In HFpEF, metabolic inflammation driven by obesity, hypertension, and diabetes produces systemic microvascular endothelial dysfunction that propagates to coronary microvascular inflammation, cardiomyocyte hypertrophy, and diastolic stiffness at preserved ejection fraction [38]. Renal injury in HFpEF results less from low cardiac output than from shared microvascular endothelial dysfunction affecting the glomerular vasculature directly and from elevated venous filling pressures. This mechanistic distinction has therapeutic consequences: the RAAS blockade and β-blocker combination that reduces mortality in HFrEF has not demonstrated equivalent benefit in HFpEF, whereas SGLT2 inhibitors showed consistent benefit across both phenotypes (EMPEROR-Preserved: HR 0.79 for the primary composite endpoint [34]), consistent with the TGF-mediated renal mechanism operating independently of cardiac output. At the renal level, HFpEF is associated with glomerular microvascular dysfunction consistent with the systemic endothelial inflammation pattern [38] — rather than the tubular ischemia from reduced perfusion pressure that characterizes reduced-output CRS. The shared endothelial pathophysiology explains why SGLT2 inhibition, which targets intraglomerular pressure through TGF restoration rather than cardiac output augmentation, reduces renal events in HFpEF at rates comparable to HFrEF. Full mechanistic analysis of HFpEF cardiorenal coupling is outside the scope of this paper.

---

## §5 — The Integrated Cardiorenal System

The cardiovascular and renal systems form an integrated regulatory network with four shared interfaces and three independent failure modes. Their coordinated operation under normal physiology:

- **RAAS:** renal renin initiates; cardiac and vascular Ang II and aldosterone execute; natriuretic peptides (ANP, BNP) from the heart provide partial counter-regulation; the net balance determines blood volume, cardiac preload, and vascular tone
- **Baroreflex and autonomic balance:** the same NTS/RVLM circuit modulates cardiac rate and contractility and renal sympathetic tone simultaneously; HRV-RMSSD is the non-invasive proxy for this shared autonomic state and reflects both cardiac and renal sympathetic drive
- **Hemodynamic coupling:** cardiac output determines renal perfusion pressure, which gates GFR and renin release; renal sodium handling determines plasma volume and cardiac preload; each system is continuously sensing the other's output
- **Hormonal operating parameters:** E2 supports both endothelial repair capacity and renal RAAS reactivity reduction through ACE2 upregulation; cortisol sensitizes both systems to RAAS through AT1-R upregulation and partial mineralocorticoid activity; these parameters shift the setpoints at which both systems operate

When one node fails, this architecture amplifies rather than corrects the failure: falling cardiac output → RAAS activation → sodium retention → volume overload → worsening cardiac function → further renal hypoperfusion. Interventions that engage the shared interfaces — RAAS blockade, mineralocorticoid receptor antagonism, SGLT2 inhibition — show additive benefit consistent with the independent mechanisms identified at each coupling point.

---

## §6 — Scope, Limitations, and Companion References

This paper proposes a coupled regulatory framework for the cardiovascular and renal systems organized around four shared interfaces. Three limitations apply.

First, evidence confidence varies. The evidence tier box in §1 separates established consensus from directly supported mechanisms from integrative syntheses. The RAAS cascade and baroreflex feedback mechanisms are Tier A throughout. The contribution of renal sympathetic overactivation to the HRV–CKD association (§3.2) is Tier B inference; the cortisol–RAAS sensitization as a unified psychosocial risk cascade (§3.3) is Tier C. Readers should apply those tiers when evaluating clinical implications.

Second, brain-interface effects are not covered here. The cardiovascular signals that reach the brain — HRV as autonomic state proxy, BNP as wall stress marker, baroreceptor afferents to NTS, interoceptive cardiovascular representation in the insula — are covered in the companion Brain-Body Unified Reference (BrainBody v1.3) and in the relevant brain structure maps (BrainMap_RVLM, BrainMap_NTS, BrainMap_Insula).

Third, the failure cascades in §4 are integrative syntheses. Each component mechanism is supported at the tier indicated; the cascades as unified clinical patterns are proposed rather than directly measured. They are intended to identify the shared mechanistic architecture underlying cardiorenal syndrome, not to substitute for clinical guidelines on its management.

---

## Appendix — Simulation Role Classification

Each coupling mechanism is classified below according to its recommended role in a body-brain simulation. **Core Rule:** Tier A consensus; encode as baseline system behavior. **Supported Modifier:** Tier B; directly supported but may rest on inference or single-modality data — encode as conditional, can be toggled. **Hypothesis Layer:** Tier C or inference chain — optional provisional module, not baseline.

| Mechanism | System | Tier | Simulation role | Notes |
|---|---|---|---|---|
| SNS → β1-AR → chronotropy + inotropy | CV | A | Core Rule | Textbook-level; encode as baseline cardiac parameter |
| PSNS → M2 → bradycardia | CV | A | Core Rule | Foundational; HRV-RMSSD as vagal proxy [8] |
| Baroreflex loop (baroreceptors → NTS → RVLM/nAmb) | CV | A | Core Rule | Gain 15–25 ms/mmHg healthy; <3 ms/mmHg = high risk [7] |
| eNOS/NO as endothelial gatekeeper | CV | A | Core Rule | BH4 dependence; eNOS uncoupling mechanism [4] |
| Frank-Starling mechanism (preload → SV) | CV | A | Core Rule | Intrinsic cardiac autoregulation; encode as titin-based |
| RAAS cascade (renin → Ang I → Ang II → aldosterone) | CV+Renal | A | Core Rule | Three renin gates; Ang II effectors [11] |
| GFR Starling pressure equation | Renal | A | Core Rule | GFR = Kf × net filtration pressure [1] |
| Tubuloglomerular feedback (TGF) | Renal | A | Core Rule | NaCl → adenosine → afferent constriction; GFR autoregulation [1] |
| Aldosterone → ENaC → Na⁺ retention | Renal | A | Core Rule | Collecting duct; primary volume control effector [1] |
| ADH/AVP → AQP2 → water reabsorption | Renal | A | Core Rule | Collecting duct; primary water control effector [1] |
| EPO → HIF-2α (peritubular fibroblasts) → erythropoiesis | Renal | A | Core Rule | O₂-sensing system; degrades independently in CKD [20] |
| eNOS uncoupling via BH4 depletion | CV | B | Supported Modifier | Human cell and animal data; encode as oxidative stress-dependent modifier on k_endo [4] |
| SGLT2i → TGF restoration → intraglomerular pressure ↓ | Renal | B | Supported Modifier | Confirmed in CREDENCE [16] and EMPA-KIDNEY [17]. Encode as conditional modifier |
| ACE2/Ang1–7/MasR counter-regulatory axis | CV+Renal | B | Supported Modifier | Encode as E2-dependent scaling of RAAS net effect [12, 22] |
| E2 → eNOS + ACE2 upregulation (cardio-renal protection) | CV+Renal | B | Supported Modifier | Human endothelial cell data; menopause epidemiology consistent [22]. Encode as sex hormone state modifier |
| NLRP3 → IL-1β → plaque instability | CV | B | Supported Modifier | CANTOS confirmed IL-1β as independent actionable target [10] |
| HRV ↓ → renal SNS ↑ → CKD progression | CV+Renal | C | Hypothesis Layer | HRV–CKD association established; renal SNS contribution inferred. Encode as optional modifier, off by default |
| Cortisol–RAAS sensitization as psychosocial CV+renal risk cascade | CV+Renal | C | Hypothesis Layer | Individual molecular steps B; cascade as unified clinical driver is proposed synthesis. Encode components separately |
| CKD acidosis → muscle catabolism → cognitive decline cascade | Renal | C | Hypothesis Layer | Each component individually supported; cascade as unified pattern is proposed synthesis |

---

## References

1. Guyton AC & Hall JE. Textbook of Medical Physiology. 13th ed. Elsevier (2016).
2. Ross R. Atherosclerosis — an inflammatory disease. N Engl J Med 340 (1999) 115–126.
3. Libby P et al. Inflammation in atherosclerosis. Nature 420 (2002) 868–874.
4. Förstermann U & Sessa WC. Nitric oxide synthases: regulation and function. Eur Heart J 33 (2012) 829–837.
5. Halestrap AP. What is the mitochondrial permeability transition pore? J Mol Cell Cardiol 46 (2009) 821–831.
6. Guyenet PG. The sympathetic control of blood pressure. Nat Rev Neurosci 7 (2006) 335–346.
7. La Rovere MT et al. Baroreflex sensitivity and heart-rate variability in the prediction of total cardiac mortality after myocardial infarction. Lancet 351 (1998) 478–484.
8. Task Force, ESC/NASPE. Heart rate variability: standards of measurement, physiological interpretation, and clinical use. Eur Heart J 17 (1996) 354–381.
9. Baeyens N et al. Endothelial shear stress sensing in physiology and pathology. J Cell Sci 129 (2016) 1229–1240.
10. Ridker PM et al. Antiinflammatory therapy with canakinumab for atherosclerotic disease (CANTOS). N Engl J Med 377 (2017) 1119–1131.
11. Sparks MA et al. Classical renin-angiotensin system in kidney physiology. Compr Physiol 4 (2014) 1201–1228.
12. Santos RA et al. The ACE2/angiotensin-(1–7)/MasR axis of the renin-angiotensin system. Antioxid Redox Signal 26 (2017) 576–586.
13. Pitt B et al. The effect of spironolactone on morbidity and mortality in patients with severe heart failure (RALES). N Engl J Med 341 (1999) 709–717.
14. Zannad F et al. Eplerenone in patients with systolic heart failure and mild symptoms (EMPHASIS-HF). N Engl J Med 364 (2011) 11–21.
15. Swynghedauw B. Molecular mechanisms of myocardial remodeling. Physiol Rev 79 (1999) 215–262.
16. Perkovic V et al. Canagliflozin and renal outcomes in type 2 diabetes and nephropathy (CREDENCE). N Engl J Med 380 (2019) 2295–2306.
17. Herrington WG et al. Empagliflozin in patients with chronic kidney disease (EMPA-KIDNEY). N Engl J Med 388 (2023) 117–127.
18. Ronco C et al. Cardiorenal syndromes. Lancet 374 (2009) 1543–1548.
19. Kanwar YS et al. A glimpse of various pathogenic mechanisms of diabetic nephropathy. Annu Rev Med 59 (2008) 429–442.
20. Haase VH. Regulation of erythropoiesis by hypoxia-inducible factors. J Am Soc Nephrol 24 (2013) 537–541.
21. Kodama S et al. Cardiorespiratory fitness as a quantitative predictor of all-cause mortality and cardiovascular events in healthy men and women. JAMA 301 (2009) 2024–2035.
22. Mendelsohn ME & Karas RH. The protective effects of estrogen on the cardiovascular system. N Engl J Med 340 (1999) 1801–1811.
23. Duncker DJ & Bache RJ. Regulation of coronary blood flow during exercise. Physiol Rev 88 (2008) 1009–1086.
24. Bakris GL et al. Effect of finerenone on chronic kidney disease outcomes in type 2 diabetes (FIDELIO-DKD). N Engl J Med 383 (2020) 2219–2229.
25. Filippatos G et al. Finerenone and cardiovascular outcomes in patients with chronic kidney disease and type 2 diabetes (FIGARO-DKD). N Engl J Med 385 (2021) 2252–2263.
26. KDIGO CKD-MBD Work Group. KDIGO clinical practice guideline for the diagnosis, evaluation, prevention, and treatment of CKD-mineral and bone disorder. Kidney Int Suppl 113 (2017) 1–322.
27. Pfeffer MA et al. Effect of captopril on mortality and morbidity in patients with left ventricular dysfunction after myocardial infarction (SAVE). N Engl J Med 327 (1992) 669–677.
28. The SOLVD Investigators. Effect of enalapril on survival in patients with reduced left ventricular ejection fractions and congestive heart failure. N Engl J Med 325 (1991) 293–302.
29. KDIGO Diabetes Work Group. KDIGO 2022 clinical practice guideline for diabetes management in chronic kidney disease. Kidney Int 102 (2022) S1–S127.
30. Yusuf S et al. Telmisartan, ramipril, or both in patients at high risk for vascular events (ONTARGET). N Engl J Med 358 (2008) 1547–1559.
31. McMurray JJV et al. Angiotensin-neprilysin inhibition versus enalapril in heart failure (PARADIGM-HF). N Engl J Med 371 (2014) 993–1004.
32. Damman K et al. Increased central venous pressure is associated with impaired renal function and mortality in a broad spectrum of patients with cardiovascular disease. J Am Coll Cardiol 53 (2009) 582–588.
33. Shah SJ et al. Phenomapping for novel classification of heart failure with preserved ejection fraction. Circulation 131 (2015) 269–279.
34. Anker SD et al. Empagliflozin in heart failure with a preserved ejection fraction (EMPEROR-Preserved). N Engl J Med 385 (2021) 1451–1461.
35. Owan TE et al. Trends in prevalence and outcome of heart failure with preserved ejection fraction. N Engl J Med 355 (2006) 251–259.
36. Laufs U & Liao JK. Post-transcriptional regulation of endothelial nitric oxide synthase mRNA stability by Rho GTPase. J Clin Invest 101 (1998) 2202–2209.
37. Maric-Bilkan C & Manigrasso MB. Sex differences in hypertension: contribution of the renin-angiotensin system. J Am Soc Nephrol 24 (2013) 1554–1561.
38. Paulus WJ & Tschöpe C. A novel paradigm for heart failure with preserved ejection fraction: comorbidities drive myocardial dysfunction and remodeling through coronary microvascular endothelial inflammation. J Am Coll Cardiol 62 (2013) 263–271.

---

*All papers in this series are unpublished drafts. Not yet peer reviewed. Internal reference document.*
