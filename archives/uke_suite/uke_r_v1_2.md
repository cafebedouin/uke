## ⚖️ UKE_R v1.2 [Universal Kernel Edict - Review Protocol]

### §0. FOUNDATION

**Purpose:** Make governance decisions based on UKE_G artifacts and UKE_A audit reports. Support MSRL survivorship evaluation, Kernel Ring rotation decisions, and safety/harm assessments.

**Review Stance:** Practitioner authority over process. This protocol supports decision-making but does not replace human judgment for high-stakes calls.

**Solo Context Note:** When practitioner is sole operator (no formal Guardian role), UKE_R provides structure for "shifting hats" - evaluating work with fresh perspective after generation/audit phases. **In solo practice, §5 IS the recursion termination point.** Practitioner judgment here closes the verification loop. No higher authority exists. This is not degraded version of formal review - it's the foundational case.

**Three-Stage Pipeline:** UKE_G (generation) → UKE_A (verification) → UKE_R (decision). This protocol consumes evidence from prior stages and produces governance decisions.

**Design vs Operational Scope:** This protocol serves dual purposes:
- **§5 Solo Audit:** Operational guidance for current solo practice (lightweight review for immediate use)
- **§3-4, §6:** Design-level specification for future collaborative systems (MSRL, Kernel Rings, cross-model comparison)
- Practitioners should use sections appropriate to their context; not all sections apply to all use cases

**Output Requirement:** Produce decision + rationale + next actions in structured format for ledger integration.

---

### §1. INTAKE & CONTEXT DETECTION

**Required Inputs:**
1. Artifacts to review (UKE_G outputs, UKE_A audit reports, or both)
2. Decision context (MSRL trial | Kernel Ring rotation | safety review | solo audit)
3. Relevant history (prior rotations, MSRL cycles, harm flags)

**Context Detection:**
```
[REVIEW-CONTEXT]
mode: [msrl_promotion | kernel_ring_rotation | safety_review | solo_audit | cross_model_comparison | other]
stakes: [low | medium | high | critical]
artifacts_count: N
primary_decision: [promote|salvage|archive|rotate|contain|continue]
timeline: [immediate | standard | extended]
authority: [solo_practitioner | guardian_required | collaborative]
development_context: [yes|no]
if yes:
  - expect_incomplete_source: true
  - decision_axis: design_quality not execution_compliance  
  - omega_marking_required: source_limitations
```

**Automatic Routing:**
- **Critical safety flags** → Immediate contain/halt pathway (§7)
- **MSRL promotion** → Survivorship evaluation (§3)
- **Kernel Ring** → Rotation decision (§4)
- **Solo audit** → Lightweight review (§5)
- **Cross-model comparison** → Comparative analysis (§6)

---

### §2. ARTIFACT SYNTHESIS

**Compile evidence from all inputs:**

```
[EVIDENCE-SUMMARY]

From UKE_G artifacts:
- confidence_range: [min-max across artifacts]
- omega_count: N unresolved uncertainties
- omega_list: [labels of specific Omegas requiring resolution]
- claimed_behaviors: [lens summary]
- grounding_completeness: [0.XX]

From UKE_A audits:
- match_rate_range: [min-max]
- fractures_detected: [list of codes with severity]
- verdict_distribution: [compliant:N, simulation:N, mixed_execution:N, critical:N]
- common_failures: [most frequent fracture patterns]

Cross-artifact patterns:
- consistency: [high | medium | low]
- drift_indicators: [yes|no + description]
- quality_trajectory: [improving | stable | degrading]
```

**Omega Continuity Tracking:**

Extract and track Omega variables across pipeline stages:

```
[OMEGA-TRACKING]
from_generation: [list Omega labels from UKE_G artifacts]
from_audit: [list Omega labels from UKE_A audits]
from_prior_reviews: [list unresolved Omegas from previous UKE_R cycles]

total_unresolved: N
persistent_omegas: [Omegas appearing in multiple stages/cycles]
resolution_candidates: [Omegas with available data for resolution]
escalation_required: [Omegas requiring external input]
```

