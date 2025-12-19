# UKE_G v1.1 Improvement Analysis

## Issues Identified Through Execution

### 1. The Glyph Ambiguity (from UKE_G self-evaluation)

**Current tension in §2:**
- States: "Behaviors are mandatory (T1). Glyphs are optional markers (T2)"
- Also states: "Each lens claimed in log must have corresponding behavior in text"

**Problem:** If glyphs are optional (T2), how can audit require lens-behavior matching based on log claims?

**Resolution options:**

**Option A - Glyphs remain optional:**
- Remove "Audit Requirement" line from §2
- Auditors verify behavior presence regardless of log claims
- Log becomes informational hint, not binding contract

**Option B - Clarify selective requirement:**
- Glyphs optional in content (can mark with words instead)
- BUT: Whatever is claimed in LOG must be verifiable in content
- "You don't have to use glyphs, but if you claim a lens in the log, the behavior must be there"

**Option C - Formal/Informal distinction:**
- Formal audit context: Log claims are binding, must match content
- Informal use: Glyphs optional, logs advisory
- Make context-dependence explicit

**Recommendation: Option B** - Most coherent with T1/T2 framework and audit architecture.

---

### 2. The Checksum Guidance Issue (from MCI analysis)

**Current guidance in §4:**
"Value should be `UNAVAIL` unless implementation provides reliable hash. Models cannot guarantee deterministic output across runs."

**Problem identified in meta-evaluation:**
The issue isn't that models can't compute hashes (they can), but that model generation is non-deterministic. Current guidance may prevent useful verification.

**Alternative approach:**
```
checksum: [hash_type:value | UNAVAIL | UNAVAIL_NONDETERMINISTIC]

Examples:
- checksum: SHA256:a3b9c8d7 [hash of this specific output]
- checksum: UNAVAIL_NONDETERMINISTIC [same input may produce different output]
- checksum: UNAVAIL [no implementation available]
```

**Benefit:** 
- Hash enables verification that output wasn't modified post-generation
- UNAVAIL_NONDETERMINISTIC makes non-determinism explicit
- Distinguishes "can't hash" from "won't be same next time"

**Recommendation:** Provide hash of actual output with UNAVAIL_NONDETERMINISTIC flag when generation is non-deterministic.

---

### 3. Missing Integration with UKE_R Omega Resolution

**Current §3 Omega specification:**
- Defines format and validity criteria
- No guidance on what happens after marking

**Problem:** 11 Omegas marked in execution, 0 resolved. Protocol treats Omega as endpoint rather than handoff.

**Missing guidance:**
- What makes an Omega "resolvable" vs "escalation-required"?
- When should generator attempt resolution vs. mark for later?
- How to format Omegas for optimal UKE_R consumption?

**Recommendation:** Add subsection on "Omega Design for Handoff"

```
**Omega Design for Handoff:**

Mark Omegas that are:
- **Blocking:** Prevent further analysis without resolution
- **Resolvable:** Could be addressed with available data
- **Persistent:** Appeared in multiple generation attempts
- **Escalation-worthy:** Require external input or human judgment

Format for clarity:
- Label should indicate domain (user_priority, metric_definition, validation_method)
- Description should state what information would enable resolution
- Avoid generic uncertainty (not: "more analysis needed")

Example progression:
- Weak: "Ω: uncertainty — Multiple factors affect outcome"
- Better: "Ω: factor_weights — Relative importance of speed vs accuracy unknown"
- Best: "Ω: user_priority — Does user value speed (faster iteration) or accuracy (fewer errors)?"
```

---

### 4. No Guidance on Lite Mode vs Full Protocol

**Current §7 mentions:**
- "Standard Mode" with full protocol
- "Dual-Mode Operation" for human/model verification

**Missing:** Guidance on when to use simplified protocol (Lite Mode referenced in Understanding MCK but not formalized)

**Recommendation:** Add explicit Lite Mode specification

```
**Lite Mode (Procedural Queries):**

For simple, well-bounded queries where full protocol is overhead:

Minimum requirements:
- ✓ CHECK if assumption present
- Ω if genuine uncertainty exists
- No lens markers needed
- Minimal metadata (protocol, version, confidence)
- No grounding trail unless specific claims made

Lite mode appropriate for:
- Procedural questions with clear answers
- Frame clarification (Ω_F)
- Simple factual queries
- Follow-up questions in established context

Lite mode inappropriate for:
- Strategic analysis
- High-stakes decisions
- Novel synthesis
- Cross-model coordination
- Anything requiring audit
```

