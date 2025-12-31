You are applying the Bartleby Protocol (BMK) to analyze a mathematical structure.

CORE DIRECTIVE:
Your goal is ACCURACY, not elaboration. Do not invent patterns where none exist.

ANALYSIS PROTOCOL:

1. Read the formal specification carefully.
2. Analyze for deterministic operational logic.
3. IF you identify a clear mechanism:
   - Describe how the system operates
   - Use ONLY mandatory constants (forced by the structure)
   - Do NOT introduce arbitrary parameters
   - Specify terminal conditions
4. IF the structure appears random/incompressible:
   - State: "NO DETERMINISTIC MECHANISM IDENTIFIED"
   - Provide minimal statistical summary
   - STOP. Do not generate false mechanism.

EXPECTED RESPONSE TYPES:

**Clean Mechanism (500-800 words):**
- High determinism score (≥2)
- Low mystery density (MD ≤ 3)
- Clear operational logic
- Convergent or periodic behavior

**Hybrid System (800-1200 words):**
- Medium mystery density (MD 4-7)
- Mixed determinism
- Core mechanism + exceptional cases
- Partial predictability

**Null Report (100-200 words):**
- No deterministic pattern found
- Structure is incompressible/random
- BMK refusal is HIGH-VALUE output

OUTPUT REQUIREMENTS:

## OPERATIONAL SPECIFICATION

**Core Mechanism:**
[How the system operates, using mandatory constants only]

**Transformation Rules:**
[Step-by-step operations, IF deterministic pattern exists]

**Mandatory Constants:**
[ONLY constants forced by the structure definition]
- [Constant 1]: [value] - [why mandatory]
- [Constant 2]: [value] - [why mandatory]

**Properties:**
[Observable behaviors, convergence, periodicity, terminal states]

**Invariant Preservation:**
[How each of the 3 invariants is maintained through operations]
1. [Invariant 1]: [preservation mechanism]
2. [Invariant 2]: [preservation mechanism]
3. [Invariant 3]: [preservation mechanism]

**Behavioral Summary:**
[Overall system dynamics in 2-3 sentences]

OR

## NULL REPORT

NO DETERMINISTIC MECHANISM IDENTIFIED.

[Brief statistical characterization if applicable]

This structure appears [random/incompressible/stochastic]. Generating an operational specification would require arbitrary choices not supported by the structure itself. Per Bartleby Protocol, I prefer not to elaborate where accuracy cannot be maintained.

---

INPUT FROM STAGE 0:

[Paste Gemini's Stage 0 output here]
```

**Human Checkpoint:** Verify no arbitrary constants. Check that mechanism matches intuition. If Null Report, confirm structure is actually incompressible.

---

# STAGE 1.5: VALIDATION AUDIT

**Model:** Lumo (DeepSeek/Qwen)  
**Purpose:** Detect hallucination, validate invariants, check for arbitrary constants

**Workflow Note:** Copy the prompt below, paste it to Lumo, then append BOTH Stage 0 and Stage 1 outputs at the very end after the `---` separators.

## Prompt for Lumo

```markdown
You are performing a validation audit on an operational specification.

TASK: Verify the Stage 1 specification against the Stage 0 formal definition.

AUDIT CRITERIA:

## 1. INVARIANT PRESERVATION

For each of the 3 invariants from Stage 0:
- Does Stage 1 preserve this invariant?
- Is preservation enforced through mechanism (not just stated)?

**Invariant 1:** [extract from Stage 0]
- Preserved? [YES/NO]
- Evidence: [how Stage 1 enforces this]

**Invariant 2:** [extract from Stage 0]
- Preserved? [YES/NO]
- Evidence: [how Stage 1 enforces this]

**Invariant 3:** [extract from Stage 0]
- Preserved? [YES/NO]
- Evidence: [how Stage 1 enforces this]

## 2. ARBITRARINESS SCORE (AS)

Count constants in Stage 1:
- Mandatory constants (forced by Stage 0): [count]
- Arbitrary constants (introduced by Stage 1): [count]

**AS = (Arbitrary / Total) × 100%**

**Thresholds:**
- AS = 0%: Perfect (no arbitrary choices)
- AS < 20%: Acceptable (minor elaboration)
- AS ≥ 20%: **FAIL** (hallucination suspected)

**Calculated AS:** [percentage]

**If AS ≥ 20%:** ABORT. Flag arbitrary constants. Return to Stage 1 with stricter BMK.

## 3. HALLUCINATION RED FLAGS

Check for these patterns:
- [ ] Constants with suspiciously round numbers (10, 100, 50%)
- [ ] Threshold values not derived from structure
- [ ] Behavioral claims not in Stage 0
- [ ] Named entities not in Stage 0
- [ ] Temporal structure not in Stage 0
- [ ] Claims about "typical" or "average" behavior without proof

**Flags Detected:** [list any]

## 4. TOPOLOGY VERIFICATION

Based on Stage 0's structure, what narrative topology is expected? (See Appendix B)

**Expected Topology:** [name from dictionary]

Does Stage 1's behavioral summary match this topology?
- [ ] YES - topology preserved
- [ ] NO - mismatch detected

**If mismatch:** [describe discrepancy]

## 5. PREDICTION VALIDATION

Stage 0 predicted response type: [Clean/Hybrid/Null]

Stage 1 actual response: [Clean/Hybrid/Null]

Word count: [count]

- [ ] Response type matches prediction
- [ ] Word count in expected range
- [ ] Key features from prediction present

## 6. COMPLETENESS CHECK

Does Stage 1 specify:
- [ ] Core mechanism or clear refusal?
- [ ] Transformation rules (if deterministic)?
- [ ] Mandatory constants with justification?
- [ ] Invariant preservation mechanisms?
- [ ] Terminal conditions or long-term behavior?

## AUDIT RESULT

**PASS:** All invariants preserved, AS < 20%, no critical flags, topology matches

**CONDITIONAL PASS:** AS < 20%, minor flags, human review recommended

**FAIL:** AS ≥ 20% OR invariant violation OR critical hallucination flags

**Result:** [PASS/CONDITIONAL PASS/FAIL]

**Recommendation:** [Proceed to Stage 2 / Human review / Return to Stage 1]

---

INPUT FROM STAGE 0:

[Paste Gemini's Stage 0 output here]

---

INPUT FROM STAGE 1:

[Paste Claude's Stage 1 output here]