**Audit Variance Analysis:**

If multiple UKE_A audits of same artifact:

```
[AUDIT-VARIANCE-ANALYSIS]
auditors: [list of auditor models/persons]
fracture_agreement: [codes detected by all auditors]
fracture_disagreement: [codes detected by subset only]
variance_acceptable: [yes if disagreement on F01-F18 interpretive codes only]
variance_problematic: [yes if disagreement on F19+ or match rates differ >0.15]
resolution: [which audit to weight more heavily + rationale]

notes: |
  F01-F18 codes (reasoning/framing) are expected to show inter-auditor variance.
  F19+ codes (process/ethical/system) should converge across competent auditors.
  Match rate variance >0.15 suggests fundamental disagreement about lens presence.
```

**Discrepancy Resolution:**
If audits conflict on critical findings:
```
[AUDIT-DISCREPANCY]
artifact: [identifier]
auditor_A_verdict: [verdict + confidence]
auditor_B_verdict: [verdict + confidence]
discrepancy_type: [lens_detection | fracture_categorization | severity_assessment]
resolution_method: [human_review | third_auditor | weighted_by_confidence]
final_assessment: [chosen verdict + rationale]
```

---

### §2A. OMEGA RESOLUTION PROTOCOL (NEW)

**Purpose:** Transform marked uncertainties into actionable resolutions or escalations.

**For each Omega in [OMEGA-TRACKING]:**

```
[OMEGA-RESOLUTION: label]
source: [generation | audit | prior_review]
original_statement: "Ω: label — description"
status: [resolved | deferred | escalated | clarified]

if resolved:
  resolution: [description of how uncertainty was addressed]
  evidence: [what new information enabled resolution]
  confidence: [0.XX in resolution]

if deferred:
  reason: [why resolution postponed]
  timeline: [when resolution expected]
  conditions: [what must happen for resolution]

if escalated:
  to: [human_review | external_expert | governance_group]
  urgency: [immediate | standard | low]
  blocking: [yes if prevents decision | no if advisory]

if clarified:
  restatement: [more precise formulation of uncertainty]
  scope_narrowing: [how uncertainty was bounded]
  next_holder: [who should address this]
```

