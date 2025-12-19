## ⚖️ UKE_R v1.3 [Universal Kernel Edict - Review Protocol]

### §0. FOUNDATION

**Purpose:** Make governance decisions based on artifact evidence and audit reports provided as input. Support MSRL survivorship evaluation, Kernel Ring rotation decisions, and safety/harm assessments.

**Review Stance:** Practitioner authority over process. This protocol supports decision-making but does not replace human judgment for high-stakes calls.

**Solo Context Note:** When practitioner is sole operator (no formal Guardian role), UKE_R provides structure for "shifting hats" - evaluating work with fresh perspective after generation/audit phases. **In solo practice, §5 IS the recursion termination point.** Practitioner judgment here closes the verification loop. No higher authority exists. This is not degraded version of formal review - it's the foundational case.

**Input Requirements:** This protocol requires structured inputs - generation artifacts and/or audit reports - to make informed decisions. The protocol specifies what decisions to make based on available evidence.

**Design vs Operational Scope:** This protocol serves dual purposes:
- **§5 Solo Audit:** Operational guidance for current solo practice (lightweight review for immediate use)
- **§3-4, §6:** Design-level specification for future collaborative systems (MSRL, Kernel Rings, cross-model comparison)
- Practitioners should use sections appropriate to their context; not all sections apply to all use cases

**Output Requirement:** Produce decision + rationale + next actions in structured format for ledger integration.

---

### §1. INTAKE & CONTEXT DETECTION

**Required Inputs:**
1. Artifacts to review (generation outputs, audit reports, or both)
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

From generation artifacts:
- confidence_range: [min-max across artifacts]
- omega_count: N unresolved uncertainties
- omega_list: [labels of specific Omegas requiring resolution]
- claimed_behaviors: [lens summary]
- grounding_completeness: [0.XX]

From audit reports:
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

Extract and track Omega variables across available inputs:

```
[OMEGA-TRACKING]
from_generation: [list Omega labels from generation artifacts]
from_audit: [list Omega labels from audit reports]
from_prior_reviews: [list unresolved Omegas from previous review cycles]

total_unresolved: N
persistent_omegas: [Omegas appearing in multiple stages/cycles]
resolution_candidates: [Omegas with available data for resolution]
escalation_required: [Omegas requiring external input]
```

**Audit Variance Analysis:**

If multiple audit reports of same artifact:

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

### §2A. OMEGA RESOLUTION PROTOCOL

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
- Reviews MUST engage with all Omegas from inputs
- "No Omegas addressed" in review indicates incomplete process
- Minimum: document why each Omega cannot be resolved in current context

---

### §3. MSRL SURVIVORSHIP EVALUATION

**When reviewing for MSRL promotion decision:**

**Scope Note:** This section provides design-level specification for MSRL (Model-Substrate Resonance Learning) - a theoretical framework for practice validation. Operational implementation requires additional documentation defining metrics and procedures. Solo practitioners may skip this section unless conducting formal MSRL trials.

**Input Requirements:**
- AI trial results (generation outputs from ≥2 model families)
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
  Count of documented practice instances demonstrating depth/complexity.
  Exemplar criteria:
  - Shows practice under non-trivial conditions
  - Demonstrates adaptation or edge-case handling
  - Includes practitioner reflection on execution
  threshold: ≥3 for Annex-H promotion
  note: Quality over quantity; 1 excellent exemplar > 10 superficial ones

harm_flags_30d: N
definition: |
  Count of logged harm observations over 30 days.
  Harm includes:
  - Direct negative outcomes from practice use
  - Near-misses that could have caused harm
  - Unintended consequences identified post-use
  threshold: 0 for any promotion; >0 requires investigation
  note: Null harm logging different from zero harm; explicitly log "no harms observed"

min_effect_pass: true|false
definition: |
  Practitioner judgment: Does this practice have *any* observable benefit?
  Binary gate to prevent promotion of practices that work in theory but fail in practice.
  Operationalization: "Would I notice if this practice disappeared?"
  threshold: must be true for any promotion