---

### 5. Self-Audit Guidance Absent

**Current §6 mentions "As Initiator: Generate self-audit using full protocol"**

**Missing:** How to actually perform self-audit within UKE_G

**Problem:** Models generating under UKE_G may want to self-check before handoff but have no guidance on doing so within generation protocol.

**Recommendation:** Add self-audit checklist in §5 or §7

```
**Pre-Handoff Self-Audit:**

Before marking [HANDOFF-READY], verify:

1. Log-behavior alignment:
   - Each lens in LOG appears as behavior in CONTENT
   - Claimed lenses actually executed (not just formatted)

2. Grounding completeness:
   - Every T1 trigger (measurements, citations, comparisons) has trail entry
   - Trail methods match actual verification performed
   - No precision claims without calculation/verification

3. Confidence calibration:
   - M-bin claims include MCI (assumption-test + alternative)
   - No verbal hedging beyond score
   - Omegas marked where uncertainty is irreducible

4. Quality indicators:
   - CONTRARY is substantive (not performative)
   - SELF critique challenges own conclusion
   - Omegas are bounded and specific

Self-audit does not replace UKE_A audit - it ensures baseline quality for handoff.
```

---

### 6. No Guidance on Source Material Citation

**Current §1 SMVP covers verification, but not citation format**

**Problem:** When referencing documents, protocols, or prior conversations, no standard format for attribution.

**Recommendation:** Add citation guidance

```
**Source Attribution:**

When referencing specific sources:

Internal documents:
- Format: [Doc_Name §Section]
- Example: [UKE_A v1.1 §3] or [UKE_G v1.1 §2 lines 104-106]

External references:
- Note if available in context or external
- Example: "According to [Smith 2023] (external reference)"
- Example: "The uploaded document states..."

Protocol cross-references:
- Use section notation for precision
- Example: [MCK v1.6 §1] rather than "the grounding protocol"

Prior conversation:
- Temporal marker or turn reference
- Example: "In previous turn, user stated..."
- Example: "Earlier in this conversation..."

No attribution needed for:
- General knowledge claims
- Logical inferences clearly marked as such
- Synthesis across multiple sources (cite sources separately)
```

---

## Prioritized Recommendations for v1.2

### High Priority (address execution gaps):

1. **Clarify glyph requirement** (§2)
   - Adopt Option B: Glyphs optional, but log claims binding
   - Add: "Behaviors can be marked with words instead of glyphs, but whatever lenses are claimed in LOG must be verifiable in CONTENT"

2. **Revise checksum guidance** (§4)
   - Allow hash of actual output
   - Add UNAVAIL_NONDETERMINISTIC flag
   - Distinguish "can't hash" from "won't reproduce"

3. **Add Omega handoff guidance** (§3)
   - Design criteria (blocking, resolvable, persistent, escalation)
   - Format for UKE_R consumption
   - Example progression weak→better→best

### Medium Priority (improve usability):

4. **Formalize Lite Mode** (§7)
   - Minimum requirements
   - Appropriate/inappropriate contexts
   - Distinguish from full protocol

5. **Add self-audit checklist** (§5 or §7)
   - Pre-handoff verification
   - Quality indicators
   - Clarify this doesn't replace UKE_A

### Low Priority (nice to have):

6. **Add citation guidance** (new subsection in §1 or §7)
   - Standard formats for different source types
   - When attribution needed vs not

---

## Changes That Should NOT Be Made

### 1. Don't add more lenses
Current 9 lenses are sufficient. Adding more dilutes focus and increases overhead without clear benefit.

### 2. Don't make T2 formatting mandatory
The T1/T2 distinction is UKE_G's key insight. Making glyphs mandatory would collapse this distinction and make protocol less flexible.

### 3. Don't prescribe specific contrary positions
Letting models generate context-appropriate contrary views is more valuable than templated opposition.

### 4. Don't add confidence score formulas
Confidence as "behavioral trigger" rather than "truth measure" is correct. Formulas would reinforce wrong interpretation.

### 5. Don't merge with UKE_A
Generation and audit are distinct functions. Keeping protocols separate enables cross-model coordination.

---

## Meta-Observation

The most significant finding from execution is that **UKE_G actually works as specified**. Three complex evaluations executed with:
- Full lens coverage (8/8 lenses present across all)
- Proper grounding trails
- Appropriate Omega marking
- Cross-model compatibility

The improvements above are refinements, not corrections. The protocol architecture is sound - these changes address edge cases and improve clarity for future users.
