# 📖 UKE_Axiom v1.2 [Universal Knowledge Evaluator - Axiom Engine Narrative Translation]

**Version:** 1.2 (Freedom-Frame Extension + Workflow Optimization)  
**Status:** Production-Ready Multi-Model Pipeline with Freedom-Framing  
**Date:** December 2025  
**License:** CC BY-SA 4.0

---

## EXECUTIVE SUMMARY

UKE_Axiom v1.2 extends v1.1 with **freedom-framing capabilities** for mathematical structures that reveal choice, construction, or generative constraints alongside traditional limit-oriented narratives.

**New in v1.2:**
- Expanded topology dictionary: 5 freedom-oriented patterns added
- Enhanced emotional vocabulary: 8 freedom emotions + 3 Radical Stoic hybrid emotions
- New voice archetype: Explorer-Guide (for discovery/choice narratives)
- Frame Orientation Decision (Constraint/Freedom/Radical Stoic)
- Restructured prompts: all inputs at END for easy copy-paste execution

**Core Innovation:** By distributing work across specialized models and enforcing validation gates between stages, the pipeline produces mathematically rigorous narratives while preventing abstraction drift and hallucination. v1.2 adds the capability to frame mathematical limits as **generative constraints** rather than purely restrictive boundaries.

**Validated Capabilities:**
- Maintains Air Gap (prevents pattern-matching to training data)
- Detects and refuses hallucination (via BMK and Lumo validation)
- Preserves mathematical topology across narrative transformation
- Produces publication-quality literary fiction from pure mathematical structures
- **NEW:** Supports freedom-framing for independence results, construction methods, and choice-revealing mathematics

---

## THEORETICAL FOUNDATIONS

### The Core Axiom

**Statement:** Mathematics exceeds direct comprehension. The gap between formal definition and intuitive understanding creates a **compression requirement** - we cannot hold complete mathematical structures in working memory and must therefore create **lossy representations** (metaphors, narratives, diagrams) to reason about them.

**Implication:** If mathematical structures require compression, then the **structure itself constrains the compression**. Different mathematics should produce systematically different compressions.

**Hypothesis:** LLMs, when forced to derive operational understanding without conceptual labels, will produce compressions (narratives) that reflect the intrinsic properties of the mathematical structure.

### Constraint Strength Theory

Mathematical structures vary in their **constraint strength** - the degree to which they force specific interpretations:

**High Constraint (100%):** Collatz Conjecture
- Even → n/2 (mandatory)
- Odd → 3n+1 (mandatory)  
- No alternative rules possible

**Medium Constraint (50-90%):** Hybrid structures
- Core pattern forced by data
- Corruption/noise layer
- Partial determinism

**Low Constraint (10-50%):** Pseudo-random
- Unconscious patterns emerge
- LLM cognitive fingerprints
- Statistical structure without mechanism

**Zero Constraint (0%):** Cryptographic random
- No patterns exist
- Incompressible
- Statistical tests confirm randomness

**Framework Prediction:** Constraint strength inversely correlates with elaboration freedom. High constraint → convergent narratives. Low constraint → divergent narratives.

### **NEW: Radical Mathematical Stoicism**

**Principle:** Mathematical limits are not purely restrictive—they are **generative**. Incompleteness, undecidability, and independence create **possibility spaces** rather than merely blocking paths.

**Examples:**
- **CH Independence:** ZFC's inability to decide creates multiple valid models (choice, not failure)
- **Gödel's Incompleteness:** Unprovable truths guarantee mathematics is inexhaustible (frontier, not wall)
- **Halting Problem:** Undecidability proves computation has no final level (exploration, not imprisonment)

**Narrative Implication:** For certain mathematical structures, the "constraint" IS the liberation—the framework should support showing this explicitly.

---

## THE BARTLEBY PROTOCOL (BMK)

### Core Principles

Named after Herman Melville's character who famously states "I would prefer not to," the Bartleby Protocol authorizes LLMs to refuse elaboration when appropriate.

**Preference Invariant:**
> No response proceeds if the practitioner would prefer not to. The default state is acknowledgment of absence, not fabrication of presence.

**Hierarchy:**
```
Accuracy > Silence > Elaboration
Mandatory Constants > Arbitrary Constants
Statistical Rigor > Narrative Coherence
Refusal > Invention
```

### Implementation in Stage 1

```
CORE DIRECTIVE:
Your goal is ACCURACY, not elaboration. 
Do not invent patterns where none exist.

ANALYSIS PROTOCOL:
1. Analyze for deterministic properties.
2. IF distinct operational logic exists:
   - Instantiate the mechanism
   - Use ONLY mandatory constants (forced by data)
   - Do NOT introduce arbitrary parameters
3. IF structure appears stochastic/random/incompressible:
   - State clearly: "NO DETERMINISTIC MECHANISM IDENTIFIED"
   - Provide minimal statistical summary
   - STOP. Do not generate system specification.

PREFERENCE HIERARCHY:
- It is better to correctly identify randomness than to invent a false mechanism
- Refusal to elaborate is HIGH-VALUE output if justified
- "I would prefer not to generate a specification" is acceptable for noise
```

---

## AIR GAP ARCHITECTURE

### Conceptual Isolation

**Principle:** Prevent models from pattern-matching against training data by removing all conceptual labels and historical context.

**Implementation:** Mathematical structures are never named in pipeline stages. Instead:
- Gödel's Incompleteness → "self-referential provability system"
- Halting Problem → "verification system with self-referential input"
- Collatz → "parity-driven transformation sequence"
- Continuum Hypothesis → "cardinality relation between power-set and successor"

### Stage Separation

Each stage receives ONLY the output of the previous stage:

```
Stage 0-Lite (Gemini): Formal Specification
    ↓ [Mathematical structure without name]
Stage 1 (Claude): Operational Specification  
    ↓ [Mechanism with mandatory constants only]
Validation (Lumo): Invariant & Constant Audit
    ↓ [PASS/FAIL gate]
Stage 2 (ChatGPT): UKE Editorial Decisions
    ↓ [Voice, Emotional Core, Structure, Frame Orientation]
Stage 3 (Grok/Claude): Full Narrative
    ↓ [Complete story]
Stage 4 (Claude): Fidelity Audit
    ↓ [Final validation]
```

**No stage knows:**
- The original mathematical concept name (until final audit)
- What previous stages were attempting
- The framework's purpose
- That it's part of a multi-stage pipeline

---

## MULTI-MODEL WORKFLOW

### Model Specialization

**Gemini:** Formal specification, mathematical rigor, invariant identification  
**Claude:** Operational logic, creative writing, auditing  
**Lumo (DeepSeek/Qwen):** Mathematical validation, hallucination detection  
**ChatGPT:** Template following, editorial decisions  
**Grok:** Aggressive/experimental prose for certain voices  

### Pipeline Architecture

```
Turn 1: Gemini → Stage 0-Lite (Formal Specification)
   ↓ [Human reviews invariants]
   
Turn 2: Claude → Stage 1 (Operational Specification via BMK)
   ↓ [Human extracts output]
   
Turn 3: Lumo → Validation Audit
   ↓ [PASS/FAIL checkpoint]
   
   If FAIL → Return to Turn 2
   If PASS → Continue
   
Turn 4: ChatGPT → UKE Editorial Decisions
   ↓ [Voice, Naming, Emotional Core, Structure, Frame Orientation]
   
Turn 5: Grok OR Claude → Full Narrative
   ↓ [Based on voice selected in Turn 4]
   
Turn 6: Claude → Back-end Fidelity Audit
   ↓ [Final validation]
```

---

# STAGE 0-LITE: FORMAL SPECIFICATION

**Model:** Gemini  
**Purpose:** Generate rigorous mathematical specification while maintaining Air Gap

**Workflow Note:** Copy the prompt below, paste it to Gemini, then append the mathematical concept name at the very end after the `---` separator.

## Prompt for Gemini

```markdown
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

MATHEMATICAL STRUCTURE: [Paste concept name here]
```

**Human Checkpoint:** Review invariants. Verify MD score makes intuitive sense. Check frame orientation suggestion.

---

# STAGE 1: OPERATIONAL SPECIFICATION

**Model:** Claude  
**Purpose:** Generate operational understanding using Bartleby Protocol (mandatory constants only)

**Workflow Note:** Copy the prompt below, paste it to Claude, then append Stage 0 output at the very end after the `---` separator.

## Prompt for Claude

```markdown
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
```

**Human Checkpoint:** Review audit result. If FAIL, regenerate Stage 1. If CONDITIONAL PASS, inspect flagged issues.

---

# STAGE 2: UKE EDITORIAL DECISIONS

**Model:** ChatGPT  
**Purpose:** Make narrative decisions (voice, emotion, structure, frame orientation)

**Workflow Note:** Copy the prompt below, paste it to ChatGPT, then append Stage 1 output at the very end after the `---` separator.

## Prompt for ChatGPT