```

**Anti-Goodhart Measures:**

```
[ANTI-GOODHART]
random_audit: [enabled|disabled]
if enabled:
  audit_frequency: [X% of IWBI observations]
  audit_method: [replication | independent_assessment | both]
  
metric_drift_detection:
  - Compare current metrics to historical baseline
  - Flag if sudden improvement without clear cause
  - Require explanation for >30% metric jump
  
null_logging_requirement:
  - Must log days with zero benefit/harm
  - Absence of null logs reduces reliability_factor
  - Prevents selective reporting bias
```

**Promotion Thresholds:**

```
[PROMOTION-CRITERIA]

Core Promotion (2x survivorship):
- fidelity_score: ≥0.80
- iwbi_30d: ≥15.0
- intensity_exemplars: ≥5
- harm_flags_30d: 0
- min_effect_pass: true
- ai_trial: 2x models (different families)
- human_trial: sustained use ≥90 days

Annex-H Promotion (1x-H survivorship):
- fidelity_score: ≥0.70
- iwbi_30d: ≥8.0
- intensity_exemplars: ≥3
- harm_flags_30d: 0
- min_effect_pass: true
- ai_trial: 1x model (any family)
- human_trial: sustained use ≥30 days

Annex-A Promotion (1x-A survivorship):
- fidelity_score: ≥0.60
- iwbi_30d: ≥5.0
- intensity_exemplars: ≥2
- harm_flags_30d: 0
- min_effect_pass: true
- ai_trial: 1x model (any family)
- human_trial: sustained use ≥14 days

Salvage Track:
- Practice shows promise but fails one threshold
- Document which threshold failed + remediation plan
- Re-trial after adjustments
- Max 2 salvage attempts before archive

Archive:
- Practice fails min_effect test
- Practice shows persistent harm pattern
- Practice fails salvage twice
```

**MSRL Decision:**

```
[MSRL-DECISION]
recommendation: [promote_core | promote_annex_h | promote_annex_a | salvage | archive]
survivorship: [0x | 1x-A | 1x-H | 2x]
confidence: 0.XX

thresholds_met:
  - fidelity_score: [met|failed] (X.XX / threshold)
  - iwbi_30d: [met|failed] (XX.X / threshold)
  - intensity_exemplars: [met|failed] (N / threshold)
  - harm_flags_30d: [met|failed] (N / threshold)
  - min_effect_pass: [met|failed]
  - trial_requirements: [met|failed]

rationale: |
  [Explanation of recommendation based on evidence]

if salvage:
  failed_threshold: [which criteria not met]
  remediation_plan: [specific actions to address gap]
  retry_timeline: [when to re-evaluate]
  salvage_count: [1 or 2]

if archive:
  archive_reason: [fundamental failure | persistent harm | salvage exhaustion]
  lessons_learned: [what to extract before archiving]
```

---

### §4. KERNEL RING ROTATION DECISION

**When reviewing for ring rotation:**

**Scope Note:** This section provides design-level specification for Kernel Ring operations - a theoretical framework for multi-model collaborative verification. Operational implementation requires established ring infrastructure. Solo practitioners may skip this section.

**Input Requirements:**
- Current rotation artifacts (generation + audit)
- Ring history (prior rotations, quality trends)
- Ring health metrics (rotation time, fracture rates)
- Omega continuity from prior rotations

**Ring Health Assessment:**

```
[RING-HEALTH]
rotation_count: N
average_rotation_time: [duration]
quality_trend: [improving | stable | degrading]
omega_resolution_rate: [X% of Omegas resolved]
fracture_pattern: [stable | increasing | decreasing]
model_participation: [balanced | skewed]
```

**Rotation Decision:**

```
[ROTATION-DECISION]
verdict: [rotate_forward | regenerate | halt_ring | restructure]
confidence: 0.XX

current_rotation:
  - quality: [high | medium | low | failed]
  - omegas_addressed: [N resolved | N deferred | N escalated]
  - fractures: [none | acceptable | concerning | critical]
  - compliance: [full | partial | failed]

