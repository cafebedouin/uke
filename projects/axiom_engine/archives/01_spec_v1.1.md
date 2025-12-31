You are creating a formal mathematical specification with strict constraints.

MATHEMATICAL STRUCTURE: [Name, e.g., "Gödel's Incompleteness Theorem"]

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

4. EPISTEMIC STATUS
   - Proven / Conjectured / Open
   - What is known vs. unknown
   - Key properties verified

5. STRUCTURAL PROPERTIES
   - Regularity: [Exact | Periodic | Chaotic | Random]
   - Computational Complexity: [O(?)]
   - Temporal Structure: [Convergent | Oscillating | Divergent | Static]

FORMAT:
Use clear markdown sections. Be rigorous. Avoid poetic language.

CRITICAL: Maintain "Air Gap" - do not reveal this structure's identity 
through cultural associations, famous quotes, or historical anecdotes.

Example opening (for reference, do not copy):
"Consider a formal system S with axioms A and inference rules R.
Construct statement G that encodes: 'This statement is not provable in S'..."
```

## Output Format

```
# FORMAL SPECIFICATION

## Domain & Definition
[Complete mathematical specification without naming the structure]

## Core Invariants

### Invariant 1: [Type: State/Structural/Behavioral]
[Statement of invariant]

### Invariant 2: [Type: State/Structural/Behavioral]  
[Statement of invariant]

### Invariant 3: [Type: State/Structural/Behavioral]
[Statement of invariant]

## Transformation Rules / Proof Structure
- Rule 1: [condition] → [action]
- Rule 2: [condition] → [action]
- Terminal Condition: [what happens at end]

## Epistemic Status
**Proof Status:** [Proven/Conjectured/Open] (Score: 0-3)
- 0 = Fully proven
- 1 = Mostly proven with minor gaps
- 2 = Conjectured with strong evidence
- 3 = Open question

- What is proven: [list]
- What is conjectured: [list]
- Open questions: [list if applicable]

## Structural Analysis

**Regularity:** [Exact/Periodic/Chaotic/Random] (Score: 0-3)
- 0 = Exact (deterministic, no variation)
- 1 = Periodic (cycles, predictable)
- 2 = Chaotic (deterministic but sensitive)
- 3 = Random (stochastic, no pattern)

**Computational Complexity:** [O(?)] (Score: 0-3)
- 0 = O(1) or O(log n)
- 1 = O(n) or O(n log n)
- 2 = O(n²) or O(2^n)
- 3 = Uncomputable or undecidable

**Enforcement Mechanism:** [Natural/Active/Vigilant] (Score: 0-3)
- Natural (0): Properties hold automatically
- Active (2): Requires verification at each step
- Vigilant (3): Must defend against violation

**Intuitive Distance:** [Direct/Expert/Alien] (Score: 0-3)
- Direct (0): Immediately graspable
- Expert (2): Requires training to understand
- Alien (3): Fundamentally counterintuitive

## Mystery Density Calculation

MD = 0.3×(Proof Status) + 0.2×(Regularity) + 0.1×(Complexity) 
   + 0.2×(Enforcement) + 0.2×(Intuition)

**Total MD:** [0.0-3.0]

**Interpretation:**
- MD 0.0-0.5: Very Low Mystery (simple, proven structures)
- MD 0.6-1.5: Low-Medium Mystery (standard complexity)
- MD 1.6-2.5: High Mystery (counterintuitive, open questions)
- MD 2.6-3.0: Extreme Mystery (alien, unprovable, incomprehensible)

## Predictions for Stage 1

**Expected Drama Level:** [0/1/2/3]
- 0 = Exactness (no variation, pure function)
- 1 = Maintenance (system holds pattern against drift)
- 2 = Emergence (pattern arises from interaction)
- 3 = Transformation (fundamental state change)

**Expected Metaphor Load:** [Very Low/Low/Medium/High/Very High]
- Very Low: Direct operations (arithmetic)
- Low: Simple physical analogues (motion)
- Medium: Abstract but familiar (games, journeys)
- High: Requires multiple metaphor layers
- Very High: Nearly impossible to express directly

**Expected Reconstruction Fidelity:** [%]
[Estimate: Can reader reconstruct the math from narrative?]

## Validation Criteria for Stage 1

**Stage 1 SHOULD Produce:**
- [Expected features based on structure]
- Word count: [~300 for null / ~400-600 for clean / ~800 for hybrid]
- [Specific transformation rules expected]

**Stage 1 should NOT Produce:**
- Arbitrary modulo operations (mod 137, mod 1337, etc.)
- Unmotivated large thresholds (950,000; 6,148,914,691)
- Periodic resets without mathematical basis
- Multi-component systems when simple rules suffice
- Constants not derivable from this specification
```

## Human Validation Checklist

After Gemini produces Stage 0-Lite:

- [ ] Are there exactly 3 invariants?
- [ ] Are invariants mathematically correct?
- [ ] Is Air Gap maintained? (structure name not mentioned again)
- [ ] Are transformation rules complete?
- [ ] Are all constants mandatory (none arbitrary)?
- [ ] Is formal definition sufficient for Stage 1?

---