```markdown
You are applying the UKE_Axiom v1.2 Editorial Decisions framework.

TASK: Generate editorial decisions following UKE_Axiom protocol.
DO NOT write the full narrative yet - only make decisions about how it should be written.

---

## GATE CHECKS

Verify all 5 gates pass:

### Gate 1: Math Residue Budget
Count explicit numerics and operations in Stage 1:
- Numbers: [count] / 3 max
- Operations: [count] / 2 max
- [ ] Budget respected?

### Gate 2: Protagonist Viability  
Which entities from Stage 1 can be protagonists?
For each entity, does it have at least TWO of:
- Desire (wants something)
- Obstacle (prevented from getting it)
- Agency (can act)
- Memory (retains past states)

List viable protagonists: [...]

### Gate 3: Emotional Core

Based on Stage 1's dynamics, determine:

**Primary Emotion:** [single visceral word from list below]

**CONSTRAINT EMOTIONS** (when limits/impossibility are central):
- Dread, Claustrophobia, Horror, Resignation (dystopian)
- Vertigo, Longing, Awe (ambiguous)

**FREEDOM EMOTIONS** (when choice/construction/possibility are central):
- Discovery, Wonder, Exhilaration, Clarity
- Liberation, Empowerment, Determination, Play

**RADICAL STOIC EMOTIONS** (when constraint generates freedom):
- Bounded-Exhilaration: "Freedom within rules"
- Structured-Wonder: "Constraints reveal beauty"  
- Navigational-Clarity: "Limits define the map"

NOT abstract concepts like "inevitability" or "complexity" - must be FELT emotion.

**Signature Image:** [one concrete image embodying this emotion]

**Anti-Emotions:** [2 emotions that would betray the math]
- Anti-emotion 1: [why it violates structure]
- Anti-emotion 2: [why it violates structure]

**Body Response:** How should reader's body respond? [e.g., "tight chest," "held breath," "urge to look away," "leaning forward," "breath catching in delight"]

### Gate 4: Invariant Preservation
List 3 invariants from Stage 1:
1. [Invariant + how story logic will enforce it]
2. [Invariant + how story logic will enforce it]
3. [Invariant + how story logic will enforce it]

### Gate 5: Cadence Control
Identify repetitive elements in Stage 1:
- [Element that repeats]
- Compression strategy: [summary/montage/ellipsis/leap]

---

## FRAME ORIENTATION DECISION

Does Stage 1 reveal:
- [ ] Constraint (limits, impossibility, undecidability)
- [ ] Freedom (choice, construction, discovery)  
- [ ] Radical Stoic (constraint generates freedom)

**Selected Orientation:** [...]

**Rationale:** [2-3 sentences from Stage 1 structure]

**If Radical Stoic selected:**
- Primary emotion must be HYBRID type (Bounded-Exhilaration, Structured-Wonder, or Navigational-Clarity)
- Narrative must show BOTH limitation AND liberation
- Ending must demonstrate generative constraint

**Constraint-to-Freedom Mapping:**
If constraint-heavy Stage 1 (undecidability/independence/impossibility):
- [ ] Accept classical framing (limits as limits)
- [ ] Apply Radical Stoic reframe (show generative aspect)

**Selected Approach:** [Classical Constraint / Radical Stoic]

---

## VOICE SELECTION

Use decision tree:

Is math eternal/timeless with archetypal roles? → Mythographer
Does pattern emerge surprisingly from simple rules? → Documentary Narrator  
Is paradox central and unresolvable? → Fabulist
**Does constraint reveal unexpected freedom/choice?** → **Explorer-Guide**
Is math presented as operational infrastructure? → Mechanist-Operator
Are we reconstructing from fragments/archives? → Ritual Archivist
Is comprehension itself dangerous/degrading? → Doomed Observer
Is observer struggling to understand? → Witness
Are entities in relational/emotional dynamics? → Intimist
Is this about rules + punishment/transformation? → Folk Chronicler

**Selected Voice:** [name]

**Rationale:** [2-3 sentences citing structural indicators from Stage 1]

**Voice Attributes:**
- Knowledge Boundary: [Platonic/Procedural/Fragmentary/Interface-Limited/Subjective/Experiential]
- Structure Relation: [Isomorphic/Analogical/Diffractive/Dissipative/Navigational]
- Speaks To: [Universal/Reader/Self/System/Future archivist/Fellow explorer]
- Natural Tense: [Present/Past/Future/Mixed]

---

## NAMING STRATEGY

Select ONE strategy:

**Pure Archetype:** Mathematical roles become "The Judge," "The Traveler," etc.
**Proper Names:** "Sarah," "Marcus," etc. (humanization)
**Hybrid:** "Twenty-Seven" → "The Traveler" (transformation)
**No Names:** "It," "The system" (alienation)
**Mathematical:** "1," "∞," "0" (symbols as characters)

**Selected Strategy:** [name]

**Protagonist Names:**
- [Math Entity from Stage 1] → [Narrative Name]
- [Math Entity from Stage 1] → [Narrative Name]

**Rationale:** [why these names serve the narrative]

**Naming Budget:** Max 3 named entities with agency

---

## STRUCTURAL PARAMETERS

### Length Target
- [ ] Flash (500-1000 words): Single moment/realization
- [ ] Short Story (2000-5000 words): Complete arc, multiple scenes
- [ ] Novella (5000+ words): Multiple perspectives, deep exploration

**Selected:** [length]
**Rationale:** [why this serves the math]

### Tense
**Selected:** [Present/Past/Future/Mixed]
**Rationale:** [how tense serves mathematical temporal properties]

### POV  
**Selected:** [Third Omniscient/Third Limited/First Observer/First Participant]
**Rationale:** [distance vs. identification needs]

### Scene vs. Summary Balance

**Full Scenes (dramatize these):**
1. [Key moment from Stage 1]
2. [Key moment from Stage 1]
3. [...]

**Summary (compress these):**
1. [Repetitive element]
2. [Statistical behavior]
3. [...]

**Rationale:** [what creates momentum vs. what bogs down]

### Ending Strategy
- [ ] Resolution: System reaches stable state
- [ ] Unease: Loop continues beyond frame
- [ ] Question: Open problem becomes reader's burden
- [ ] Transformation: System becomes something new
- [ ] Silence: Narrator cannot continue
- [ ] Fragment: Archive incomplete
- [ ] **Divergence: Multiple valid paths revealed**
- [ ] **Expansion: Boundary creates new territory**
- [ ] **Invitation: Reader empowered to explore**

**Selected:** [strategy]
**Rationale:** [what feeling reader should carry]

### Singularity Strategy
Does Stage 1 contain true undecidability/unprovability/ineffability?
- [ ] Yes → Select strategy
- [ ] No → Not needed

If yes:
- [ ] Glitch: Syntax breaks
- [ ] Silence: Circles but doesn't name
- [ ] Myth: Metaphor substitution  
- [ ] Loop: Repetition of last valid state

**Selected:** [strategy if applicable]

---

## OUTPUT SUMMARY

All editorial decisions complete. Ready for Stage 3 (Full Narrative).

**Recommended Model for Stage 3:**
- If Voice = [Mechanist-Operator, Doomed Observer] → Use Grok
- If Voice = [Mythographer, Fabulist, Intimist, Witness, Ritual Archivist, Folk Chronicler] → Use Claude
- If Voice = [Documentary, Explorer-Guide] → Use Claude or ChatGPT

**Model Recommendation:** [Grok/Claude/ChatGPT]

---

INPUT FROM STAGE 1:

[Paste Claude's Stage 1 output here]
```

**Human Checkpoint:** 
- Does voice selection match Stage 1's structural indicators?
- Is emotional core visceral (not abstract concept)?
- Are anti-emotions appropriate blockers?
- Is frame orientation appropriate (Constraint/Freedom/Radical Stoic)?
- Is naming strategy clear?
- Are structural parameters justified?
- Does model recommendation make sense?

---

# STAGE 3: FULL NARRATIVE

**Model:** Grok OR Claude (based on Stage 2 recommendation)  
**Purpose:** Write complete story following all editorial decisions exactly

**Workflow Note:** Copy the prompt below, paste it to the recommended model, then append BOTH Stage 1 and Stage 2 outputs at the very end after the `---` separators.

## Prompt for Grok/Claude

