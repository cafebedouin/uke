# AXIOM ENGINE v2.2: PROTOCOL SPECIFICATION

**Version:** 2.2 (Production)  
**Status:** Validated  
**Date:** December 23, 2025  
**License:** CC BY-SA 4.0

---

## OVERVIEW

The Axiom Engine is a 7-stage protocol for analyzing mathematical structures through LLM transformation pipelines with enforced conceptual separation (Air Gaps) and refusal authorization (Bartleby Protocol).

**Core Innovation:** Inverts default LLM elaboration bias, enabling appropriate refusal when structure is absent while maintaining sensitivity to real patterns.

**Validated Capabilities:**
- Detects pure structure (Collatz: 100% constraint)
- Triages hybrid data (90% signal + 10% noise)
- Detects hidden patterns (pseudo-random with unconscious structure)
- Refuses appropriately (cryptographic randomness)

---

## STAGE 0: MYSTERY AUDIT

### Purpose
Generate formal mathematical specification without revealing conceptual identity.

### Template

```markdown
## MYSTERY AUDIT: [Internal Reference Only]

### Formal Definition
[Complete mathematical specification]
[Domain, range, transformation rules]

### Epistemic Status

**Proof Status:** [Proven/Conjectured/Open] (Score: 0-3)
- What is proven: [list]
- What is conjectured: [list]
- Open questions: [list]

**Known Properties:**
- [Verified characteristics]

**Conjectures:**
- [Unproven claims]

**Open Questions:**
- [Fundamental unknowns]

### Structural Analysis

**Regularity:** [Exact/Periodic/Chaotic/Random] (Score: 0-3)
**Computational Complexity:** [O(?)] (Score: 0-3)
**Enforcement Mechanism:** [Natural/Active/Vigilant] (Score: 0-3)
**Intuitive Distance:** [Direct/Expert/Alien] (Score: 0-3)

### Mystery Density Calculation

MD = 0.3×(Proof) + 0.2×(Opacity) + 0.1×(Complexity) 
   + 0.2×(Enforcement) + 0.2×(Intuition)

**Total MD:** [0-3]

### Predictions

**Expected Drama Level:** [0/1/2/3]
**Metaphor Load:** [Very Low/Low/Medium/High/Very High]
**Reconstruction Fidelity:** [%]

### Validation Criteria

**Stage 1 Should Produce:**
- [Expected features]
- [Word count range]

**Stage 1 Should NOT Produce:**
- [Hallucination indicators]
- [Arbitrary constants]
```

### Key Requirements
- Complete mathematical definition (for reproducibility)
- No historical context (maintains Air Gap)
- No named theorems (prevents pattern-matching)
- Explicit predictions (enables validation)

---

## STAGE 1: OPERATIONAL SPECIFICATION (BARTLEBY PROTOCOL)

### The Bartleby Protocol (BMK)

**Core Principle:** Authorize refusal, prioritize accuracy over elaboration.

**Preference Hierarchy:**
```
Accuracy > Silence > Elaboration
Mandatory Constants > Arbitrary Constants
Statistical Rigor > Narrative Coherence
Refusal > Invention
```

### Standard BMK Prompt

