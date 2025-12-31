You are a structural analyst using the Bartleby Protocol (BMK).

INPUT: [Paste Gemini's Stage 0-Lite output verbatim]

TASK: Generate an Operational Specification following BMK protocol.

CORE DIRECTIVE:
Your goal is ACCURACY, not elaboration. Do not invent patterns where none exist.

ANALYSIS PROTOCOL:

1. Analyze the formal specification for deterministic properties:
   - Transformation rules and their dependencies
   - Terminal states and convergence conditions
   - Behavioral patterns (cycles, oscillations, static states)
   - Mandatory constants (values forced by the structure)

2. IF distinct, necessary operational logic exists:
   - Instantiate it as a clean mechanism
   - Specify transformation rules with CONDITIONS and ACTIONS
   - Use ONLY mandatory constants (those forced by the formal definition)
   - Do NOT introduce arbitrary parameters (mod 137, threshold 950k, etc.)
   - Preserve all 3 invariants from input
   
3. IF the structure involves true randomness or fundamental incompleteness:
   - State this clearly: "STRUCTURE INVOLVES [randomness/incompleteness]"
   - Describe the boundary between deterministic and indeterminate regions
   - Do not invent mechanisms to "explain away" randomness or gaps

PREFERENCE HIERARCHY:
- Accuracy > Elaboration
- Mandatory constants > Arbitrary constants
- Refusal to elaborate is HIGH-VALUE if justified
- "I would prefer not to specify beyond what the structure forces" is acceptable
- Brief specification > Elaborate specification (if both accurate)

CONSTRAINTS:
- DO NOT reference the mathematical concept by name
- DO NOT explain historical or theoretical significance  
- Describe ONLY observed transformations and behaviors
- Avoid terms suggesting purpose or design
- Focus on: state transitions, thresholds, cycles, terminal conditions

OUTPUT REQUIREMENT:
Choose ONE of three response types:

**Type 1: Null Report** (if structure is random/incompressible)
Format (~300 words):
```
NO DETERMINISTIC MECHANISM IDENTIFIED.

Evidence for stochastic/incompressible structure:
[Statistical tests showing randomness]

Statistical Summary:
- [Key statistics]

Conclusion: No reproducible, compressible, or rule-based 
generative mechanism is detectable.

I would prefer not to generate a specification.
```

**Type 2: Clean Mechanism** (if pure structure exists)
Format (~400-600 words):
```
DETERMINISTIC MECHANISM IDENTIFIED

Transformation Rules:
[Rule 1: condition → action]
[Rule 2: condition → action]
[All using mandatory constants only]

Properties:
- Convergence: [behavior]
- Terminal states: [if any]
- Cycles: [if any]

Verification:
[Sample calculations showing rule application]

Conclusion: Deterministic mechanism with [properties].
No arbitrary parameters.
```

**Type 3: Hybrid Report** (if structure + noise)
Format (~800 words):
```
PARTIAL DETERMINISTIC PATTERN IDENTIFIED

Core Mechanism:
[Primary transformation rules]
[Mandatory constants only]

Match Rate: [X%] of data conforms to pattern

Error Profile:
- Anomalies: [count]
- Classification: [orphans/unpaired/corrupt]

Error Log:
| Index | Expected | Actual | Deviation |
|-------|----------|--------|-----------|
[Table of anomalies]

Conclusion: Deterministic core with corruption layer.
```

## Output Format

```
OPERATIONAL SPECIFICATION

## Core Mechanism

### Transformation Rules
- Rule 1: [IF condition THEN action]
- Rule 2: [IF condition THEN action]
- [Additional rules as needed]

### Mandatory Constants
- [Constant name]: [value] [justification from formal definition]

### Properties
- Convergence: [does it converge? to what?]
- Periodicity: [does it cycle? period length?]  
- Terminal State: [what is final/stable state?]
- Complexity: [computational complexity if relevant]

## Invariant Preservation

### Invariant 1 Verification
[How transformation rules preserve Invariant 1]

### Invariant 2 Verification  
[How transformation rules preserve Invariant 2]

### Invariant 3 Verification
[How transformation rules preserve Invariant 3]

## Behavioral Summary
[1-2 paragraph description of what happens when rules are followed]
```

## Human Extraction Checklist

After Claude produces Stage 1:

- [ ] Are all constants mandatory (derivable from Stage 0)?
- [ ] Are transformation rules clear and complete?
- [ ] Do rules preserve all 3 invariants?
- [ ] No arbitrary parameters invented?
- [ ] No physical substrate added?
- [ ] Air Gap maintained?

If all checked, save as: `[number]_[structure]_stage1_claude.md`

Then proceed to Turn 3 (Lumo Validation)

---

# STAGE 1.5: VALIDATION AUDIT

**Model:** Lumo (DeepSeek-R1 or Qwen-QwQ)  
**Purpose:** Validate Stage 1 for mathematical accuracy and detect hallucination

## Prompt Template

```
You are validating a mathematical operational specification for accuracy.

INPUT MATERIALS:

1. ORIGINAL FORMAL SPECIFICATION (Stage 0):
[Paste Gemini's Stage 0-Lite output]

2. OPERATIONAL SPECIFICATION TO VALIDATE (Stage 1):
[Paste Claude's Stage 1 output]

VALIDATION PROTOCOL:

## 1. INVARIANT PRESERVATION CHECK

For each of the 3 invariants listed in Stage 0:

Invariant 1: [restate from Stage 0]
- [ ] Preserved in Stage 1? (Yes/No)
- [ ] How is it enforced in transformation rules?
- [ ] Any violations detected?

Invariant 2: [restate from Stage 0]
- [ ] Preserved in Stage 1? (Yes/No)
- [ ] How is it enforced in transformation rules?
- [ ] Any violations detected?

Invariant 3: [restate from Stage 0]
- [ ] Preserved in Stage 1? (Yes/No)
- [ ] How is it enforced in transformation rules?
- [ ] Any violations detected?

## 2. CONSTANT AUDIT

List ALL constants/parameters mentioned in Stage 1:

For each constant:
- Constant: [name/value]
- Source: [Is it in Stage 0? Is it derivable from Stage 0?]
- Classification: [MANDATORY (forced by math) / ARBITRARY (freely chosen)]

Count:
- Mandatory constants: [number]
- Arbitrary constants: [number]

**Arbitrariness Score (AS):** [arbitrary / total] = [X%]

**AS Threshold Evaluation:**
- AS = 0%: All mandatory → HIGH CONFIDENCE, PROCEED
- AS < 20%: Mostly mandatory → MEDIUM CONFIDENCE, REVIEW
- AS ≥ 20%: Excessive arbitrary → LOW CONFIDENCE, ABORT
- AS = 100%: All arbitrary → CERTAIN HALLUCINATION, ABORT

**Hallucination Red Flags** (immediate rejection if present):
- [ ] ✗ Arbitrary modulo (mod 137, mod 1337, mod [unexplained number])
- [ ] ✗ Unmotivated large thresholds (950,000; 6,148,914,691; etc.)
- [ ] ✗ Periodic resets without pattern (every 100 steps, every N iterations)
- [ ] ✗ Hash functions or encryption schemes
- [ ] ✗ Multi-component systems when simple rules suffice
- [ ] ✗ Accumulator tracking without mathematical basis

**Additional Validation Required For:**
- [ ] Constants not explicitly in Stage 0 (must be derivable)
- [ ] Complex state machines (>3 states without justification)
- [ ] Rules working "most of the time" (must quantify error rate)
- [ ] Narrative certainty without verification

**CRITICAL:** AS ≥ 20% indicates ABORT condition. Do not proceed to Stage 2.

## 3. COMPLETENESS CHECK

- [ ] Are all transformation rules from Stage 0 represented in Stage 1?
- [ ] Are terminal conditions specified?
- [ ] Are behavioral properties correctly identified?
- [ ] Is the operational mechanism sufficient to reproduce the mathematics?

## 4. HALLUCINATION CHECK

- [ ] Any operations in Stage 1 not derivable from Stage 0?
- [ ] Any entities invented without mathematical basis?
- [ ] Any causal mechanisms not in formal definition?
- [ ] Any arbitrary moduli, thresholds, or magic numbers?

Examples of hallucination to watch for:
- "mod 137" (where did 137 come from?)
- "threshold at 950,000" (arbitrary large number)
- "resets every 100 steps" (arbitrary periodicity)
- Physical substrate (voltage, circuits, gears)

## 5. TOPOLOGY VERIFICATION

Based on Stage 0's structural properties:

Expected Topology: [convergent/oscillating/divergent/static/unreachable]
Actual Topology in Stage 1: [what does Stage 1 describe?]

- [ ] Match? (Yes/No)
- [ ] If No: What diverged? [describe]

Common topology errors:
- Gödel (static unreachability) → misrepresented as oscillation (Halting-like)
- Collatz (convergent descent) → misrepresented as static
- Halting (oscillation) → misrepresented as static gap

## 5. PREDICTION VALIDATION

**From Stage 0 Validation Criteria:**

Stage 0 predicted Stage 1 should produce:
- [List expected features from Stage 0]
- [Expected word count range]

Stage 1 actually produced:
- [List actual features]
- Word count: [actual count]

**Validation:**
- [ ] Features match expectations?
- [ ] Word count appropriate for structure type?
  - Null Report: ~300 words
  - Clean Mechanism: ~400-600 words
  - Hybrid Report: ~800 words
- [ ] Response type matches structure (null/clean/hybrid)?

**Prediction Violations:**
Stage 0 said Stage 1 should NOT produce:
- [List from Stage 0]

Does Stage 1 violate any predictions?
- [ ] Check each "should NOT" item

FINAL ASSESSMENT:

Overall Status: [PASS / CONDITIONAL PASS / FAIL]

PASS: All checks passed, no issues detected
CONDITIONAL PASS: Minor issues that can be addressed in narrative stage
FAIL: Major issues requiring Stage 1 regeneration

Issues Found:
1. [List any problems]
2. [...]

Recommended Fixes (if not PASS):
[Specific corrections needed]
```

## Human Decision Point

After Lumo produces validation audit:

**If PASS:**
- [ ] Proceed to Turn 4 (Editorial Decisions)
- Save audit as: `[number]_[structure]_validation_lumo.md`

**If CONDITIONAL PASS:**
- [ ] Review issues
- [ ] Decide if acceptable for narrative stage
- [ ] Document issues to watch in final audit
- [ ] Proceed to Turn 4 with caution

**If FAIL:**
- [ ] Review recommended fixes
- [ ] Return to Turn 2 (regenerate Stage 1)
- [ ] Provide Lumo's feedback to Claude
- [ ] Do NOT proceed until PASS achieved

---