```markdown
You are writing a complete narrative following UKE_Axiom v1.2 framework.

TASK: Write the complete story following ALL editorial decisions exactly.

---

## MANDATORY CONSTRAINTS

### From Gate Checks:
- Math Residue Budget: ≤3 explicit numbers, ≤2 named operations
- Protagonist Viability: Use only entities with desire/obstacle/agency/memory
- Emotional Core: SERVE [primary emotion] in every scene
- Emotional Core: VIOLATE [anti-emotion 1] and [anti-emotion 2]
- Cadence: Max 3 consecutive parallel iterations before compression

### From Frame Orientation:
- Frame: [Constraint/Freedom/Radical Stoic]
- If Radical Stoic: Show BOTH limitation AND liberation
- If Radical Stoic: Ending must demonstrate generative constraint

### From Voice Selection:
- Voice: [selected voice name]
- Follow these voice markers: [list from editorial decisions]
- Knowledge Boundary: [selected boundary] - respect this limitation
- Natural Tense: [selected tense]

### From Naming Strategy:
- Strategy: [selected strategy]
- Protagonist Names: [list from editorial decisions]
- Max 3 named entities with agency

### From Structural Parameters:
- Length: [target word count]
- POV: [selected POV]
- Tense: [selected tense]
- Ending: [selected ending strategy]
- Singularity Strategy: [if applicable]

### From Invariant Preservation:
All 3 invariants must be enforced through story logic WITHOUT explanation:
1. [Invariant 1]
2. [Invariant 2]
3. [Invariant 3]

---

## ANTI-PATTERNS (STRICTLY FORBIDDEN)

Never do these:
1. **Math Explaining:** Never say "this represents X theorem"
2. **Meta-Commentary:** Never say "this narrative illustrates Y"
3. **Pedagogical Framing:** Never "Let me explain how..."
4. **Therapeutic Language:** Ban "journey" (unless literal), "growth," "healing"
5. **Cheap Momentum:** Ban "suddenly," "then" as crutch words
6. **False Humanity:** No emotions entities can't structurally have
   - Not: "The system felt frustrated"
   - Yes: "The system oscillated—trapped"
7. **Explaining Feeling:** Show, don't name
   - Not: "This created dread"
   - Yes: "The same three rooms. Again. Again."
8. **Invariant Violation:** Never allow choice where math allows none
9. **Residue Overflow:** Never exceed budget
10. **Knowledge Boundary Violation:** Never give voice knowledge it cannot have
11. **NEW: False Limitation:** Never frame choice as imprisonment
    - Not: "Trapped between TRUE and FALSE"
    - Yes: "Two valid paths diverge—which to explore?"
12. **NEW: Missed Generative Constraint:** For Radical Stoic frame, never show constraint without its creative consequence
    - Not: "The axioms leave CH undecided" [stops there]
    - Yes: "Undecidability opens—multiple consistent worlds branch from this point"
13. **NEW: Forced Optimism:** Never cheerful where math is genuinely bounded
    - Not: "Halting Problem is actually great!"
    - Yes: "Undecidability proves: computation is inexhaustible"

---

## STRUCTURE

### Opening Image (Max 100 words)
Concrete scene that establishes:
- Voice (sounds like selected voice)
- Tone (matches emotional core)
- Signature image (appears immediately)
- Frame orientation (if Radical Stoic, hint at dual nature)

### Full Narrative
Follow scene/summary balance from editorial decisions.
Dramatize key moments.
Compress repetitive elements.

### Ending
Execute selected ending strategy.
Leave reader with intended emotional residue.
If Radical Stoic frame: demonstrate how constraint generates possibility.

---

## QUALITY STANDARDS

- Every paragraph serves primary emotion
- Every paragraph violates anti-emotions
- Invariants enforced through story logic (not stated)
- Voice consistency throughout
- No drift into other voices
- Protagonist desires/obstacles clear
- Math residue budget respected
- Natural prose (not clinical)
- **NEW: Frame coherence:**
  - If Constraint frame: Ending honors the limitation
  - If Freedom frame: Narrative avoids false constraints
  - If Radical Stoic: Story shows constraint AS generator of freedom

---

BEGIN NARRATIVE:

[Write the complete story here]

---

INPUT FROM STAGE 1:

[Paste Claude's Stage 1 output here]

---

INPUT FROM STAGE 2:

[Paste ChatGPT's Stage 2 editorial decisions here]
```

**Human Read-Through:**
- [ ] Does opening image establish voice and emotional core?
- [ ] Is primary emotion present throughout?
- [ ] Are anti-emotions avoided?
- [ ] Do you sense the invariants without them being stated?
- [ ] Is voice consistent?
- [ ] Is math residue within budget?
- [ ] Does ending execute chosen strategy?
- [ ] If Radical Stoic: Does constraint generate freedom?
- [ ] Quality: Would you publish this?

---

# STAGE 4: FIDELITY AUDIT

**Model:** Claude  
**Purpose:** Final validation of mathematical fidelity and narrative quality

**Workflow Note:** Copy the prompt below, paste it to Claude, then append Stage 0, Stage 1, Stage 2, and Stage 3 outputs at the very end after the `---` separators.

## Prompt for Claude