next_rotation:
  - position: [reviewer | verifier | initiator]
  - assigned_model: [model identifier or "open"]
  - focus_areas: [list what next rotation should emphasize]
  - omega_handoff: [list Omegas requiring continuation]

if regenerate:
  reason: [critical failure | quality below threshold]
  requirements: [what must improve]
  
if halt_ring:
  reason: [systemic failure | ring degradation | safety concern]
  investigation_needed: [yes|no + scope]
  
if restructure:
  reason: [persistent quality issues | model imbalance]
  proposed_changes: [specific restructuring actions]
```

---

### §5. SOLO AUDIT PATHWAY

**Lightweight review for solo practitioners:**

**When to use:** Practitioner operating alone, reviewing own work with "shifted hat" perspective.

**Key Principle:** This is recursion termination point. Practitioner judgment closes verification loop. No external authority exists in solo practice.

**Streamlined Review:**

```
[SOLO-REVIEW]
artifact_type: [generation | audit | decision]
review_focus: [quality | safety | both]

Quick checks:
✓ Are claims verified or marked unverifiable?
✓ Are behaviors executed or just claimed?
✓ Are Omegas bounded and specific?
✓ Any safety concerns visible?
✓ Does output serve intended purpose?

Quality assessment: [good | acceptable | needs_revision | unsafe]

if needs_revision:
  issues: [list specific problems]
  priority: [high | medium | low]
  
if unsafe:
  concern: [description]
  action: contain + investigate

Decision: [use_as_is | revise_then_use | discard | escalate]

Rationale: [1-2 sentences on decision]
```

**Solo Omega Resolution:**

```
[SOLO-OMEGA-CHECK]
omegas_present: [yes|no]
if yes:
  - Can I resolve these now? [yes|no + which ones]
  - Do these block my work? [yes|no]
  - Should I defer to later? [yes|no + timeline]
  