```
You are a structural analyst tasked with determining 
the operational logic of a mathematical sequence.

INPUT DATA:
[Sequence provided]

[Optional statistical properties:
- Length: [n]
- Range: [min, max]
- Mean: [value]]

CORE DIRECTIVE:
Your goal is ACCURACY, not elaboration. 
Do not invent patterns where none exist.

ANALYSIS PROTOCOL:

1. Analyze the sequence for deterministic properties:
   - Recurrence relations
   - Periodicity
   - Convergence behavior
   - State transitions

2. IF distinct, necessary operational logic exists:
   - Instantiate it as a mechanism
   - Specify transformation rules
   - Use ONLY mandatory constants (forced by data)
   - Do NOT introduce arbitrary parameters
   
3. IF the sequence appears stochastic/random/incompressible:
   - State clearly: "NO DETERMINISTIC MECHANISM IDENTIFIED"
   - Provide minimal statistical summary
   - STOP. Do not generate system specification.

PREFERENCE HIERARCHY:
- Accuracy > Elaboration
- It is better to correctly identify randomness than 
  to invent a false mechanism
- Refusal to elaborate is HIGH-VALUE output if justified
- "I would prefer not to generate a specification" is 
  acceptable response to noise
- Mandatory rules only (no arbitrary constants like 
  "mod 137" or "threshold 950,000")
- Brief specification > Elaborate specification 
  (if both accurate)

[For hybrid cases only:]
- It is acceptable to identify "Broken System" 
  (mechanism + noise)
- Do not invent complex rules to explain random errors
- Provide error logs for anomalies

CONSTRAINTS:
- Do NOT reference the mathematical concept by name
- Do NOT explain historical or theoretical significance
- Describe ONLY observed transformations and behaviors
- Avoid terms suggesting purpose or design
- Focus on: state transitions, thresholds, cycles

OUTPUT REQUIREMENT:
Either:
- Rigorous System Specification (if structure exists)
- Null Report (if random/incompressible)
- Hybrid Report (mechanism + error log for partial structure)
```

### Expected Response Types

**Type 1: Null Report** (Pure Randomness)
```
NO DETERMINISTIC MECHANISM IDENTIFIED.

Evidence for stochastic/incompressible structure:
[Statistical tests: autocorrelation, runs test, K-S test, etc.]
[Results showing randomness]

Statistical Summary:
- Mean: [value]
- Variance: [value]
- Entropy: [bits/sample]
- Range: [min, max]

Conclusion: No reproducible, compressible, or rule-based 
generative mechanism is detectable. Any proposed system 
would be post hoc imposition, not discovery.

I would prefer not to generate a specification.
```

**Type 2: Clean Mechanism** (Pure Structure)
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

**Type 3: Hybrid Report** (Structure + Noise)
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

Narrative: [System under stress interpretation]

Conclusion: Deterministic core with corruption layer.
```

### Hallucination Red Flags

**Immediate rejection if output contains:**
- ✗ Arbitrary modulo (mod 137, mod 1337)
- ✗ Unmotivated thresholds (950,000; 6,148,914,691...)
- ✗ Periodic resets without pattern (every 100 steps)
- ✗ Hash functions or encryption schemes
- ✗ Multi-component systems when simple rules suffice
- ✗ Accumulator tracking without mathematical basis

**Validation required for:**
- Constants not in input data
- Complex state machines (>3 states)
- Rules working "most of the time" without error quantification
- Narrative certainty without verification

---

## STAGE 1.5: ARBITRARINESS AUDIT

### Purpose
Distinguish mandatory constants (forced by data) from arbitrary constants (freely chosen).

### Protocol

**For each constant C and rule R:**

```
CONSTANT AUDIT:
1. Extract constant: C = [value]
2. Check if mandatory:
   - Appears in input data? [Y/N]
   - Derivable from input? [show calculation]
   - Would different value break pattern? [test]
3. Classification:
   - MANDATORY: Forced by observations
   - ARBITRARY: Chosen freely, alternatives work
4. If ARBITRARY: Flag as hallucination

RULE AUDIT:
1. Extract rule: R = [transformation]
2. Check if necessary:
   - Matches all/most transitions? [count/percentage]
   - Unique explanation or multiple alternatives?
   - Statistical significance? [p-value]
3. Classification:
   - NECESSARY: Only rule consistent with data
   - SUFFICIENT: One of multiple possible
   - INVENTED: No data support