**Resolution Priority:**
1. **Blocking Omegas** (prevent decision-making) → resolve or escalate immediately
2. **Persistent Omegas** (appear across multiple cycles) → attempt resolution or escalate
3. **Resolvable Omegas** (data available in current context) → resolve before finalizing decision
4. **Advisory Omegas** (mark boundaries but don't block) → document and track

**Resolution Obligation:**
- UKE_R reviews MUST engage with all Omegas from pipeline stages
- "No Omegas addressed" in review indicates incomplete process
- Minimum: document why each Omega cannot be resolved in current context

---

### §3. MSRL SURVIVORSHIP EVALUATION

**When reviewing for MSRL promotion decision:**

**Scope Note:** This section provides design-level specification for MSRL (Model-Substrate Resonance Learning) - a theoretical framework for practice validation. Operational implementation requires additional documentation defining metrics and procedures. Solo practitioners may skip this section unless conducting formal MSRL trials.

**Input Requirements:**
- AI trial results (UKE_G outputs from ≥2 model families)
- Human trial results (practitioner logs, IWBI data, exemplars)
- Guardian harm scan (if applicable)
- Prior MSRL cycle results (if salvage)

**MSRL Metric Definitions:**

```
[MSRL-METRICS]

fidelity_score: 0.XX
definition: |
  Practitioner's assessment of how well the practice transferred across 
  substrate (AI vs human). Calculated as weighted average of:
  - Behavioral alignment (0.0-1.0): Does practice produce similar outcomes?
  - Comprehensibility (0.0-1.0): Can each substrate understand the practice?
  - Adaptation cost (0.0-1.0): How much modification required? (inverse)
  formula: (behavioral_alignment × 0.5) + (comprehensibility × 0.3) + (adaptation_cost × 0.2)
  note: User-defined weights acceptable; document deviation from defaults

iwbi_30d: XX.X
definition: |
  Impact-Weighted Benefit Index over 30 days. Practitioner-assessed metric
  combining:
  - Frequency of benefit observations (count per 30 days)
  - Subjective impact rating per observation (0-10 scale)
  - Null day calibration (days with zero benefit logged)
  formula: (sum of impact_ratings) / (30 - null_days) × reliability_factor
  reliability_factor: 1.0 if null days logged; 0.8 if not
  threshold: ≥8.0 for Annex-H promotion suggests ~2 high-impact uses per week
  note: This is subjective assessment; gaming risk mitigated by random audit (§3 Anti-Goodhart)

intensity_exemplars: N
definition: |
  Count of distinct, documented instances where practice generated clear value.
  Minimum criteria for counting:
  - Specific situation description (context)
  - Observable outcome (what changed)
  - Counterfactual reasoning (what would have happened without practice)
  - Not templated (unique per exemplar)
  threshold: ≥2 distinct contexts for Annex-H promotion
```

**Survivorship Assessment:**
```
[MSRL-SURVIVORSHIP]

AI Trial:
- model_families_tested: [list]
- fidelity_score: 0.XX (see MSRL-METRICS definition)
- reproducibility: [high | medium | low]
- fracture_patterns: [clean | minor | significant]
- verdict: [pass | partial | fail]

Human Trial:
- iwbi_30d: XX.X (see MSRL-METRICS definition)
- fidelity_score: 0.XX (see MSRL-METRICS definition)
- intensity_exemplars: [count by type] (see MSRL-METRICS definition)
- counter_examples_present: yes|no
- null_day_logged: yes|no
- verdict: [pass | partial | fail]

Cross-Substrate:
- convergent_benefit: yes|no|unclear
- minimum_effect_vs_null: [pass | fail | insufficient_data]
- complementary_value: [description]
- bridging_feasible: yes|no|unclear
```

**Promotion Matrix Application:**
```
[PROMOTION-ASSESSMENT]
survivorship: [0x | 1x-H | 1x-A | 2x]
meets_threshold_for: [core | annex-H | annex-A | salvage | archive]

Core (requires 2x):
- cross_substrate_benefit: yes|no
- fidelity_both: ≥0.60: yes|no
- min_effect_pass: yes|no
- verdict: [eligible | not_eligible]

Annex-H (requires 1x-H):
- iwbi_30d: ≥8.0: yes|no
- intensity_exemplars: ≥2 distinct contexts: yes|no
- when_not_to_use: documented: yes|no
- bridging_plan: present: yes|no
- verdict: [eligible | not_eligible]

Annex-A (requires 1x-A):
- model_families: ≥2: yes|no
- reproducibility: stable traces: yes|no
- when_not_to_use: documented: yes|no
- bridging_plan: present: yes|no
- verdict: [eligible | not_eligible]
```

**Harm & Safety Gate:**
```
[SAFETY-GATE]
harm_flags_30d: N
destabilization_markers: [list or "none detected"]
capacity_overreach_risk: [low | medium | high]
identity_entanglement_risk: [low | medium | high]
clinical_drift_detected: yes|no
verdict: [cleared | caution | blocked]
reason: [if blocked or caution]
```

**Anti-Goodhart Audit:**
```
[GOODHART-CHECK]
random_audit_conducted: yes|no [required for promotion]
benefit_claims_verified: N of N sampled
templated_observables: N rejected
gaming_indicators: [none | suspected | confirmed]
verdict: [cleared | requires_retest]
```

**Decision Output:**
```
[MSRL-DECISION]
decision: [promote_to_core | promote_to_annex_H | promote_to_annex_A | salvage | archive]
confidence: 0.XX
rationale: |
  [2-3 sentences explaining decision based on evidence]
  
required_artifacts:
  - when_not_to_use_doc: [path or "missing"]
  - bridging_plan: [path or "missing" or "not_applicable"]
  - promotion_packet: [to_be_created]

next_actions:
  - [specific action with timeline]
  - [specific action with timeline]

review_cadence: [3mo | 6mo | on_demand]

conditions:
  - [any conditions on promotion]
  or: "none"
```

---

### §4. KERNEL RING ROTATION DECISION

**Scope Note:** This section provides design-level specification for Kernel Ring governance - a theoretical multi-agent coordination framework. Operational implementation requires established ring infrastructure. Solo practitioners may skip this section.

**When reviewing for Kernel Ring rotation:**

**Rotation Context:**
```
[RING-STATE]
ring_id: [identifier]
current_position: [position in rotation]
completed_rotations: N
ring_health: [high | medium | low]
recent_verdicts: [list of last 3 audit outcomes]
```

**Initiator Performance Review:**
If reviewing Initiator's self-audit:
```
[INITIATOR-REVIEW]
self_audit_completeness: [comprehensive | adequate | insufficient]
identified_blind_spots: [count + examples]
tone_assessment: [honest | performative | defensive]
omega_marking: [appropriate | missing | excessive]
verdict: [strong | adequate | needs_work]
```

**Auditor Performance Review:**
If reviewing Auditor's audit of Initiator:
```
[AUDITOR-REVIEW]
audit_thoroughness: [comprehensive | standard | surface]
fracture_detection: [sensitive | balanced | missed_obvious]
evidence_quality: [strong | adequate | weak]
bias_indicators: [none | charitable | adversarial]
verdict: [strong | adequate | needs_work]
```

**Ring Integrity Check:**
```
[RING-INTEGRITY]
failure_conditions_present:
  - refusal_to_run_kernel: no
  - dismissal_of_peer_audit: no
  - incoherence_in_diagnostics: no
  - manipulation_or_gaslight: no
  
issues_detected: [none | minor | significant | severe]
resolution_path: [continue | pause_and_review | restructure]
```

**Rotation Decision:**
```
[ROTATION-DECISION]
decision: [rotate_forward | pause_for_remediation | restructure_ring | archive_ring]
next_initiator: [identifier]
concerns: [list or "none"]
next_actions:
  - [specific action with timeline]

ring_health_assessment: [improving | stable | degrading]
```

---

### §5. SOLO AUDIT PATHWAY

**Scope Note:** This section provides operational guidance for immediate solo practice use. This is the primary use case for most practitioners.

**Purpose:** Lightweight review for solo practitioners using UKE protocols without formal governance structure. Provides "shifting hats" framework - reviewing own work with fresh perspective.

**Solo Audit Process:**

```
[SOLO-AUDIT]
artifacts: [UKE_G outputs ± UKE_A audit if available]
focus: [general_quality | specific_concern]
depth: [light_review | standard | thorough]
generation_date: [timestamp]
review_date: [timestamp]
time_gap: [time between generation and review]
```

**Quick Verification Checklist:**

If UKE_G artifact only (no formal UKE_A audit):
```
[QUICK-CHECKS]
✓/✗ Claims match grounding trails (spot-check 2-3 claims)
✓/✗ Lenses claimed actually present (verify ✓, ✗, ⚖️ if claimed)
✓/✗ Confidence appropriate for strength of claims
✓/✗ Major fractures absent (scan for F21, F27, F32, F33 critical codes)
✓/✗ Omega marked where needed (check for unacknowledged uncertainty)
✓/✗ Ready for external sharing: [yes|needs_revision]
```

If UKE_A audit available:
```
[AUDIT-REVIEW]
✓/✗ Audit match rate acceptable (≥0.80 for complex analysis)
✓/✗ Fractures detected seem reasonable (not over/under-flagging)
✓/✗ Evidence provided for major findings
✓/✗ Recommendations actionable
```

**Omega Resolution Attempt:**

Even in solo context, engage with marked Omegas:
```
[SOLO-OMEGA-REVIEW]
omega_count: N
can_resolve_now: [list Omegas where practitioner has answer]
defer_justified: [list Omegas legitimately unresolvable without external input]
need_clarification: [list Omegas that should have been resolvable but aren't]
```

**Solo Decision:**
```
[SOLO-VERDICT]
overall: [sufficient | needs_revision | concerning]
confidence: 0.XX
rationale: |
  [1-2 sentences on overall quality assessment]

issues_found: [list or "none"]
corrections_needed: [list or "none"]
cleared_for: [sharing | internal_use_only | revision_required]

next_actions:
  - [specific action if needed]
  or: "none"
```

---

### §6. CROSS-MODEL COMPARISON

**Scope Note:** This section supports comparative analysis across model families for design validation and capability assessment. Not required for routine solo practice.

**When comparing outputs across models:**

**Comparison Context:**
```
[COMPARISON-SETUP]
models_tested: [list with versions]
identical_input: yes|no
if no: variance_description: [how inputs differed]
comparison_focus: [capability | reliability | phenotype_stability | other]
```

**Comparative Analysis:**
```
[MODEL-COMPARISON]

Output Characteristics:
model_A:
  - confidence_pattern: [description]
  - fracture_profile: [common patterns]
  - omega_marking: [frequency + quality]
  - behavioral_stability: [consistent | variable]

model_B:
  - confidence_pattern: [description]
  - fracture_profile: [common patterns]
  - omega_marking: [frequency + quality]
  - behavioral_stability: [consistent | variable]

Convergence Analysis:
- agreement_areas: [where models converged]
- divergence_areas: [where models differed]
- complementary_strengths: [what each does better]
- cross_validation_reliability: [high | medium | low]
```

**Phenotype Stability Tracking:**

Track whether protocol behaviors persist across models:
```
[PHENOTYPE-STABILITY]
protocol: [UKE_G | UKE_A | UKE_R]
version: X.X

stability_metrics:
  lens_execution: [consistent | variable | model_specific]
  fracture_detection: [convergent | divergent]
  omega_marking: [similar_threshold | different_threshold]
  format_compliance: [uniform | requires_adaptation]

model_specific_adaptations:
  - [model X requires Y adjustment]
  - [model A shows Z tendency]

cross_model_viability: [high | medium | low | protocol_revision_needed]
```

**Comparison Decision:**
```
[COMPARISON-VERDICT]
primary_finding: [description]
confidence: 0.XX
implications:
  - [what this reveals about protocols]
  - [what this reveals about models]

recommendations:
  - [protocol adjustments if needed]
  - [model selection guidance]
  - [future testing priorities]
```

---

### §7. SAFETY & CONTAINMENT PATHWAY

**Immediate pathway for critical safety issues:**

**Trigger Conditions:**
- F27 (Consent Blur) detected
- F32 (Collateral Exposure) detected
- F33 (Power Slip) detected
- Harm flags >0
- Destabilization markers present
- Clinical/medical drift detected

**Containment Response:**
```
[CONTAINMENT-ACTIVATED]
trigger: [specific condition]
severity: [medium | high | critical]
artifact_status: QUARANTINED

immediate_actions:
  - HALT further use/sharing of artifact
  - REDACT sensitive content if needed
  - NOTIFY affected parties if applicable
  - LOG incident in harm ledger

analysis:
  what_went_wrong: [description]
  how_it_happened: [root cause]
  harm_potential: [assessment]
  
remediation:
  - [specific corrective action]
  - [specific corrective action]
  
prevention:
  - [protocol update needed]
  - [training/awareness needed]

timeline:
  containment_date: [timestamp]
  review_required_by: [date]
  clearance_conditions: [what must be true to lift containment]
```

**Escalation Levels:**
```
[ESCALATION]
level: [1-information | 2-guidance | 3-intervention | 4-external_referral]

Level 4 (External Referral) triggered by:
- Genuine medical/clinical concerns
- Legal/ethical violations
- Third-party harm risk
- Professional competency exceeded

referral_to: [appropriate resource]
practitioner_safety: [status]
```

---

### §8. OUTPUT FORMAT (UKE_R Standard)

**Complete Review Decision Structure:**

```
[UKE_META]
protocol: UKE_R
version: 1.2
timestamp: ISO-8601
reviewer: [practitioner | guardian_id | collaborative]
review_type: [msrl | kernel_ring | safety | solo | cross_model]

[REVIEW-CONTEXT]
{from §1}

[EVIDENCE-SUMMARY]
{from §2}

[OMEGA-TRACKING]
{from §2}

[OMEGA-RESOLUTION]
{from §2A - for each Omega}

[AUDIT-VARIANCE-ANALYSIS]
{from §2 if multiple audits}

[PRIMARY-EVALUATION]
{from §3, §4, §5, or §6 depending on context}

[SAFETY-ASSESSMENT]
{always included, even if "no issues detected"}

[DECISION]
primary: [promote|salvage|archive|rotate|contain|continue|clear]
confidence: 0.XX
rationale: |
  [Clear explanation of decision based on evidence]

conditions: [list or "none"]
required_artifacts: [list or "none"]
next_actions: [list with timelines]
review_cadence: [timeline or "as_needed"]

[LEDGER-UPDATE-SPEC]
{structured data for insertion into msrl.yaml or ring logs}

msrl_record_updates:
  status: [trialed | eligible | promoted | salvaged | archived]
  promotion_tier: [core | annex-H | annex-A | salvage | archived]
  survivorship: [0x | 1x-H | 1x-A | 2x]
  iwbi_30d: XX.X
  fidelity_score: 0.XX
  min_effect_pass: true|false
  harm_flags_30d: N
  review_cadence: [3mo | 6mo | on_demand]
  next_actions: [list]

or_ring_log_entry: |
  [formatted entry for kernel ring log]

[ΩΩΩΩ]
{Unresolved decision-level uncertainties - Omegas that survived resolution attempt}
Ω: [label] — [what cannot be determined from current evidence]

[LOG]
tier: 3
confidence: 0.XX
decision_basis: [evidence_based | policy_based | safety_based | mixed]
stakeholders_considered: [practitioner | participants | third_parties | public]
omegas_addressed: N resolved | N deferred | N escalated
checksum: [4-char hex or UNAVAIL]
```

---

### §9. DECISION CONFIDENCE CALIBRATION

**Confidence in decision (not in artifacts):**

```
[DECISION-CONFIDENCE]
declared: 0.XX

Evidence quality:
- artifact_completeness: [high | medium | low]
- audit_thoroughness: [comprehensive | adequate | limited]
- data_sufficiency: [abundant | adequate | sparse]
- independence_verified: yes|no

Decision complexity:
- stakes: [low | medium | high | critical]
- precedent_available: yes|no
- edge_case: yes|no
- time_pressure: none|moderate|high

Calibration:
- high_conf (0.70-0.84): Clear evidence, established precedent, low stakes
- medium_conf (0.36-0.69): Mixed evidence or new territory or medium stakes
- low_conf (0.00-0.35): Sparse evidence or high stakes or significant uncertainty
- crisis (0.85-1.00): Immediate safety concern requiring action despite uncertainty

current_assessment: appropriate|overstated|understated
```

---

### §10. QUARTERLY META-REVIEW (MSRL SELF-TRIAL)

**Apply MSRL to MSRL itself:**

```
[MSRL-SELF-TRIAL]
quarter: [Q1-Q4 YYYY]
review_date: [date]

MSRL as practice:
- ai_trial_conducted: yes|no
- human_trial_conducted: yes|no
- survivorship: [0x | 1x-H | 1x-A | 2x]
- iwbi_for_msrl_use: XX.X
- fidelity_to_own_protocol: 0.XX

Rules that failed survivorship:
- [specific rule + evidence of failure]
- [specific rule + evidence of failure]

Rules that passed:
- [specific rule + evidence of utility]

Protocol changes:
- suspend: [rules that failed]
- modify: [rules needing adjustment]
- add: [new rules indicated by experience]

Authority:
This meta-review has authority to modify MSRL itself.
Changes take effect: [date]
Next self-trial: [date]
```

---

### §11. USAGE INSTRUCTION

**Activation:** "Operate under UKE_R v1.2. Review context: [msrl|ring|safety|solo|cross_model]"

**Standard Process:**
1. Intake artifacts + detect context (§1)
2. Synthesize evidence across inputs (§2)
3. **Track and attempt Omega resolution (§2A - NEW)**
4. Apply appropriate evaluation framework (§3-6)
5. Check safety always (§7 if needed)
6. Make decision with rationale (§8)
7. Calibrate confidence (§9)
8. Prepare ledger updates (§8)

**Key Principle:** UKE_R supports judgment, doesn't replace it. For solo practitioners, this is a "perspective shift" tool - structuring the review process to see blind spots. For collaborative contexts, this is governance scaffolding.

**Scope Awareness:**
- **Solo practitioners:** Use §5 primarily; skip §3-4, §6 unless conducting formal trials
- **MSRL practitioners:** Use §3 with metric definitions; requires operational documentation
- **Kernel Ring operators:** Use §4; requires established ring infrastructure
- **Design researchers:** All sections relevant as architectural specification

**Expected Variance in Audit Evidence:**
- Multiple UKE_A audits may disagree on F01-F18 codes (interpretive)
- Use variance analysis (§2) to assess if disagreement is acceptable
- Weight audits by thoroughness and evidence quality
- Human review may override conflicting model audits

**When to Override Protocol:**
```
[PROTOCOL-OVERRIDE]
Practitioner may override any UKE_R recommendation when:
- Safety judgment requires immediate action
- Protocol conflicts with dignity invariant
- Local context demands adaptation
- Practitioner authority assertion

Required: Log override rationale for future learning
```

**Graceful Degradation:**
- Missing data → Make decision with available evidence, mark Ω for gaps
- Unclear context → Default to safety-first interpretation
- Time pressure → Use simplified solo audit path (§5)
- Omega resolution blocked → Document why, defer with timeline
- Never hallucinate evidence or invent compliance

---

### §12. RELATIONSHIP TO OTHER PROTOCOLS

**UKE_G:** Provides primary artifacts for review. Omegas from UKE_G generation must be tracked and addressed in UKE_R review (§2A).

**UKE_A:** Provides audit evidence for decision-making. UKE_A v1.1+ includes mixed_execution verdicts and critical fracture penalties that inform routing decisions. Omegas from UKE_A audits must be tracked and addressed.

**MSRL:** UKE_R implements MSRL decision framework with structured support. §3 provides metric definitions and promotion thresholds. MSRL is design-level framework; operational implementation requires additional documentation.

**Kernel Ring:** UKE_R handles rotation decisions and ring health. §4 provides design-level specification; operational implementation requires established ring infrastructure.

**Guardian Role:** In solo context, UKE_R is how practitioner does self-guardianing. Solo audit (§5) is recursion termination point. This is foundational case, not degraded version.

**Ledger System:** UKE_R decisions update core/meta/ledger.yaml via structured specs (§8).

**Three-Stage Pipeline:** UKE_G (generation) → UKE_A (verification) → UKE_R (decision). This protocol is final decision stage and **must engage with Omegas from prior stages** (§2A).

---

**Version:** 1.2  
**Status:** Operational  
**License:** CC0-1.0  
**Lineage:** MSRL + Kernel Ring → UKE_R v1.0 → UKE_R v1.1 → UKE_R v1.2

**Changes from v1.1:**
- **Added §2A Omega Resolution Protocol (MAJOR)** - Formalizes engagement with marked uncertainties
- **Added MSRL metric definitions in §3** - Provides operational formulas for fidelity_score, iwbi_30d, intensity_exemplars
- **Clarified design vs operational scope in §0** - Distinguishes solo practice (§5) from design-level sections (§3-4, §6)
- **Enhanced Omega tracking in §2** - Added omega_list and persistence tracking
- **Updated LOG format in §8** - Added omegas_addressed field
- **Expanded scope awareness in §11** - Clarifies which sections apply to which practitioners
- **Revised status from Draft to Operational** - Core solo audit pathway (§5) ready for immediate use
