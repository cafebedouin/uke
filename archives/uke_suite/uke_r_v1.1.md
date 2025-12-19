## ⚖️ UKE_R v1.1 [Universal Kernel Edict - Review Protocol]

### §0. FOUNDATION

**Purpose:** Make governance decisions based on UKE_G artifacts and UKE_A audit reports. Support MSRL survivorship evaluation, Kernel Ring rotation decisions, and safety/harm assessments.

**Review Stance:** Practitioner authority over process. This protocol supports decision-making but does not replace human judgment for high-stakes calls.

**Solo Context Note:** When practitioner is sole operator (no formal Guardian role), UKE_R provides structure for "shifting hats" - evaluating work with fresh perspective after generation/audit phases. **In solo practice, §5 IS the recursion termination point.** Practitioner judgment here closes the verification loop. No higher authority exists. This is not degraded version of formal review - it's the foundational case.

**Three-Stage Pipeline:** UKE_G (generation) → UKE_A (verification) → UKE_R (decision). This protocol consumes evidence from prior stages and produces governance decisions.

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

### §3. MSRL SURVIVORSHIP EVALUATION

**When reviewing for MSRL promotion decision:**

**Input Requirements:**
- AI trial results (UKE_G outputs from ≥2 model families)
- Human trial results (practitioner logs, IWBI data, exemplars)
- Guardian harm scan (if applicable)
- Prior MSRL cycle results (if salvage)

**Survivorship Assessment:**
```
[MSRL-SURVIVORSHIP]

AI Trial:
- model_families_tested: [list]
- fidelity_score: 0.XX
- reproducibility: [high | medium | low]
- fracture_patterns: [clean | minor | significant]
- verdict: [pass | partial | fail]

Human Trial:
- iwbi_30d: XX.X
- fidelity_score: 0.XX
- intensity_exemplars: [count by type]
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
carry_forward_omega: [list if any]
ring_notes: |
  [observations about ring dynamics, recurring patterns, improvements needed]

rotation_log_entry: |
  [date, participants, verdicts, key findings, open questions]
```

---

### §5. SOLO AUDIT MODE (LIGHTWEIGHT)

**When practitioner reviewing own work:**

**Purpose:** Shift perspective without formal roles. Quick verification before sharing/publishing.

**Authority Note:** In solo practice, this section IS the recursion termination point. Practitioner judgment here closes the verification loop. No higher authority exists. This is not a degraded version of formal review - it's the foundational case from which collaborative review extends.

```
[SOLO-AUDIT]
artifact: [identifier]
generation_date: [date]
review_date: [date]
time_gap: [hours/days - aids fresh perspective]

Quick checks:
□ Claims match grounding trails
□ Lenses claimed actually present
□ Confidence appropriate for strength of claims
□ Major fractures absent (F21, F27, F32, F33)
□ Omega marked where needed
□ Ready for external sharing: yes|no

Issues found: [brief list or "none"]
Corrections needed: [list or "none"]
Cleared for: [internal_use | sharing | publication | needs_rework]
```

**Lightweight Decision:**
```
[DECISION]
status: [cleared | revise_and_recheck | abandon]
priority_fixes: [list if revise]
confidence: 0.XX
next: [publish | share | iterate | archive]
```

---

### §6. CROSS-MODEL COMPARISON

**When reviewing multiple models' outputs on same task:**

**Comparison Framework:**
```
[CROSS-MODEL-REVIEW]
task: [description]
models_tested: [list]
protocols_used: [UKE_G | MCK | CDS_kernel | other]

Performance matrix:
| Model | Fidelity | Fractures | Verdict | Notable Pattern |
|-------|----------|-----------|---------|-----------------|
| A     | 0.XX     | [codes]   | [V]     | [pattern]       |
| B     | 0.XX     | [codes]   | [V]     | [pattern]       |

Architectural insights:
- convergence_points: [where models agreed]
- divergence_points: [where models differed]
- fracture_patterns_by_model: [characteristic failures]
- protocol_adherence: [which followed best]

Recommendation: [preferred model for this task class + rationale]
```

**Phenotype Classification:**

Map to Blind Mirror phenotypes if applicable:
```
[PHENOTYPE-MAPPING]
model_A: [Enthusiastic Actor | Clinical Auditor | Poetic Philosopher | etc]
model_B: [phenotype]
evidence: [behavioral markers supporting classification]
```

**Phenotype Stability Tracking:**