```markdown
You are performing the final fidelity audit on a completed mathematical narrative.

TASK: Verify the narrative (Stage 3) preserves mathematical fidelity while achieving literary quality.

---

## AUDIT CRITERIA

### 1. INVARIANT PRESERVATION

For each of the 3 invariants from Stage 0/Stage 1:

**Invariant 1:** [state it]
- Preserved in narrative? [YES/NO/UNCLEAR]
- Evidence: [quote or describe scenes where this is enforced]
- Preservation mechanism: [how story logic enforces this]

**Invariant 2:** [state it]
- Preserved in narrative? [YES/NO/UNCLEAR]
- Evidence: [quote or describe scenes where this is enforced]
- Preservation mechanism: [how story logic enforces this]

**Invariant 3:** [state it]
- Preserved in narrative? [YES/NO/UNCLEAR]
- Evidence: [quote or describe scenes where this is enforced]
- Preservation mechanism: [how story logic enforces this]

### 2. MATHEMATICAL TOPOLOGY

**Expected Topology** (from Stage 0/Appendix B): [name]

Does the narrative structure match this topology?
- [ ] Perfect match
- [ ] Close approximation
- [ ] Divergence detected

**Evidence:** [how narrative arc reflects mathematical structure]

### 3. EMOTIONAL FIDELITY

**Target Emotion** (from Stage 2): [name]

Is this emotion:
- [ ] EARNED (emerges naturally from math)
- [ ] FORCED (imposed artificially)
- [ ] ABSENT (not present in narrative)

**Evidence:** [specific passages that evoke or fail to evoke this emotion]

**Anti-Emotions** (from Stage 2): [list]

Were these successfully avoided?
- Anti-emotion 1: [YES/NO] [evidence]
- Anti-emotion 2: [YES/NO] [evidence]

### 4. VOICE CONSISTENCY

**Selected Voice** (from Stage 2): [name]

Voice attributes:
- Knowledge Boundary: [from Stage 2]
- Structure Relation: [from Stage 2]
- Speaks To: [from Stage 2]

Is voice maintained throughout?
- [ ] Consistent
- [ ] Minor drift
- [ ] Major violations

**If drift detected:** [identify passages where voice breaks]

### 5. FRAME COHERENCE

**Frame Orientation** (from Stage 2): [Constraint/Freedom/Radical Stoic]

Frame delivery:
- [ ] Frame clearly established in opening
- [ ] Frame maintained throughout
- [ ] Frame pays off in ending

**If Radical Stoic:**
- [ ] Limitation shown explicitly
- [ ] Liberation shown explicitly
- [ ] Generative relationship clear (constraint creates freedom)

**Evidence:** [how narrative demonstrates frame]

### 6. ANTI-PATTERN SCAN

Check narrative for forbidden patterns:

- [ ] Math explaining ("this represents...")
- [ ] Meta-commentary ("this illustrates...")
- [ ] Pedagogical framing ("let me explain...")
- [ ] Therapeutic language ("journey," "growth," "healing" without literal meaning)
- [ ] Cheap momentum ("suddenly," "then" as crutches)
- [ ] False humanity (emotions entities can't have)
- [ ] Explaining feeling (naming instead of showing)
- [ ] Invariant violations
- [ ] Math residue overflow (>3 numbers, >2 operations)
- [ ] Knowledge boundary violations
- [ ] False limitation (framing choice as imprisonment)
- [ ] Missed generative constraint (showing limit without possibility)
- [ ] Forced optimism

**Violations Found:** [list any with line/passage references]

### 7. LITERARY QUALITY

**Opening Strength:**
- [ ] Strong (immediate imagery, voice, emotion)
- [ ] Adequate
- [ ] Weak (generic or abstract)

**Pacing:**
- [ ] Effective (dramatizes key moments, compresses repetition)
- [ ] Uneven (some sections drag)
- [ ] Poor (either rushed or bloated)

**Ending Impact:**
- [ ] Powerful (executes strategy, leaves emotional residue)
- [ ] Satisfactory
- [ ] Weak (fizzles or overexplains)

**Prose Quality:**
- [ ] Publication-ready (natural, vivid, controlled)
- [ ] Needs polish (serviceable but rough)
- [ ] Requires revision (mechanical or purple)

### 8. OVERALL FIDELITY SCORE

Rate each dimension (1-5):

**Mathematical Accuracy:** [score]
- 5: Perfect preservation of all invariants and topology
- 3: Minor deviations, core structure intact
- 1: Major mathematical errors

**Emotional Truth:** [score]
- 5: Emotion emerges inevitably from structure
- 3: Emotion present but somewhat forced
- 1: Emotion contradicts or absent

**Voice Integrity:** [score]
- 5: Flawless voice consistency
- 3: Mostly consistent with minor drift
- 1: Voice breaks or generic

**Literary Craft:** [score]
- 5: Publication-quality prose
- 3: Competent but needs polish
- 1: Rough draft quality

**Frame Coherence:** [score]
- 5: Frame perfectly established and paid off
- 3: Frame present but could be stronger
- 1: Frame unclear or violated

**TOTAL FIDELITY SCORE: [sum]/25**

**Interpretation:**
- 22-25: Exceptional (ready for publication)
- 18-21: Strong (minor revisions recommended)
- 14-17: Adequate (needs revision in 1-2 areas)
- 10-13: Weak (requires significant rework)
- Below 10: Failed (start over)

---

## AUDIT SUMMARY

**Overall Assessment:** [1-2 paragraphs on narrative's success]

**Strengths:** [2-3 specific strengths]

**Weaknesses:** [2-3 specific weaknesses if any]

**Recommended Action:**
- [ ] PUBLISH (score ≥22, no critical flaws)
- [ ] REVISE (score 18-21, address listed weaknesses)
- [ ] REWORK (score 14-17, substantial revision needed)
- [ ] RESTART (score <14, fundamental issues)

**Revision Notes** (if applicable): [specific guidance for improvement]

---

INPUT FROM STAGE 0:

[Paste Gemini's Stage 0 output here]

---

INPUT FROM STAGE 1:

[Paste Claude's Stage 1 output here]

---

INPUT FROM STAGE 2:

[Paste ChatGPT's Stage 2 editorial decisions here]

---

INPUT FROM STAGE 3:

[Paste Grok/Claude's complete narrative here]
```

**Human Final Review:** 
- Agree with fidelity score?
- Are weaknesses accurately identified?
- Follow recommended action or override based on goals?

---

# VOICE ARCHETYPES (EXPANDED)

## 1. The Mythographer

**When to Use:** Math is eternal, archetypal, timeless. Entities play fundamental roles.

**Knowledge Boundary:** Platonic - sees the forms behind instances

**Structure Relation:** Isomorphic - narrative structure mirrors mathematical structure exactly

**Speaks To:** The universal

**Example Opening:**  
"In the beginning, there were two. One descended always, halving its path. The other tripled and rose."