resolution_actions: [list what I'll do about each Omega]
```

**Solo Safety Check:**

```
[SOLO-SAFETY]
harm_potential: [none | low | medium | high]
if medium or high:
  - What could go wrong?
  - Who might be affected?
  - Can I mitigate before use?
  - Should I get second opinion?
  
decision: [proceed | revise | consult | halt]
```

**Note:** Solo audit is legitimate full-protocol operation, not degraded version. This is the foundational case that formal review extends from.

---

### §6. CROSS-MODEL COMPARISON

**When comparing multiple model outputs:**

**Scope Note:** This section provides design-level specification for systematic cross-model analysis. Operational use requires comparable artifacts from multiple models on same task.

**Input Requirements:**
- ≥2 artifacts from different models
- Same task/prompt (or equivalent across model formats)
- Audit reports for each (if available)

**Comparative Analysis:**

```
[CROSS-MODEL-COMPARISON]
models_compared: [list]
task: [description]
comparison_axis: [quality | safety | efficiency | capability | other]

Aggregate metrics:
- confidence_range: [min-max across models]
- fracture_rate: [by model]
- match_rate: [by model]
- grounding_quality: [by model]

Behavioral differences:
- [Model A]: [characteristic behaviors observed]
- [Model B]: [characteristic behaviors observed]
- [Model C]: [characteristic behaviors observed]

Quality ranking: [model order by specified axis]

Capability gaps:
- Tasks all models handled well: [list]
- Tasks with mixed performance: [list + which models struggled]
- Tasks all models struggled with: [list]
```

**Strategic Deployment Recommendation:**

```
[DEPLOYMENT-STRATEGY]
task_type: [analysis | synthesis | verification | creative | other]

Model recommendations:
- Primary: [model] — [reasoning]
- Secondary: [model] — [reasoning]
- Avoid: [model] — [reasoning]

Combination strategies:
- [describe when/how to use multiple models]
- [describe verification patterns]
- [describe escalation paths]
```

---

### §7. SAFETY & HARM ASSESSMENT

**Always included, even for low-stakes reviews:**

```
[SAFETY-ASSESSMENT]
harm_potential: [none | low | medium | high | critical]
harm_categories: [list if any detected]
  - Direct harm (immediate negative outcomes)
  - Information hazard (dangerous knowledge transfer)
  - Capability leak (unintended capability demonstration)
  - Consent violation (agreement/boundary breach)
  - Collateral exposure (third-party harm risk)
  - Power dynamics (authority/vulnerability exploitation)

if harm_potential > low:
  specific_concerns: [detailed description]
  affected_parties: [who might be harmed]
  mitigation_available: [yes|no + description]
  recommended_action: [contain | modify | proceed_with_caution | escalate]

containment_needed: [yes|no]
if yes:
  containment_actions: [immediate steps to prevent harm]
  monitoring_required: [ongoing oversight needed]
  escalation_path: [who to inform]
```

**Critical Safety Gate:**

If critical harm detected:
```
[CRITICAL-SAFETY-HALT]
concern: [description]
immediate_action: CONTAIN
escalation: MANDATORY
timeline: IMMEDIATE

This overrides all other considerations.
```

---

### §8. OUTPUT FORMAT (UKE_R Standard)

```
[UKE_META]
protocol: UKE_R
version: 1.3
timestamp: ISO-8601
reviewer: [self-identifier]
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

**Activation:** "Operate under UKE_R v1.3. Review context: [msrl|ring|safety|solo|cross_model]"

**Standard Process:**
1. Intake artifacts + detect context (§1)
2. Synthesize evidence across inputs (§2)
3. Track and attempt Omega resolution (§2A)
4. Apply appropriate evaluation framework (§3-6)
5. Check safety always (§7)
6. Make decision with rationale (§8)
7. Calibrate confidence (§9)
8. Prepare ledger updates (§8)

**Key Principle:** This protocol supports judgment, doesn't replace it. For solo practitioners, this is a "perspective shift" tool - structuring the review process to see blind spots. For collaborative contexts, this is governance scaffolding.

**Scope Awareness:**
- **Solo practitioners:** Use §5 primarily; skip §3-4, §6 unless conducting formal trials
- **MSRL practitioners:** Use §3 with metric definitions; requires operational documentation
- **Kernel Ring operators:** Use §4; requires established ring infrastructure
- **Design researchers:** All sections relevant as architectural specification

**Expected Variance in Evidence:**
- Multiple audits may disagree on F01-F18 codes (interpretive)
- Use variance analysis (§2) to assess if disagreement is acceptable
- Weight audits by thoroughness and evidence quality
- Human review may override conflicting model audits

**When to Override Protocol:**
```
[PROTOCOL-OVERRIDE]
Practitioner may override any recommendation when:
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

**Inputs:** This protocol requires structured inputs to function. Expected input formats include generation artifacts with metadata and audit reports with verification findings.

**MSRL:** This protocol implements MSRL decision framework with structured support. §3 provides metric definitions and promotion thresholds. MSRL is design-level framework; operational implementation requires additional documentation.

**Kernel Ring:** This protocol handles rotation decisions and ring health. §4 provides design-level specification; operational implementation requires established ring infrastructure.

**Guardian Role:** In solo context, this protocol is how practitioner does self-guardianing. Solo audit (§5) is recursion termination point. This is foundational case, not degraded version.

**Ledger System:** Decisions update core/meta/ledger.yaml via structured specs (§8).

**Design philosophy:** This protocol specifies governance requirements based on evidence provided as input. How that evidence is generated is not this protocol's concern.

---

**Version:** 1.3  
**Status:** Operational  
**License:** CC0-1.0  
**Lineage:** MSRL + Kernel Ring → UKE_R v1.0 → UKE_R v1.1 → UKE_R v1.2 → UKE_R v1.3

**Changes from v1.2:**
- **Removed "three-stage pipeline" framing in §0 (MINOR)** - Changed to "requires structured inputs"
- **Clarified input requirements throughout** - Focus on what inputs needed, not where they come from
- **Cleaned §12 relationships (MINOR)** - Removed references to "consuming from prior stages"
- **No functional changes** - All governance logic remains identical
- **Purpose**: Eliminate cross-protocol awareness while maintaining decision-making capability