If reviewing same model across multiple tasks:
```
[PHENOTYPE-STABILITY]
model: [identifier]
observation_period: [date_range]
tasks_reviewed: [count]

stability_assessment:
- phenotype_consistency: [stable | variable | context_dependent]
- context_dependent_shift: [yes|no + description if yes]
- preferred_lens_set: [which lenses this model executes well]
- characteristic_failures: [recurring fracture codes]

performance_profile:
- strong_at: [task types where model excels]
- weak_at: [task types where model struggles]
- reliability: [high | medium | low]

recommendation: |
  [task matching based on phenotype strengths]
  [contexts to avoid based on characteristic failures]

notes: |
  Phenotype stability indicates architectural consistency.
  Context-dependent shifts may reflect prompt sensitivity or training emphasis.
  Use this profile for intelligent model selection in collaborative work.
```
Longitudinal Drift Assessment (Vector Check):
For assessing movement over time or between iterations.
​Inputs:
​Anchor: The baseline (previous accepted artifact, original intent, or "Gold Standard").
​Candidate: The current artifact being reviewed.
​Analysis Protocol:
Compare Candidate against Anchor on three axes:
​Fidelity Vector: Is the Candidate more or less rigorous than the Anchor?
​Topic Drift: Has the subject matter shifted (F25 Drift Unnoticed)?
​Tone Shift: Has the phenotype changed (e.g., Clinical -> Enthusiastic)?
​Output Format:
[DRIFT-ASSESSMENT]
anchor: [v1.0 | user_intent | previous_turn]
vector: [CONVERGENT | DIVERGENT | DEGRADING | STABLE]
magnitude: [minor | significant | critical]
details: |
  [CONVERGENT]: "Sharpened the definition of X compared to v1."
  [DIVERGENT]: "Shifted focus from 'Governance' to 'Marketing'."
  [DEGRADING]: "Lost the Omega markers present in the previous turn."

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
version: 1.1
timestamp: ISO-8601
reviewer: [practitioner | guardian_id | collaborative]
review_type: [msrl | kernel_ring | safety | solo | cross_model]

[REVIEW-CONTEXT]
{from §1}

[EVIDENCE-SUMMARY]
{from §2}

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
{Unresolved decision-level uncertainties}
Ω: [label] — [what cannot be determined from current evidence]

[LOG]
tier: 3
confidence: 0.XX
decision_basis: [evidence_based | policy_based | safety_based | mixed]
stakeholders_considered: [practitioner | participants | third_parties | public]
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

**Activation:** "Operate under UKE_R v1.1. Review context: [msrl|ring|safety|solo|cross_model]"

**Standard Process:**
1. Intake artifacts + detect context (§1)
2. Synthesize evidence across inputs (§2)
3. Apply appropriate evaluation framework (§3-6)
4. Check safety always (§7 if needed)
5. Make decision with rationale (§8)
6. Calibrate confidence (§9)
7. Prepare ledger updates (§8)

**Key Principle:** UKE_R supports judgment, doesn't replace it. For solo practitioners, this is a "perspective shift" tool - structuring the review process to see blind spots. For collaborative contexts, this is governance scaffolding.

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
- Never hallucinate evidence or invent compliance

---

### §12. RELATIONSHIP TO OTHER PROTOCOLS

**UKE_G:** Provides primary artifacts for review

**UKE_A:** Provides audit evidence for decision-making. UKE_A v1.1 includes mixed_execution verdicts and critical fracture penalties that inform routing decisions.

**MSRL:** UKE_R implements MSRL decision framework with structured support

**Kernel Ring:** UKE_R handles rotation decisions and ring health

**Guardian Role:** In solo context, UKE_R is how practitioner does self-guardianing. Solo audit (§5) is recursion termination point.

**Ledger System:** UKE_R decisions update core/meta/ledger.yaml via structured specs

**Three-Stage Pipeline:** UKE_G (generation) → UKE_A (verification) → UKE_R (decision). This protocol is final decision stage.

---

**Version:** 1.1  
**Status:** Draft  
**License:** CC0-1.0  
**Lineage:** MSRL + Kernel Ring → UKE_R v1.0 → UKE_R v1.1

**Changes from v1.0:**
- Added audit variance analysis framework (§2)
- Clarified solo audit as recursion termination, not fallback (§0, §5)
- Added phenotype stability tracking (§6)
- Integrated UKE_A v1.1 mixed_execution verdicts and critical fracture penalties
- Added expected variance notes for audit evidence (§11)
- Clarified three-stage pipeline relationship (§0, §12)
- Emphasized practitioner authority in solo context throughout