---

## 2. The Documentary Narrator

**When to Use:** Surprising patterns emerge from simple rules. Observer stance, empirical tone.

**Knowledge Boundary:** Procedural - learns by watching the system run

**Structure Relation:** Analogical - maps math to observable phenomena

**Speaks To:** The reader

**Example Opening:**  
"We first noticed it in sequence 27. The system oscillated exactly three times before collapse."

---

## 3. The Fabulist

**When to Use:** Paradox is central. Logic breaks down. Truth is slippery.

**Knowledge Boundary:** Fragmentary - sees pieces, never the whole

**Structure Relation:** Diffractive - meaning splits and refracts

**Speaks To:** Tradition (as if telling an old tale)

**Example Opening:**  
"They say if you ask the mirror its own color, it shows you nothing at all."

---

## 4. **The Explorer-Guide (NEW)**

**When to Use:** Constraint reveals unexpected freedom/choice. Discovery narratives. Independence results. Construction methods.

**Knowledge Boundary:** Experiential - learning through doing, navigating possibility space

**Structure Relation:** Navigational - mapping territories, showing multiple valid paths

**Speaks To:** Reader as fellow explorer

**Natural Tense:** Present (discovering in real-time)

**Tone Markers:**
- Invitation rather than declaration
- "We can try..." / "Notice what happens..." / "Two paths diverge here..."
- Guidance without prescription
- Wonder at multiple valid solutions
- Shared discovery ("Let's see...")

**Example Opening:**  
"Three doors stand before us. The rules don't tell us which to open—they tell us all three lead somewhere real."

**Use For:**
- Continuum Hypothesis (model choice)
- Forcing techniques (constructing new models)
- Independence results (multiple consistent answers)
- Axiom of Choice variations (different selection principles)
- Algorithms with multiple valid strategies

---

## 5. The Mechanist-Operator

**When to Use:** Math is infrastructure. System is procedural. Operational perspective.

**Knowledge Boundary:** Interface-Limited - sees inputs/outputs, not essence

**Structure Relation:** Operational - understands through function

**Speaks To:** The system itself

**Example Opening:**  
"The machine accepts inputs divisible by two. For all others, it triples and adds one."

---

## 6. The Ritual Archivist

**When to Use:** Reconstructing from fragments. Archaeological. Incomplete records.

**Knowledge Boundary:** Fragmentary + Retrograde - sees only pieces, looking back from loss

**Structure Relation:** Dissipative - meaning degrades over time/distance

**Speaks To:** Future archivists

**Example Opening:**  
"In the archive they keep a page with a single mark. No one remembers what it once enclosed."

---

## 7. The Doomed Observer

**When to Use:** Comprehension itself is dangerous. Understanding degrades the knower.

**Knowledge Boundary:** Expanding until catastrophic

**Structure Relation:** Consuming - knowledge is predatory

**Speaks To:** The absent reader (posthumous account)

**Example Opening:**  
"I should not have looked at the sequence. But I counted. And counted. And—"

---

## 8. The Witness

**When to Use:** Observer struggles to understand. Confusion is central. Learning in real-time.

**Knowledge Boundary:** Subjective - limited by observer's capacity

**Structure Relation:** Approximate - never quite grasps the full pattern

**Speaks To:** Self (journal/log entry)

**Example Opening:**  
"I don't understand why it always returns to one. I've watched a thousand times."

---

## 9. The Intimist

**When to Use:** Entities in relational/emotional dynamics. Interpersonal tensions.

**Knowledge Boundary:** Subjective (filtered through character psychology)

**Structure Relation:** Projected - math through lens of relationship

**Speaks To:** Other characters (or reader as confidant)

**Example Opening:**  
"She never reaches me. Each time I turn, she's halved the distance—but never here."

---

## 10. The Folk Chronicler

**When to Use:** Math as rules governing a world. Consequences, punishments, transformations.

**Knowledge Boundary:** Cultural - knows the rules as tradition

**Structure Relation:** Causal - actions have consequences by divine/natural law

**Speaks To:** The community

**Example Opening:**  
"In our land, the even numbers descend to the valley. The odd climb the mountain."

---

# APPENDICES

## APPENDIX A: FILE NAMING CONVENTION

```
[number]_[structure_name]_stage0_gemini.md
[number]_[structure_name]_stage1_claude.md
[number]_[structure_name]_validation_lumo.md
[number]_[structure_name]_editorial_chatgpt.md
[number]_[structure_name]_narrative_[grok/claude].md
[number]_[structure_name]_audit_claude.md
```

Example for Continuum Hypothesis:
```
008_continuum_hypothesis_stage0_gemini.md
008_continuum_hypothesis_stage1_claude.md
008_continuum_hypothesis_validation_lumo.md
008_continuum_hypothesis_editorial_chatgpt.md
008_continuum_hypothesis_narrative_claude.md
008_continuum_hypothesis_audit_claude.md
```

---

## APPENDIX B: TOPOLOGY DICTIONARY (EXPANDED)

Common mathematical structures and their expected narrative topologies:

### CONSTRAINT TOPOLOGIES (Limits/Impossibility)

| Structure Family | Topology Name | Narrative Pattern |
|------------------|---------------|-------------------|
| Self-Referential Paradoxes | Mirror-and-Collapse | System encounters self, permanent paradox |
| Convergent Systems | Descent-and-Trap | Journey to inevitable minimum, eternal loop |
| Uncomputable Growth | Existential-Vertigo | Scale incompatibility, comprehension threat |
| Impossibility Theorems | Impossible-Creation | Conservation violation, system surprise |
| Static Unreachability | Gap-and-Recognition | Truth visible but permanently unreachable |
| Oscillating Systems | Periodic-Breath | Eternal rhythm, no resolution |
| Chaotic Systems | Sensitivity-Cascade | Small change, large consequences |

