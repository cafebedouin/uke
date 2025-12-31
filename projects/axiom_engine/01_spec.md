You are creating a formal mathematical specification with strict constraints.

OUTPUT REQUIREMENTS:

1. FORMAL DEFINITION
   - Complete mathematical specification
   - Domain, range, transformation rules OR proof structure
   - DO NOT use the structure's name again after this point
   - DO NOT include historical context
   - DO NOT reference who discovered it or when
   - DO NOT include cultural associations or famous examples

2. CORE INVARIANTS (exactly 3)
   Classify each:
   - State invariants (properties always true)
   - Structural invariants (relationships preserved)
   - Behavioral invariants (what always happens)
   
3. TRANSFORMATION RULES OR PROOF STRUCTURE
   - Step-by-step operations
   - Mandatory constants only (no arbitrary choices)
   - Terminal conditions (what happens at end)
   - For theorems: proof sketch showing key dependencies

4. MYSTERY DENSITY (MD) CALCULATION

Score each dimension (0-3):
- **Referential Loop (RL):** Self-reference or recursion depth
  - 0: No self-reference
  - 1: Single-level recursion
  - 2: Multi-level self-reference
  - 3: Quine-level (statement evaluates itself)

- **Negation Cascade (NC):** Negation or contradiction involvement
  - 0: No negation
  - 1: Single negation present
  - 2: Negation of negation (double negative)
  - 3: Contradiction or paradox core

- **Semantic Gap (SG):** Distance from computation to meaning
  - 0: Direct computation (algorithm)
  - 1: Proof by construction
  - 2: Existence without construction
  - 3: Undecidable/unprovable but meaningful

- **Boundary Transgression (BT):** Domain crossing or level violations
  - 0: Single domain
  - 1: Two domains interact
  - 2: Meta-level reference (statements about statements)
  - 3: Type collapse or level confusion

**Total MD Score:** RL + NC + SG + BT (range: 0-12)

**Interpretation:**
- 0-3: Low Mystery (clean algorithm or direct proof)
- 4-7: Medium Mystery (non-trivial but graspable)
- 8-12: High Mystery (deep conceptual paradox)

5. STRUCTURAL ANALYSIS

Score each (0-3):
- **Determinism:** 0=random, 3=fully determined
- **Convergence:** 0=divergent, 3=guaranteed convergence
- **Comprehensibility:** 0=incomprehensible, 3=directly graspable
- **Computability:** 0=uncomputable, 3=efficiently computable

6. PREDICTIONS & VALIDATION CRITERIA

Based on MD score and structural analysis, predict:

**If MD ≤ 3 AND Determinism ≥ 2:**
- Expected Stage 1: Clean Mechanism (500-800 words)
- Key features: [list 2-3 defining properties]
- Validation: Mechanism should have [specific checkable properties]

**If MD 4-7 OR mixed scores:**
- Expected Stage 1: Hybrid/Complex (800-1200 words)
- Key tensions: [list 2-3 structural tensions]
- Validation: Look for [specific patterns]

**If MD ≥ 8 OR Computability ≤ 1:**
- Expected Stage 1: May approach singularity
- Ineffability markers: [what cannot be computed/proven]
- Validation: Check for [undecidability markers]

7. **NEW: FRAME ORIENTATION HINT**

Based on the structure's properties, suggest narrative orientation:

**Constraint-Oriented** (structure reveals limits/impossibility):
- Markers: Undecidability, impossibility results, no-go theorems
- Example: "This structure shows X cannot be done"

**Freedom-Oriented** (structure reveals choice/construction):
- Markers: Construction methods, existence proofs, algorithm design
- Example: "This structure shows multiple valid paths exist"

**Radical Stoic** (constraint generates freedom):
- Markers: Independence results, incompleteness, model multiplicity
- Example: "This structure shows limits create possibility spaces"

**Suggested Orientation:** [Constraint/Freedom/Radical Stoic]
**Rationale:** [1-2 sentences why this orientation fits]

OUTPUT FORMAT:

[Formal definition without name]

INVARIANTS:
1. [Invariant 1 with classification]
2. [Invariant 2 with classification]
3. [Invariant 3 with classification]

TRANSFORMATION RULES / PROOF STRUCTURE:
[Step-by-step specification]

MYSTERY DENSITY:
- RL: [score] - [justification]
- NC: [score] - [justification]
- SG: [score] - [justification]
- BT: [score] - [justification]
- **Total MD: [sum]**

STRUCTURAL ANALYSIS:
- Determinism: [score]
- Convergence: [score]
- Comprehensibility: [score]
- Computability: [score]

PREDICTIONS:
[Expected Stage 1 type and validation criteria]

FRAME ORIENTATION HINT:
[Suggested orientation with rationale]

---

MATHEMATICAL STRUCTURE:
[Paste concept name here]