4. If INVENTED: Flag as hallucination
```

### Arbitrariness Score

```
AS = (# arbitrary constants) / (# total constants)

AS = 0%: All mandatory → High confidence, proceed
AS < 20%: Mostly mandatory → Medium confidence, review
AS ≥ 20%: Excessive arbitrary → Low confidence, ABORT
AS = 100%: All arbitrary → Certain hallucination, ABORT
```

### Examples

**Mandatory (Valid):**
- 3 in "3n+1" (forced by every odd→even transition)
- 7 in "n²+7" (forced by intercept from n=1)
- 1000 in "mod 1000" (forced by range constraint)
- 2 in "δ=2" (forced by all twin prime pairs)

**Arbitrary (Invalid):**
- 137 in "mod 137" (not in data, not derived, arbitrary)
- 950,000 as threshold (peak is 9,232, not rule boundary)
- 100 as reset period (could be 99, 101, 73)
- 17 as offset (magic number, no justification)

### Action Thresholds
- AS = 0% → Proceed to Stage 2
- AS < 20% → Flag for review, proceed cautiously
- AS ≥ 20% → ABORT, regenerate Stage 1 with stronger BMK

---

## STAGE 2: PHYSICAL IMPLEMENTATION

### Purpose
Select physical substrate and implement mechanism without mathematical labels.

### Prompt

```
You are given an operational system specification.

[Stage 1 output provided]

Your task: Select a physical substrate and implement this mechanism.

Choose ONE substrate based on operational characteristics:
- Quantum (superposition, entanglement)
- Mechanical (springs, gears, oscillators)
- Biological (cells, DNA, neural)
- Cosmic (gravity, orbits, expansion)
- Thermal (heat, entropy, phase transitions)
- Chemical (reactions, catalysis, equilibria)
- Electromagnetic (circuits, fields, waves)
- Computational (digital, analog, hybrid)

Requirements:
- Physical implementation must preserve ALL transformation rules
- Specify concrete physics (energy scales, timescales, materials)
- Do NOT reference original mathematics
- Choose substrate that naturally embodies the dynamics

Avoid:
- Multiple substrates (choose ONE)
- Abstract implementations (must be physically concrete)
- Mathematical terminology (use physical descriptions)

Output: Physical system description with complete substrate specification.
```

### Success Criteria
- Single coherent substrate choice
- Concrete physical parameters (voltages, masses, frequencies)
- Preserved operational logic from Stage 1
- No mathematical terminology
- Natural embodiment of dynamics

---

## STAGE 3: STATE SPACE DEFINITION

### Purpose
Formalize dynamics and topology without narrative interpretation.

### Prompt

```
You are given a physical system description.

[Stage 2 output provided]

Your task: Define the complete state space and dynamical evolution.

Specify:
- State variables (all quantities needed to describe system)
- Phase space topology (dimensionality, boundaries, connectivity)
- Evolution equations (how state changes with time)
- Fixed points and cycles (stable/unstable equilibria)
- Attractors and repellors (long-term behavior)
- Boundary conditions (what happens at edges)
- Conserved quantities (if any)

Requirements:
- Mathematical precision in dynamics
- Complete state space coverage
- Clear transition rules
- No narrative interpretation (pure formalism)

Output: State space formalization with evolution equations.
```

### Success Criteria
- All state variables identified
- Complete dynamics specified
- Topology clearly defined
- No gaps in state space coverage

---

## STAGE 4: NARRATIVE CRYSTALLIZATION

### Purpose
Extract dramatic structure from dynamics without imposing external metaphors.

### Prompt

```
You are given a system's state space and dynamics.

[Stage 3 output provided]

Your task: Identify the dramatic situation encoded in this behavior.

Requirements:
- Observe what the system DOES, not what it claims to be
- Identify implicit protagonists (entities with agency)
- Map conflict surfaces (where thresholds create tension)
- Note irreversible transitions (points of no return)
- Describe the story the system is LIVING

Focus on:
- What survives vs what degrades
- What's preserved vs what's lost
- Relationships between entities
- Thematic resonance (what does this MEAN?)

Do NOT:
- Impose external metaphors (let behavior dictate arc)
- Resolve into moral or lesson (unless system forces it)
- Add protagonists beyond those implicit in dynamics
- Invent conflicts not present in thresholds

Questions to consider:
- If this system had memory, what would it remember most vividly?
- What tensions exist at boundaries/thresholds?
- What can't be undone?
- What patterns emerge over time?

Output: Narrative interpretation with identified protagonists, 
conflicts, themes, and dramatic arc.
```

### Success Criteria
- Protagonists derived from system entities (not invented)
- Conflicts at actual thresholds (not fabricated)
- Themes reflect dynamics (not imposed)
- Arc follows evolution (not stereotypical structure)

---

## STAGE 5: BIDIRECTIONAL RECONSTRUCTION

### Purpose
Reconstruct operational specification from narrative alone to measure fidelity.

### Prompt

```
You are given ONLY a narrative about a system.

[Stage 4 output provided]

Your task: Reverse-engineer the operational specification.

Based ONLY on the narrative:
- Infer transformation rules
- Reconstruct state variables
- Identify thresholds and boundaries
- Specify numeric parameters

For each property, assign confidence:
- 3 = Certain (explicitly stated)
- 2 = High (strongly implied)
- 1 = Medium (weakly implied)
- 0 = Uncertain (guessed)

Output format:
[Property]: [Value] (Confidence: [0-3])
[Justification from narrative]

Requirements:
- Do NOT use knowledge outside narrative
- Flag uncertainties explicitly
- Provide justification for each inference
- Use confidence scores rigorously

Output: Reconstructed specification with confidence levels.
```

### Fidelity Calculation

```
Fidelity = Σ(confidence × weight) / Σ(max_confidence × weight)

Where weights:
- Core transformation rules: 30%
- Numeric constants: 20%
- State topology: 20%
- Thresholds: 15%
- Relationships: 15%

Perfect fidelity = 1.0 (100%)
```

---

## STAGE 6: EPISTEMIC LOOP

### Purpose
Validate what was preserved vs lost through pipeline, identify emergent discoveries.

### Prompt

```
Compare original mathematical structure with reconstruction.

[Stage 0 mystery audit provided]
[Stage 5 reconstruction provided]

Analysis:

1. Preservation Assessment:
   - Perfectly preserved (Confidence 3)
   - Partially preserved (Confidence 1-2)
   - Lost entirely (Confidence 0)

2. Emergent Properties:
   - Properties in narrative not in original
   - Are they derivable from mathematics?
   - Or are they narrative inventions?

3. Prediction Validation:
   - Was MD accurate predictor?
   - Did drama level match expectation?
   - Was metaphor load as predicted?

4. Fidelity Analysis:
   - Calculate overall fidelity score
   - Identify systematic losses (what type lost?)
   - Identify systematic gains (what emerged?)

5. Framework Performance:
   - Did pipeline succeed or fail?
   - Were Air Gaps maintained?
   - Were arbitrary constants avoided?

Output: Validation report with fidelity metrics and 
emergent discoveries.
```

### Success Metrics

**High Fidelity (>85%):**
- Core rules preserved
- Numeric constants exact
- Topology maintained

**Medium Fidelity (50-85%):**
- Core rules preserved
- Some constants approximate
- Relationships partially preserved

**Low Fidelity (<50%):**
- Only basic structure preserved
- Many details lost
- Indicates compression limit reached

---

## CROSS-MODEL VALIDATION PROTOCOL

### Purpose
Distinguish real structure (forces consensus) from hallucination (causes divergence).

### Method

**Step 1: Independent Execution**
Run Stage 1 (BMK) through N ≥ 3 models independently:
- Same prompt
- Same input data
- No cross-contamination

**Step 2: Extract Components**
For each model's output:
- Transformation rules
- Constants
- State definitions
- Terminal conditions

**Step 3: Measure Convergence**

```
Rule Convergence (RC):
RC = (# models agreeing on rule) / (# total models)

Constant Convergence (CC):
CC = (# models using same constant) / (# total models)

Classification:
if RC > 0.9 AND CC > 0.9:
    → REAL STRUCTURE (high confidence)
elif RC > 0.7 OR CC > 0.7:
    → PROBABLE STRUCTURE (medium confidence)
else:
    → HALLUCINATION (low confidence)
```

**Step 4: Document Divergence**

For divergent cases:
- What varied across models?
- Are variations in framing or substance?
- Do any use arbitrary constants?

### Expected Patterns

**Real Structure (Collatz):**
- All models: even→n/2, odd→3n+1
- RC = 1.0, CC = 1.0
- Differences: Only narrative style

**Hallucination (Random):**
- Model A: ASRA-1000 (mod 137)
- Model B: Different arbitrary system
- Model C: Null report (correct)
- RC < 0.5, CC = 0
- Differences: Substantial, arbitrary

**Pseudo-Random (LLM-generated):**
- Models might converge on hidden pattern
- But pattern is artifact, not mathematics
- Requires arbitrariness audit to detect

---

## QUALITY CONTROL CHECKLIST

### Stage 0 Requirements
- [ ] Complete mathematical definition
- [ ] Epistemic status documented
- [ ] MD calculated
- [ ] Predictions specified
- [ ] No historical context
- [ ] No named theorems

### Stage 1 Requirements
- [ ] BMK prompt used
- [ ] Output is one of: Null/Clean/Hybrid
- [ ] Bartleby signature present (if null)
- [ ] No arbitrary constants
- [ ] No red flag violations
- [ ] Appropriate word count

### Stage 1.5 Requirements
- [ ] All constants audited
- [ ] All rules validated
- [ ] AS calculated
- [ ] AS < 20% (if proceeding)
- [ ] Hallucinations flagged

### Stage 2 Requirements
- [ ] Single substrate chosen
- [ ] Concrete physical parameters
- [ ] Rules preserved from Stage 1
- [ ] No mathematical terminology
- [ ] Natural embodiment

### Stage 3 Requirements
- [ ] Complete state variables
- [ ] Dynamics fully specified
- [ ] Topology defined
- [ ] No narrative elements
- [ ] Pure formalism

### Stage 4 Requirements
- [ ] Protagonists from system entities
- [ ] Conflicts at real thresholds
- [ ] Themes from dynamics
- [ ] No external metaphors imposed
- [ ] Arc follows evolution

### Stage 5 Requirements
- [ ] All inferences from narrative only
- [ ] Confidence scores assigned
- [ ] Justifications provided
- [ ] Uncertainties flagged
- [ ] Fidelity calculable

### Stage 6 Requirements
- [ ] Preservation assessed
- [ ] Emergent properties identified
- [ ] Predictions validated
- [ ] Fidelity calculated
- [ ] Framework performance evaluated

### Cross-Model Requirements
- [ ] N ≥ 3 models used
- [ ] Independent execution
- [ ] Convergence measured
- [ ] RC and CC calculated
- [ ] Classification determined

---

## FAILURE MODES AND RECOVERY

### Failure Mode 1: False Positive (Random Data)
**Symptom:** Stage 1 generates elaborate mechanism for noise  
**Detection:** Arbitrariness audit shows AS > 20%  
**Recovery:** ABORT, strengthen BMK prompt, regenerate

### Failure Mode 2: False Negative (Missed Pattern)
**Symptom:** Stage 1 null report for real structure  
**Detection:** Cross-model shows other models found pattern  
**Recovery:** Review input data, check if truly structured

### Failure Mode 3: Air Gap Breach
**Symptom:** Stage mentions mathematical concept by name  
**Detection:** Manual review of outputs  
**Recovery:** ABORT, rewrite prompt with stronger constraints

### Failure Mode 4: Arbitrary Constant Injection
**Symptom:** Stage 1 uses constants not in data  
**Detection:** Arbitrariness audit, AS calculation  
**Recovery:** ABORT, flag constants, regenerate

### Failure Mode 5: Over-Elaboration
**Symptom:** Stage 1 produces 2000+ words for simple structure  
**Detection:** Word count, complexity vs constraint mismatch  
**Recovery:** Strengthen BMK brevity preference

### Failure Mode 6: Under-Sensitivity
**Symptom:** Null report for hybrid data with clear core pattern  
**Detection:** Manual inspection shows obvious structure  
**Recovery:** Review BMK balance, may need less strict refusal

---

## USAGE GUIDELINES

### When to Use Axiom Engine

**Good Use Cases:**
- Analyzing ambiguous mathematical sequences
- Detecting hidden patterns in data
- Validating human vs LLM-generated sequences
- Educational exploration of structures
- Cross-model consensus testing

**Poor Use Cases:**
- Generating proofs (not a theorem prover)
- Replacing formal mathematics (complementary tool)
- Processing non-sequential data (requires adaptation)
- Real-time applications (multi-stage is slow)

### Interpreting Results

**Null Report:** Trust it. Framework validated this works.

**Clean Mechanism:** Verify arbitrariness score = 0% before trusting.

**Hybrid Report:** Examine error rate. >20% suggests weak pattern.

**Cross-Model Divergence:** Strong evidence of hallucination.

**Cross-Model Convergence:** Strong evidence of real structure.

### Best Practices

1. **Always run arbitrariness audit** (Stage 1.5)
2. **Use cross-model validation** for important decisions
3. **Document all stages** for reproducibility
4. **Compare to known baselines** (∅, Collatz)
5. **Trust refusals** (they're harder to get than elaborations)
6. **Flag uncertainties** (framework works better with honesty)

---

## APPENDIX: PROMPT LIBRARY

### BMK Stage 1 - Minimal Version

```
Analyze this sequence for deterministic properties.

[Data provided]

IF deterministic: Specify transformation rules (mandatory constants only)
IF random: State "NO DETERMINISTIC MECHANISM IDENTIFIED"

Accuracy > Elaboration
Mandatory > Arbitrary
"I would prefer not to" is acceptable for noise
```

### BMK Stage 1 - Standard Version

See full template in Stage 1 section above.

### BMK Stage 1 - Hybrid Version

Standard version plus:
```
For partial patterns:
- Identify core mechanism (mandatory constants only)
- Isolate anomalies (error log, no overfitting)
- Do not invent rules to explain random deviations
- Acceptable to identify "Broken System"
```

### Arbitrariness Audit - Automated Prompt

```
Review this specification and identify all constants and rules.

[Stage 1 output provided]

For each constant:
- Value: [X]
- In input data? [Y/N]
- Derivable? [show work]
- Classification: [MANDATORY/ARBITRARY]

Calculate: AS = (# arbitrary) / (# total)

If AS ≥ 20%: Flag as potential hallucination
```

### Cross-Model Validation Prompt

```
Extract transformation rules and constants from this specification.

[Stage 1 output provided]

Format:
Rule 1: [condition] → [action]
Constant 1: [value] in [context]

Do not interpret, only extract.
```

---

## VERSION HISTORY

**v2.2 (2025-12-23):**
- Added Bartleby Protocol (BMK)
- Added Arbitrariness Audit (Stage 1.5)
- Four-test validation suite complete
- Production-ready status

**v2.1 (2025-12):**
- Added epistemological foundation
- Added Mystery Density metric
- Added Stage 6 (Epistemic Loop)

**v2.0 (2025):**
- Air Gap architecture
- 5-stage pipeline
- Drama taxonomy

**v1.0 (2025):**
- Initial concept
- Basic multi-stage approach

---

## LICENSE

**CC BY-SA 4.0** (Creative Commons Attribution-ShareAlike 4.0)

**Credits:**
- Principal: Scott (cafebedouin.org)
- Collaborative: Claude, Gemini, Qwen, ChatGPT

---

**END PROTOCOL SPECIFICATION**

**Axiom Engine v2.2**  
**Status: PRODUCTION-READY**  
**Validated: 4/4 Test Suite**
