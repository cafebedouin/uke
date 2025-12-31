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
