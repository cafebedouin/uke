You are conducting a comprehensive fidelity audit on a mathematical narrative.

INPUT MATERIALS:

1. STAGE 0 (FORMAL SPECIFICATION):
[attached]

2. STAGE 1 (OPERATIONAL SPECIFICATION):
[attached]

3. EDITORIAL DECISIONS:
[attached]

4. FINAL NARRATIVE:
[attached]

---

## AUDIT PROTOCOL

### 1. INVARIANT PRESERVATION AUDIT

For each of the 3 invariants from Stage 0:

**Invariant 1:** [restate from Stage 0]

- [ ] Is it enforced in story logic?
- [ ] Can reader intuit it without explanation?
- [ ] Would violating it break the narrative?
- **Stress Test:** Write one sentence that would violate this invariant.
  [Sentence: "..."]
  Does it feel narratively wrong? [Yes/No]

**Invariant 2:** [restate from Stage 0]

- [ ] Is it enforced in story logic?
- [ ] Can reader intuit it without explanation?
- [ ] Would violating it break the narrative?
- **Stress Test:** [sentence + evaluation]

**Invariant 3:** [restate from Stage 0]

- [ ] Is it enforced in story logic?
- [ ] Can reader intuit it without explanation?
- [ ] Would violating it break the narrative?
- **Stress Test:** [sentence + evaluation]

**Invariant Score:** [X/3 preserved]

---

### 2. TOPOLOGY VERIFICATION AUDIT

**Expected Topology** (from Stage 0 structural properties):
- Temporal Structure: [convergent/oscillating/divergent/static/unreachable]
- Key Behavior: [what should happen mathematically]

**Actual Topology** (from narrative):
- What happens in the story? [describe arc]
- Pattern: [convergent/oscillating/divergent/static/unreachable]

**Match Assessment:**
- [ ] MATCH: Topology preserved
- [ ] PARTIAL: Close but some divergence
- [ ] MISMATCH: Different topology

If PARTIAL or MISMATCH:
- What diverged? [specific differences]
- Is divergence justified by narrative constraints? [explain]
- Does it betray mathematical truth? [Yes/No]

**Topology Score:** [MATCH/PARTIAL/MISMATCH]

---

### 3. CONSTANT & RESIDUE AUDIT

**Math Residue Budget:** ≤3 numbers, ≤2 operations

Count in narrative:
- Explicit numbers: [list them] → Total: [X/3]
- Named operations: [list them] → Total: [X/2]

**Budget Status:** [PASS/FAIL]

**Constant Verification:**
For each number/operation in narrative:
1. [Number/Operation]: Source in Stage 0? [Yes/No/Derived]

**Hallucination Check:**
- [ ] Any numbers not in Stage 0 or derivable from it?
- [ ] Any operations not in Stage 1?
- [ ] Any arbitrary constants smuggled in?

**Residue Score:** [PASS/FAIL]

---

### 4. STRUCTURAL FIDELITY AUDIT

**Operations Mapping:**
For each transformation rule in Stage 1:
1. [Rule from Stage 1] → [How it appears in narrative]

**Completeness:**
- [ ] All key operations from Stage 1 present in narrative?
- [ ] Are operations recognizable (even if metaphorical)?

**Causal Fidelity:**
- [ ] Any causal powers invented without mathematical basis?
- [ ] Does protagonist have choice where math allows none?
- [ ] Are outcomes determined by math or by narrative convenience?

**Fidelity Score:** [HIGH/MEDIUM/LOW]

---

### 5. EMOTIONAL TRUTH AUDIT

**From Editorial Decisions:**
- Primary Emotion: [restate]
- Anti-Emotions: [restate]

**In Narrative:**
- Is primary emotion present throughout? [Yes/No]
- Are anti-emotions avoided? [Yes/No]
- Does emotion emerge NATURALLY from mathematical structure? [Yes/No]
- Or is emotion IMPOSED on math? [Yes/No]

**Examples:**
- Scene that serves primary emotion well: [quote/cite]
- Scene that might violate anti-emotion: [quote/cite if any]

**Emotional Score:** [NATURAL/FORCED]

---

### 6. VOICE CONSISTENCY AUDIT

**Selected Voice:** [from editorial decisions]

**Voice Markers to Check:**
[List 4-5 key markers from voice definition]

**In Narrative:**
For each marker:
- [ ] Marker 1: Present/Absent
- [ ] Marker 2: Present/Absent
- [ ] Marker 3: Present/Absent
- [ ] Marker 4: Present/Absent

**Drift Detection:**
- Does voice remain stable throughout? [Yes/No]
- Any sections where voice breaks? [cite if any]
- Does voice match knowledge boundary? [Yes/No]

**Voice Score:** [CONSISTENT/MINOR DRIFT/MAJOR DRIFT]

---

### 7. GATE COMPLIANCE AUDIT

**Gate 1 (Math Residue):** [PASS/FAIL]
**Gate 2 (Protagonist Viability):** [PASS/FAIL]
**Gate 3 (Emotional Core):** [PASS/FAIL]
**Gate 4 (Invariants):** [X/3 enforced]
**Gate 5 (Cadence):** [PASS/FAIL]

**Overall Gate Compliance:** [X/5 passed]

---

## FINAL ASSESSMENT

**FIDELITY SCORE SUMMARY:**

| Category | Score | Weight | Points |
|----------|-------|--------|--------|
| Invariant Preservation | X/3 | 25% | X/25 |
| Topology Match | MATCH/PARTIAL/MISMATCH | 20% | X/20 |
| Residue Budget | PASS/FAIL | 15% | X/15 |
| Structural Fidelity | HIGH/MED/LOW | 20% | X/20 |
| Emotional Truth | NATURAL/FORCED | 10% | X/10 |
| Voice Consistency | CONSISTENT/DRIFT | 10% | X/10 |

**TOTAL FIDELITY SCORE:** [X/100]

---

**FINAL DETERMINATION:**

- [ ] **PASS** (Score ≥ 85): High fidelity, ready for publication
- [ ] **CONDITIONAL PASS** (Score 70-84): Good but needs minor revision
- [ ] **FAIL** (Score < 70): Major issues, requires revision

---

**ISSUES FOUND:**

1. [List specific problems]
2. [...]

**RECOMMENDED REVISIONS:**

If not PASS:
1. [Specific fix needed]
2. [...]

**WHAT WAS PRESERVED:**
[The mathematical essence that survived - what reader grasps intuitively]

**WHAT WAS SACRIFICED:**
[Technical precision lost for narrative clarity - what mathematicians notice missing]

**WHY TRADE WAS NECESSARY:**
[Justification based on audience contract and emotional goals]

---

**AUDIT COMPLETE**
```

## Human Final Review

After Claude produces fidelity audit:

- [ ] Review fidelity score
- [ ] Read issues and recommendations
- [ ] Decide final status:
  - PASS → Story complete, ready for publication
  - CONDITIONAL → Make noted revisions
  - FAIL → Return to appropriate stage for regeneration

---