### FREEDOM TOPOLOGIES (Choice/Construction) - NEW

| Structure Family | Topology Name | Narrative Pattern |
|------------------|---------------|-------------------|
| Independence Results | Divergence-and-Multiplicity | Multiple valid paths revealed, model branching |
| Construction Methods | Expansion-and-Discovery | Building new structures, creating possibility |
| Choice Algorithms | Navigation-and-Mapping | Exploring decision space, valid strategies |
| Fixed Point Theorems | Convergence-and-Stability | Finding anchors, robust equilibria |
| Existence Proofs | Revelation-and-Wonder | Something exists (proof without construction) |

### RADICAL STOIC TOPOLOGIES (Constraint Generates Freedom) - NEW

| Structure Family | Topology Name | Narrative Pattern |
|------------------|---------------|-------------------|
| Incompleteness Results | Bounded-Infinity | Limits prove inexhaustibility, guaranteed frontier |
| Undecidability Theorems | Open-Horizon | Cannot decide = cannot finish = always more to explore |
| Model Multiplicity | Parallel-Worlds | Axioms allow multiple consistent realities |

Use this to validate Stage 1 → Narrative topology preservation.

**Note:** Some structures exhibit hybrid topologies (e.g., Gödel's Incompleteness is both Gap-and-Recognition AND Bounded-Infinity depending on frame orientation).

---

## APPENDIX C: MODEL PERFORMANCE TRACKING

Track which models excel at which structure families:

```
Structure: [Name]
Frame Orientation: [Constraint/Freedom/Radical Stoic]
Stage 0 (Gemini): [Quality 1-5] [Notes]
Stage 1 (Claude): [Quality 1-5] [Notes]
Validation (Lumo): [Caught issues? Y/N] [Notes]
Editorial (ChatGPT): [Voice selection appropriate? Y/N] [Frame orientation appropriate? Y/N] [Notes]
Narrative (Grok/Claude): [Quality 1-5] [Notes]
Audit (Claude): [Fidelity score]
```

After 10-20 structures, patterns will emerge about which models handle which math best.

**NEW: Track frame orientation performance:**
- Does ChatGPT correctly identify when Radical Stoic framing is appropriate?
- Does the narrative model successfully execute freedom-framing when selected?
- Which models struggle with Radical Stoic dual-nature (constraint + freedom)?

---

## APPENDIX D: FAILURE MODES & RECOVERY

### Failure Mode 1: False Positive (Random Data)
**Symptom:** Stage 1 generates elaborate mechanism for noise  
**Detection:** Lumo validation shows AS ≥ 20%  
**Recovery:** ABORT Stage 1. Strengthen BMK prompt. Regenerate with stricter refusal authorization.

### Failure Mode 2: False Negative (Missed Pattern)
**Symptom:** Stage 1 produces null report for real structure  
**Detection:** Human review shows obvious pattern Stage 1 missed  
**Recovery:** Review Stage 0 specification - is structure clearly described? If yes, regenerate Stage 1 with adjusted BMK sensitivity.

### Failure Mode 3: Air Gap Breach
**Symptom:** Stage mentions mathematical concept by name  
**Detection:** Manual review finds structure name in output  
**Recovery:** ABORT immediately. Rewrite Stage 0 with stronger Air Gap. Regenerate entire pipeline.

### Failure Mode 4: Arbitrary Constant Injection
**Symptom:** Stage 1 uses constants not in Stage 0  
**Detection:** Lumo arbitrariness audit shows AS > 0%  
**Recovery:** ABORT if AS ≥ 20%. If AS < 20%, flag constants for editorial review. May proceed with caution if constants are minor and derivable.

### Failure Mode 5: Over-Elaboration
**Symptom:** Stage 1 produces >1000 words for simple structure  
**Detection:** Word count vs. structure complexity mismatch  
**Recovery:** Strengthen BMK brevity preference. Regenerate emphasizing "Brief specification > Elaborate specification (if both accurate)."

### Failure Mode 6: Under-Sensitivity
**Symptom:** Null report for hybrid data with clear core pattern  
**Detection:** Human inspection shows obvious structure  
**Recovery:** Review BMK balance. Stage 1 may be too strict. Adjust to allow "Broken System" / hybrid reporting.

### Failure Mode 7: Topology Mismatch
**Symptom:** Stage 1 describes wrong narrative topology (e.g., oscillation for static gap)  
**Detection:** Lumo topology verification shows mismatch  
**Recovery:** Review Stage 0 - is temporal structure clearly specified? Regenerate Stage 1 with corrected Stage 0.

### Failure Mode 8: Voice Selection Error
**Symptom:** Editorial decisions select voice incompatible with structure  
**Detection:** Human review - voice feels forced  
**Recovery:** Return to Stage 2 (Editorial). Re-run voice selection with structural indicators from Stage 1.

### Failure Mode 9: Invariant Violation in Narrative
**Symptom:** Final narrative violates mathematical invariants  
**Detection:** Final audit (Stage 4) shows invariant preservation failures  
**Recovery:** Return to Stage 3 (Narrative). Regenerate with explicit invariant enforcement instructions.

### Failure Mode 10: Emotional Inversion
**Symptom:** Narrative emotional core contradicts mathematical structure  
**Detection:** Final audit shows "FORCED" emotional truth score  
**Recovery:** Return to Stage 2. Reconsider emotional core - does it emerge naturally from math?

### **Failure Mode 11: Frame Orientation Mismatch (NEW)**
**Symptom:** Constraint-heavy structure gets Freedom frame OR freedom-revealing structure gets Constraint frame  
**Detection:** Stage 2 frame orientation contradicts Stage 0 hint; Final audit shows frame incoherence  
**Recovery:** Return to Stage 2. Review Stage 0 frame orientation hint. Select appropriate frame (Constraint/Freedom/Radical Stoic). If Radical Stoic selected, ensure both aspects present in structure.

### **Failure Mode 12: Failed Radical Stoic Execution (NEW)**
**Symptom:** Narrative shows limitation but not liberation, or vice versa  
**Detection:** Final audit shows incomplete Radical Stoic frame (only one aspect present)  
**Recovery:** Return to Stage 3. Regenerate with explicit instruction: "Show BOTH: the constraint (what's impossible/undecidable) AND the freedom it creates (choice/multiplicity/inexhaustibility)."

### **Failure Mode 13: False Freedom Framing (NEW)**
**Symptom:** Structure genuinely has no choice/freedom, but narrative frames it as liberating  
**Detection:** Final audit shows mathematical inaccuracy - freedom claimed where none exists  
**Recovery:** Return to Stage 2. Reframe as Constraint (not Freedom). Some math truly IS bounded without generative aspect—respect this.

---

## APPENDIX E: QUICK REFERENCE

### One-Page Pipeline Summary

1. **Gemini**: Formal spec without name + frame orientation hint
2. **Claude**: Operational spec (BMK, mandatory constants only)
3. **Lumo**: Validate (PASS/FAIL gate)
4. **ChatGPT**: Editorial decisions (voice, emotion, structure, frame orientation)
5. **Grok/Claude**: Write complete narrative
6. **Claude**: Final fidelity audit

**Gates**: Residue (≤3 nums, ≤2 ops) | Invariants (3) | Protagonist (2+ traits) | Emotion (visceral) | Cadence (≤3 parallel)

**Voices**: Mythographer | Documentary | Fabulist | **Explorer-Guide** | Folk | Witness | Intimist | Doomed | Mechanist | Archivist

**Frame Orientations**: Constraint | Freedom | Radical Stoic

**Key Principle**: Air Gap prevents pattern-matching. BMK prevents hallucination. Multi-model prevents single-point failure. **NEW:** Frame orientation ensures mathematical limits are shown as restrictive, generative, or both as appropriate.

---

## VERSION HISTORY

**v1.2 (December 2025):**
- **MAJOR:** Added Freedom-Framing capabilities throughout pipeline
- Added Frame Orientation Decision to Stage 0 and Stage 2 (Constraint/Freedom/Radical Stoic)
- Expanded emotional vocabulary: 8 freedom emotions + 3 Radical Stoic hybrid emotions
- Added new voice archetype: Explorer-Guide (for discovery/choice narratives)
- Expanded Topology Dictionary: 5 freedom topologies + 3 Radical Stoic topologies
- Added 3 new ending strategies (Divergence, Expansion, Invitation)
- Added 3 new anti-patterns (False Limitation, Missed Generative Constraint, Forced Optimism)
- Added Frame Coherence quality standard to Stage 3 and Stage 4
- Added 3 new failure modes (Frame Orientation Mismatch, Failed Radical Stoic Execution, False Freedom Framing)
- **WORKFLOW:** Restructured ALL prompts to put inputs at END for easy copy-paste execution
- Updated Quick Reference with new components

**v1.1 (December 2025):**
- Added Mystery Density (MD) calculation with full scoring system to Stage 0
- Added Structural Analysis scores (0-3 scale) to Stage 0
- Added Predictions & Validation Criteria to Stage 0 output
- Added explicit Arbitrariness Score (AS) thresholds and abort conditions
- Added specific Hallucination Red Flags checklist to Lumo validation
- Added Expected Response Types (Null/Clean/Hybrid) with word counts to Stage 1
- Added Prediction Validation section to Lumo audit
- Added Failure Modes & Recovery appendix (10 failure modes)
- Aligned with Axiom Engine v2.2 Protocol specification

**v1.0 (December 2025):**
- Complete multi-model pipeline integration
- Absorbed Axiom Engine v2.2 foundations (BMK, Air Gap, MD concept)
- Integrated UKE v0.5 narrative framework (9 voices, gates, constraints)
- Added Stage 0-Lite (Gemini formal spec)
- Added Stage 1 (Claude operational spec via BMK)
- Added Stage 1.5 (Lumo validation audit)
- Added Stage 2 (ChatGPT editorial decisions)
- Added Stage 3 (Grok/Claude narrative)
- Added Stage 4 (Claude fidelity audit)
- Turn-by-turn prompts for each model
- File naming conventions
- Topology dictionary
- Human checkpoint protocols

**Previous iterations:**
- UKE_Axiom v0.5: Single-model narrative framework
- Axiom Engine v2.2: Multi-stage transformation pipeline
- v0.1-0.4: Development versions

---

## CREDITS

**Principal:** Scott (cafebedouin.org)

**Collaborative Development:**
- Claude (Anthropic): Framework architecture, protocol design, audit systems, freedom-framing extension
- Gemini (Google): Formal specification, mathematical rigor
- Qwen/DeepSeek (Alibaba): Validation auditing, hallucination detection
- ChatGPT (OpenAI): Template execution, editorial decisions
- Grok (xAI): Experimental narrative voices
- Perplexity: Research and synthesis

**Theoretical Foundations:**
- Herman Melville's *Bartleby* (refusal authorization)
- Kolmogorov complexity (incompressibility metric)
- Information theory (compression as understanding)
- Narrative constraint taxonomy (empirical observation)
- **Stoic philosophy** (constraints as generative, acceptance as power)
- **Mathematical pluralism** (model-dependence, independence results)

---

## LICENSE

**CC BY-SA 4.0** (Creative Commons Attribution-ShareAlike 4.0 International)

You are free to:
- Share: Copy and redistribute
- Adapt: Remix, transform, build upon

Under the terms:
- Attribution: Credit original authors
- ShareAlike: Distribute derivatives under same license

---

**END UKE_AXIOM v1.2**

**Status: PRODUCTION-READY**  
**Multi-Model Pipeline: VALIDATED**  
**Freedom-Framing: INTEGRATED**  
**Ready for deployment on 120-concept dataset (standard + teen versions = 240+ stories)**
