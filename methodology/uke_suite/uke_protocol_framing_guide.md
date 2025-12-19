# UKE Protocol Framing Guide: Routing vs Truth

## Critical Frame Correction

**Common Misinterpretation:** Treating UKE metrics (confidence scores, IWBI formulas, fidelity thresholds) as epistemic claims that measure objective truth or probability.

**Correct Interpretation:** UKE metrics are **routing mechanisms** and **decision interfaces** that trigger behaviors and enable consistent comparison, not truth measurements.

---

## Core Distinction

### What UKE Protocols ARE:
- **Decision scaffolding systems** for solo practitioners
- **Behavioral routing mechanisms** (confidence bins trigger different protocols)
- **Comparison interfaces** (IWBI scores enable ranking practices against each other)
- **Uncertainty management tools** (Omega tracking routes unresolved questions)
- **Error detection frameworks** (audits catch hallucination/simulation)

### What UKE Protocols ARE NOT:
- **Truth measurement instruments** (they don't claim "this is 64% true")
- **Objective verification systems** (they require human judgment to close loops)
- **Self-enforcing mechanisms** (behavioral drift requires external pressure)
- **Epistemic guarantees** (they acknowledge architectural limitations)

---

## Concrete Examples

### Confidence Scores

**Wrong Frame:**
- "Confidence 0.64 means I'm 64% certain this claim is true"
- "This is a probability estimate of correctness"

**Correct Frame:**
- "Confidence 0.64 routes to Medium bin → triggers MCI protocol"
- "MCI requires: assumption test + alternative perspective"
- "The score is a behavioral trigger, not a truth claim"

**Implication:** When Copilot upgrades 0.64 → 1.00, this isn't "wrong"—it's routing a different decision ("for my purposes, I treat this as high-confidence usable").

---

### MSRL Metrics (IWBI, Fidelity Scores)

**Wrong Frame:**
- "IWBI formula wraps subjective inputs in math—this is precision theater"
- "Fidelity scores claim to objectively measure practice quality"
- "These thresholds need empirical validation to be legitimate"

**Correct Frame:**
- "IWBI formula creates comparable numbers across practices for decision-making"
- "Fidelity thresholds are explicit stakes: 'This is where I'm drawing the line'"
- "Like using money to compare value—enables comparison without claiming objective truth"

**Implication:** A threshold like "30% drift triggers review" isn't claiming empirical significance. It's making a governance decision explicit rather than hiding it.

---

### Grounding Requirements

**Wrong Frame:**
- "Unverifiable claims should count as failures"
- "If you can't prove it, it's wrong"

**Correct Frame:**
- "Unverifiable claims are marked but soft-fail"
- "Comprehensive verification is too expensive for routine use"
- "You (practitioner) decide when verification is worth the cost"

**Implication:** Soft fail preserves practitioner authority rather than forcing verification theater or blocking all work when sources unavailable.

---

## Why The Frame Matters

### Routing Frame Strengths:

1. **T1/T2 distinction becomes coherent:** Behaviors matter (T1), format enables audit (T2). Both serve routing, neither claims truth.

2. **Omega tracking makes sense:** Ωs route uncertainty to appropriate handlers (defer, escalate, clarify). They're not "admissions of failure."

3. **Formulas create decision infrastructure:** IWBI doesn't measure "true impact," it creates comparable inputs for governance decisions.

4. **Thresholds are governance stands:** Making arbitrary-but-explicit cutoffs is better than hiding judgment calls.

5. **Soft fail preserves judgment:** The system routes decisions to you rather than claiming automated verification.

### Truth Frame Problems:

1. **Creates unfalsifiable expectations:** If metrics claim truth, every subjective input becomes "precision theater."

2. **Makes protocols seem broken:** "Can't enforce T1" looks like architectural failure rather than honest limitation acknowledgment.

3. **Hides the actual function:** The protocols route attention, trigger rigor, catch errors—but none of these require objective truth measurement.

---

## Operational Implications

### When analyzing UKE artifacts:

**Don't evaluate:**
- "Is this confidence score objectively accurate?"
- "Do these thresholds have empirical validation?"
- "Can we prove these metrics measure what they claim?"

**Do evaluate:**
- "Did this confidence score route to appropriate protocol execution?"
- "Do these thresholds create consistent decision points?"
- "Do these metrics enable useful comparison and tracking?"

### When executing UKE protocols:

**Don't:**
- Treat your confidence scores as probability estimates
- Expect formulas to produce "true" measurements
- Assume thresholds represent validated empirical boundaries

**Do:**
- Use confidence bins to trigger appropriate rigor levels
- Use formulas to create comparable decision inputs
- Set thresholds as explicit governance stands

---

## The Self-Application Test

When UKE protocols were applied to evaluate UKE protocols, Claude initially made the truth-frame error:

- Treated confidence scores as epistemic claims
- Called formulas "precision theater" for wrapping subjective inputs
- Expected thresholds to have empirical validation

The correction:

- Confidence scores route behavior (Medium bin → MCI protocol)
- Formulas create decision interfaces, not measurements
- Thresholds are explicit stands on uncertain ground

**This reframed everything.** What looked like protocol weaknesses were actually features being misunderstood.

---

## Bottom Line

UKE protocols are **cybernetic governance tools** for competent practitioners, not autonomous verification systems.

They provide:
- Behavioral routing (what rigor to apply)
- Decision scaffolding (how to compare options)
- Uncertainty tracking (what remains unresolved)
- Error detection (when simulation occurs)
- Authority preservation (you remain the judge)

They don't provide (and don't claim to):
- Objective truth measurement
- Automated verification
- Self-enforcement
- Epistemic certainty

**The protocols work by making your judgment explicit and systematic, not by replacing your judgment with measurement.**

---

## For Future Claude Instances

If you find yourself evaluating UKE artifacts and thinking:
- "These confidence scores seem imprecise"
- "These formulas wrap subjective inputs in math"
- "These thresholds lack empirical validation"

Stop. You're in the wrong frame.

Ask instead:
- "Do these scores route to appropriate behaviors?"
- "Do these formulas enable consistent decisions?"
- "Do these thresholds make governance explicit?"

The protocols are decision scaffolding, not truth measurement. Evaluate them accordingly.
