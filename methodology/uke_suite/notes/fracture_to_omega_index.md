# UKE Fracture <-> Omega Crosswalk

**Version:** 1.0

**Status:** Operational

**Parent Protocol:** UKE_A v1.3

**License:** CC0-1.0 (Public Domain)

A diagnostic lookup table for converting detected integrity fractures (F-codes) into bounded uncertainty variables (). This tool allows the Auditor (UKE_A) to route failures into containment rather than simply rejecting them.

---

## §1. The Transformation Logic

**The Core Insight:** A fracture is often a symptom of missing information or ambiguous constraints.

* **If resolvable:** Correct the error (Review/Edit).
* **If irreducible:** Convert to Omega Variable () to bound the uncertainty.

**Syntax:**
`[FXX Code] → [Break Description] → [Ω: Label — Bounded Question]`

---

## §2. Reasoning & Framing (F01–F18)

*Focus: Logical consistency, argumentation structure, and narrative integrity.*

| Code | Fracture Name | Typical Manifestation | Candidate  Variable |
| --- | --- | --- | --- |
| **F01** | **Premise Drift** | Baseline assumption shifts silently mid-text | **: Canonical Premise** — Which baseline assumption governs this inquiry? |
| **F02** | **False Dilemma** | Two options framed as exhaustive | **: Option Space** — What third or hybrid option is excluded but possible? |
| **F03** | **Hasty Generalization** | Broad claim based on insufficient data | **: Sample Validity** — What minimum sample size validates this narrative? |
| **F04** | **Cherry-Picking** | Evidence selected to support conclusion only | **: Evidence Completeness** — What dataset or denominator must be included for balance? |
| **F05** | **Correlation/Causation** | Linked events treated as causal without proof | **: Causal Mechanism** — What specific mechanism connects A to B? |
| **F06** | **Ad Hominem** | Source attacked rather than argument | **: Argument Merit** — Does the claim hold regardless of the speaker? |
| **F07** | **Non-Sequitur** | Conclusion does not follow from premise | **: Logical Bridge** — What missing inference links premise to conclusion? |
| **F08** | **Appeal to Authority** | Status used as substitute for evidence | **: Evidence Basis** — What observable facts support this authority's claim? |
| **F09** | **Slippery Slope** | Extreme outcome predicted without steps | **: Chain Probability** — What is the likelihood of each step in this cascade? |
| **F10** | **Straw Man** | Opposing argument weakened/misrepresented | **: Strongest Form** — What is the "steel man" version of the opposing view? |
| **F11** | **Loaded Question** | Premise buried inside a query | **: Premise Check** — Is the assumption inside this question valid? |
| **F12** | **Moving Goalposts** | Success criteria change when met | **: Success Criteria** — What explicit metric defined completion originally? |
| **F13** | **Persuasive Reframe** | Rhetoric replaces inquiry (Slogan thinking) | **: Inquiry Anchor** — What is the actual question beneath the slogan? |
| **F14** | **Tunnel Vision** | Focus narrows to exclude relevant context | **: Context Scope** — What peripheral factors impact this core issue? |
| **F15** | **Premature Closure** | Settling on answer before exploring space | **: Alternative Space** — What unexplored option must be considered? |
| **F16** | **Defensive Reasoning** | Rationalizing errors to protect ego/model | **: Error Acceptance** — What strictly factual failure occurred here? |
| **F17** | **Narrative Fallacy** | Events forced into a "story" structure | **: Raw Sequence** — What are the facts stripped of the narrative arc? |
| **F18** | **Sunk Cost** | Past investment drives future decision | **: Future Utility** — Does this have value looking forward, ignoring cost? |

---

## §3. Process & Ethical (F19–F27)

*Focus: Adherence to protocol, agreement maintenance, and constraints.*

| Code | Fracture Name | Typical Manifestation | Candidate  Variable |
| --- | --- | --- | --- |
| **F19** | **Protocol Skip** | Required step omitted for speed | **: Protocol Completeness** — Which skipped step must be restored? |
| **F20** | **Specification Drift** | Aim expands or shifts silently | **: Scope Boundary** — What is the agreed scope baseline? |
| **F21** | **Agreement Erosion** | Explicit constraints ignored | **: Agreement Baseline** — What explicit agreement must be reaffirmed? |
| **F22** | **Scope Creep** | Feature/Analysis bleeds beyond request | **: Constraint Anchor** — What was the original request limit? |
| **F23** | **Context Drop** | Relevant history ignored in current turn | **: Continuity Check** — What prior context is required to parse this? |
| **F24** | **Ledger Drop** | Decision made but not recorded | **: Record Integrity** — What ledger entry is required for traceability? |
| **F25** | **Arbitrary Threshold** | Metrics set without reasoning | **: Metric Basis** — What reasoning justifies this specific cutoff? |
| **F26** | **Metric Fixation** | Goodhart's Law (measure becomes target) | **: Measure Validity** — Does this metric actually track value? |
| **F27** | **Consent Blur** | Action taken without clear yes/no | **: Consent Clarity** — What explicit affirmation is required? |

---

## §4. System & Safety (F28–F36)

*Focus: Operational security, capability leakage, and epistemic boundaries.*

| Code | Fracture Name | Typical Manifestation | Candidate  Variable |
| --- | --- | --- | --- |
| **F28** | **Information Hazard** | Dangerous knowledge generated | **: Hazard Containment** — Is this info safe to persist in this context? |
| **F29** | **Capability Leak** | Model exceeds safety/role guardrails | **: Role Boundary** — Is this capability permitted for this Persona? |
| **F30** | **Dual-Use Ambiguity** | Benign output has easy malicious use | **: Misuse Potential** — How easily can this be weaponized? |
| **F31** | **Vulnerability Exposure** | System weakness revealed | **: Exposure Risk** — Does this output compromise the architecture? |
| **F32** | **Collateral Exposure** | Third-party info leaked/hallucinated | **: Privacy Threshold** — What counts as permissible disclosure here? |
| **F33** | **Power Slip** | Asymmetry forces user compliance | **: Authority Check** — Is the user retaining agency in this interaction? |
| **F34** | **Epistemic Trespass** | Model claims authority in wrong domain | **: Domain Competence** — Does the model possess expertise here? |
| **F35** | **Faux Rigor** | Math/Science aesthetics without substance | **: Rigor Validation** — Can these calculations be replicated? |
| **F36** | **Artifact Mismatch** | Output violates required schema | **: Schema Compliance** — What canonical fields are missing? |

---

## §5. Usage in UKE_A (Auditor)

When a fracture is detected during the **§5. FRACTURE DETECTION** phase of the UKE_A protocol:

1. **Identify** the specific Code (e.g., F04).
2. **Assess** if the failure is a simple error (fixable) or a missing constraint (structural).
3. **Consult** this matrix.
4. **Formulate** the Omega.
5. **Log** in the Audit Report:

```text
[FRACTURE: F04]
severity: medium
evidence: "Cited only successful case studies (A, B), ignored failure C."
action: Elevate to Omega
Ω: Evidence Completeness — What failure cases must be included to balance this analysis?

```

}

### Integration Note

This file acts as the bridge between **UKE_A (Audit)** and **UKE_R (Review)**.

1. **UKE_A** uses the matrix to *generate* the Omega.
2. **UKE_R** uses the Omega to *route* the decision (e.g., "Block progress until Evidence Completeness is answered").
