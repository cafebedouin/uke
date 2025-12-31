# 📖 UKE_Axiom v1.0 [Universal Knowledge Evaluator - Axiom Engine Narrative Translation]

**Version:** 1.0 (Production-Ready Multi-Model Pipeline)  
**Status:** Complete Multi-Model Workflow  
**Date:** December 2025  
**License:** CC BY-SA 4.0

---

## EXECUTIVE SUMMARY

UKE_Axiom v1.0 is a **multi-model orchestration pipeline** for translating mathematical structures into high-fidelity literary narratives. It combines:

1. **Axiom Engine v2.2** foundations (Air Gap Architecture, Bartleby Protocol, Mystery Density)
2. **UKE narrative framework** (9 Voices, Emotional Core, Invariant Preservation)
3. **Multi-model workflow** (Gemini → Claude → Lumo → ChatGPT → Grok/Claude)

**Core Innovation:** By distributing work across specialized models and enforcing validation gates between stages, the pipeline produces mathematically rigorous narratives while preventing abstraction drift and hallucination.

**Validated Capabilities:**
- Maintains Air Gap (prevents pattern-matching to training data)
- Detects and refuses hallucination (via BMK and Lumo validation)
- Preserves mathematical topology across narrative transformation
- Produces publication-quality literary fiction from pure mathematical structures

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
    ↓ [Voice, Emotional Core, Structure]
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
   ↓ [Voice, Naming, Emotional Core, Structure]
   
Turn 5: Grok OR Claude → Full Narrative
   ↓ [Based on voice selected in Turn 4]
   
Turn 6: Claude → Back-end Fidelity Audit
   ↓ [Final validation]
```

---

# STAGE 0-LITE: FORMAL SPECIFICATION

**Model:** Gemini  
**Purpose:** Generate rigorous mathematical specification while maintaining Air Gap

## Prompt Template

```
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

### Invariant 1: [Type]
[Statement of invariant]

### Invariant 2: [Type]  
[Statement of invariant]

### Invariant 3: [Type]
[Statement of invariant]

## Transformation Rules / Proof Structure
- Rule 1: [condition] → [action]
- Rule 2: [condition] → [action]
- Terminal Condition: [what happens at end]

## Epistemic Status
- Status: [Proven/Conjectured/Open]
- Known Properties: [list]
- Open Questions: [list if applicable]

## Structural Properties
- Regularity: [classification]
- Complexity: [Big-O if applicable]
- Temporal Structure: [classification]
```

## Human Validation Checklist

After Gemini produces Stage 0-Lite:

- [ ] Are there exactly 3 invariants?
- [ ] Are invariants mathematically correct?
- [ ] Is Air Gap maintained? (structure name not mentioned again)
- [ ] Are transformation rules complete?
- [ ] Are all constants mandatory (none arbitrary)?
- [ ] Is formal definition sufficient for Stage 1?

If all checked, save as: `[number]_[structure]_stage0_gemini.md`

---

# STAGE 1: OPERATIONAL SPECIFICATION

**Model:** Claude  
**Purpose:** Generate operational specification using Bartleby Protocol (BMK)

## Prompt Template

```
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
Operational Specification with:
- Transformation rules (step-by-step)
- Mandatory constants only
- Properties (convergence, periodicity, limits)
- Terminal conditions
- Verification that all 3 invariants are preserved

DO NOT:
- Add physical substrate (no voltage, circuits, gears - pure operations)
- Add narrative elements (no characters, conflicts, emotions)
- Introduce arbitrary numerical constants
- Explain "why" the mathematics works
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

Arbitrariness Score (AS): [arbitrary / total]

**CRITICAL:** If AS > 0, this indicates hallucination. Flag all arbitrary constants.

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

# STAGE 2: UKE EDITORIAL DECISIONS

**Model:** ChatGPT  
**Purpose:** Apply UKE_Axiom framework to determine voice, structure, and emotional core

## Prompt Template

```
You are applying the UKE_Axiom v1.0 Editorial Decisions framework.

INPUT: [Paste validated Stage 1 operational specification]

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

**Primary Emotion:** [single visceral word: dread, grief, claustrophobia, vertigo, awe, longing, resignation, horror]

NOT abstract concepts like "inevitability" or "complexity" - must be FELT emotion.

**Signature Image:** [one concrete image embodying this emotion]

**Anti-Emotions:** [2 emotions that would betray the math]
- Anti-emotion 1: [why it violates structure]
- Anti-emotion 2: [why it violates structure]

**Body Response:** How should reader's body respond? [e.g., "tight chest," "held breath," "urge to look away"]

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

## VOICE SELECTION

Use decision tree:

Is math eternal/timeless with archetypal roles? → Mythographer
Does pattern emerge surprisingly from simple rules? → Documentary Narrator  
Is paradox central and unresolvable? → Fabulist
Is math presented as operational infrastructure? → Mechanist-Operator
Are we reconstructing from fragments/archives? → Ritual Archivist
Is comprehension itself dangerous/degrading? → Doomed Observer
Is observer struggling to understand? → Witness
Are entities in relational/emotional dynamics? → Intimist
Is this about rules + punishment/transformation? → Folk Chronicler

**Selected Voice:** [name]

**Rationale:** [2-3 sentences citing structural indicators from Stage 1]

**Voice Attributes:**
- Knowledge Boundary: [Platonic/Procedural/Fragmentary/Interface-Limited/Subjective]
- Structure Relation: [Isomorphic/Analogical/Diffractive/Dissipative]
- Speaks To: [Universal/Reader/Self/System/Future archivist]
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

All editorial decisions complete. Ready for Turn 5 (Full Narrative).

**Recommended Model for Turn 5:**
- If Voice = [Mechanist-Operator, Doomed Observer] → Use Grok
- If Voice = [Mythographer, Fabulist, Intimist, Witness, Ritual Archivist] → Use Claude
- If Voice = [Documentary, Folk Chronicler] → Use ChatGPT or Claude

**Model Recommendation:** [Grok/Claude/ChatGPT]
```

## Human Review Checklist

After ChatGPT produces editorial decisions:

- [ ] Does voice selection match Stage 1's structural indicators?
- [ ] Is emotional core visceral (not abstract concept)?
- [ ] Are anti-emotions appropriate blockers?
- [ ] Is naming strategy clear?
- [ ] Are structural parameters justified?
- [ ] Does model recommendation make sense?

If all checked, save as: `[number]_[structure]_editorial_chatgpt.md`

Then proceed to Turn 5 with recommended model.

---

# STAGE 3: FULL NARRATIVE

**Model:** Grok OR Claude (based on Turn 4 recommendation)  
**Purpose:** Write complete narrative following all editorial decisions

## Prompt Template

```
You are writing a complete narrative following UKE_Axiom v1.0 framework.

INPUT MATERIALS:

1. OPERATIONAL SPECIFICATION (Stage 1):
[Paste Claude's validated Stage 1]

2. EDITORIAL DECISIONS (Stage 2):
[Paste ChatGPT's editorial decisions]

TASK: Write the complete story following ALL editorial decisions exactly.

---

## MANDATORY CONSTRAINTS

### From Gate Checks:
- Math Residue Budget: ≤3 explicit numbers, ≤2 named operations
- Protagonist Viability: Use only entities with desire/obstacle/agency/memory
- Emotional Core: SERVE [primary emotion] in every scene
- Emotional Core: VIOLATE [anti-emotion 1] and [anti-emotion 2]
- Cadence: Max 3 consecutive parallel iterations before compression

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

---

## STRUCTURE

### Opening Image (Max 100 words)
Concrete scene that establishes:
- Voice (sounds like selected voice)
- Tone (matches emotional core)
- Signature image (appears immediately)

### Full Narrative
Follow scene/summary balance from editorial decisions.
Dramatize key moments.
Compress repetitive elements.

### Ending
Execute selected ending strategy.
Leave reader with intended emotional residue.

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

---

BEGIN NARRATIVE:

[THE OPENING IMAGE]

[FULL NARRATIVE]
```

## Human Read-Through

After Grok/Claude produces narrative:

- [ ] Does opening image establish voice and emotional core?
- [ ] Is primary emotion present throughout?
- [ ] Are anti-emotions avoided?
- [ ] Do you sense the invariants without them being stated?
- [ ] Is voice consistent?
- [ ] Is math residue within budget?
- [ ] Does ending execute chosen strategy?
- [ ] Quality: Would you publish this?

If all checked, save as: `[number]_[structure]_narrative_[grok/claude].md`

Then proceed to Turn 6 (Final Audit)

---

# STAGE 4: FIDELITY AUDIT

**Model:** Claude  
**Purpose:** Validate final narrative preserves mathematical structure

## Prompt Template

```
You are conducting a comprehensive fidelity audit on a mathematical narrative.

INPUT MATERIALS:

1. STAGE 0 (FORMAL SPECIFICATION):
[Paste Gemini's Stage 0-Lite]

2. STAGE 1 (OPERATIONAL SPECIFICATION):
[Paste Claude's Stage 1]

3. EDITORIAL DECISIONS:
[Paste ChatGPT's editorial decisions]

4. FINAL NARRATIVE:
[Paste Grok/Claude's complete story]

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

Save audit as: `[number]_[structure]_audit_claude.md`

---

# COMPLETE WORKFLOW SUMMARY

```
Math Structure Name
    ↓
TURN 1: Gemini → Stage 0-Lite (Formal Specification)
    Human: Review invariants, check Air Gap
    Save: [number]_[structure]_stage0_gemini.md
    ↓
TURN 2: Claude → Stage 1 (Operational Specification via BMK)
    Human: Extract output, verify no arbitrary constants
    Save: [number]_[structure]_stage1_claude.md
    ↓
TURN 3: Lumo → Validation Audit
    Human: Check PASS/FAIL
    Save: [number]_[structure]_validation_lumo.md
    ↓
    If FAIL → Return to Turn 2
    If PASS → Continue
    ↓
TURN 4: ChatGPT → UKE Editorial Decisions
    Human: Review voice selection, emotional core
    Save: [number]_[structure]_editorial_chatgpt.md
    ↓
TURN 5: Grok OR Claude → Full Narrative
    Model selection based on voice
    Human: Read for quality
    Save: [number]_[structure]_narrative_[grok/claude].md
    ↓
TURN 6: Claude → Fidelity Audit
    Human: Review score, decide final status
    Save: [number]_[structure]_audit_claude.md
    ↓
COMPLETE
```

**Total Turns:** 6  
**Human Checkpoints:** 6  
**Time per Structure:** ~30-45 minutes  
**For 100 Structures:** ~50-75 hours (parallelizable)

---

# VOICE SELECTION MATRIX

## The Nine Voices

### Voice A: The Mythographer (Calvino, Le Guin, Gaiman)

**Structural Indicators:**
- Eternal patterns (cycles, recursion, infinities)
- Archetypal roles clearly defined
- Timeless quality (no specific time/place)
- Mathematical inevitability = fate/destiny

**Technical Markers:**
- Present tense, third-person omniscient
- Symbolic/archetypal naming
- Lyrical repetition for cycles
- No explanation, only observation
- Ritual cadence

**Best For:**
- Collatz (eternal descent + trap)
- Fixed-point theorems (destiny)
- Any convergent/cyclic system

**Knowledge Boundary:** Platonic (omniscient) - sees entire structure at once

**Example Opening:**  
"The Traveler begins at twenty-seven. Parity judges. Even: halve. Odd: triple, add one."

---

### Voice B: The Documentary Narrator (Herzog, Attenborough)

**Structural Indicators:**
- Emergent behavior from simple rules
- Observable phenomena requiring witness
- System complexity arising from interactions
- Wonder at natural-seeming order

**Technical Markers:**
- Past tense, observational distance
- Naturalistic detail
- Quiet revelation of complexity
- "What happens next is remarkable..."

**Best For:**
- Four Color Theorem
- Busy Beaver (uncomputable growth)
- Cellular automata
- Chaos theory

**Knowledge Boundary:** Procedural - discovers alongside reader

**Example Opening:**  
"In the beginning, fifty modules arranged themselves randomly. What happened next would reveal a hidden order."

---

### Voice C: The Fabulist (Borges, Barthelme, Lem)

**Structural Indicators:**
- Paradox requiring acceptance not resolution
- Self-referential structure
- Impossible objects/infinite libraries
- Precision about absurdity

**Technical Markers:**
- Dry, encyclopedic tone
- Catalog/library framing
- Acceptance of contradiction
- Footnotes, classifications, taxonomies

**Best For:**
- Gödel (self-referential statements)
- Banach-Tarski (paradoxical decomposition)
- Russell's Paradox
- Axiom of Choice consequences

**Knowledge Boundary:** Platonic but Broken - sees whole structure, knows it's impossible

**Example Opening:**  
"The Library contains a single question. The question asks: 'Can the Librarian answer this question?'"

---

### Voice D: The Folk Chronicler (Angela Carter, Kelly Link)

**Structural Indicators:**
- Repeating patterns = ritual/curse
- Rules with punishment/reward
- Oral tradition cadence
- Inevitability of folk tale logic

**Technical Markers:**
- "Once there was..." opening
- Rhythmic repetition
- Fairy tale causality
- Prophecy/curse framing

**Best For:**
- Halting Problem (riddle with no answer)
- Three-body problem (unstable fate)
- Game theory (promises and betrayals)

**Knowledge Boundary:** Oral - knows the ending, tells it anyway

**Example Opening:**  
"Once there was a number who angered the Judge."

---

### Voice E: The Witness (Sebald, Lydia Davis)

**Structural Indicators:**
- Personal encounter with abstraction
- Philosophical stakes
- Trying to understand = part of story
- Digressive, meditative

**Technical Markers:**
- First-person observer
- Essayistic flow
- Questions without answers
- Memory, documentation

**Best For:**
- Historical mathematical discoveries
- Incompleteness, undecidability
- Prime numbers (search for pattern)

**Knowledge Boundary:** Procedural + Limited - discovers step by step, often fails

**Example Opening:**  
"I first encountered the sequence in a margin note. What I didn't understand then was that I would never finish."

---

### Voice F: The Intimist (Literary Romance/Psychological Fiction)

**Structural Indicators:**
- Mathematical entities as relationship partners
- Internal states, desire, vulnerability
- Interpersonal dynamics drive plot
- Emotional stakes > logical stakes

**Technical Markers:**
- Close third-person or intimate first-person
- Interior monologue
- Relational language ("you," "we," "us")
- Emotional revelation as climax

**Best For:**
- Self-referential paradoxes (mutual definition = codependence)
- Convergent systems (attraction, inevitable union)
- Game theory (relationship equilibria)
- Fixed points (lovers who define each other)

**Knowledge Boundary:** Subjective - sees only what emotions reveal

**Example Opening:**  
"Cassandra could see every future except the one where Atlas stayed."

---

### Voice G: The Doomed Observer (Lovecraft, Ligotti, Laird Barron)

**Structural Indicators:**
- Scale incompatibility (math too vast for comprehension)
- Ontological threat (understanding destroys understander)
- Progressive degradation (narrator deteriorates)
- Indifference of system

**Technical Markers:**
- First-person descent into fragmentation
- Vocabulary of decay, wrongness
- Escalating inability to describe
- Terminal: silence, madness, dissolution

**Best For:**
- Uncomputable growth (Busy Beaver, Fast-Growing Hierarchy)
- Non-measurable sets
- Large cardinals
- Continuum Hypothesis

**Knowledge Boundary:** Procedural + Degrading - understands more, survives less

**Example Opening:**  
"I should not have calculated beyond n=7. The numbers leaked through the page, warping the margins."

---

### Voice H: The Mechanist-Operator (Pynchon, DeLillo, Gibson)

**Structural Indicators:**
- Systems as machinery, not myth or fate
- Characters embedded in procedural flows
- Emphasis on interfaces, signals, glitches
- Math as infrastructure

**Technical Markers:**
- Cool, clinical prose with sensory bursts
- Jargon used precisely but sparingly
- Fragmented pacing (state transitions)
- Characters monitor, maintain

**Best For:**
- Information theory (entropy, compression)
- Automata theory (FSM, Turing machines)
- Graph theory (network flows)
- Computational complexity (P vs NP, SAT)

**Knowledge Boundary:** Interface-Limited - sees dashboard, not depths

**Example Opening:**  
"The signal arrived at 03:17, a thin pulse threading through the static."

---

### Voice I: The Ritual Archivist (Anne Carson, Sjón, Sebald's poetic-documentary)

**Structural Indicators:**
- Math as ritual, liturgical fragment, archival artifact
- Narrative from scraps, marginalia, diagrams
- Story = attempt to preserve what resists preservation
- Reverent, brittle, haunted

**Technical Markers:**
- Hybrid prose: poetry + documentation
- Lists, fragments, redactions, lacunae
- Oscillates between cold record and lyrical invocation
- Ekphrastic description

**Best For:**
- Category theory (sacred correspondences)
- Topology (ritual transformations)
- Measure theory (what escapes counting)
- Prime numbers (prophetic sequence)
- Foundations (axioms as commandments)

**Knowledge Boundary:** Fragmentary + Retrograde - sees only pieces, looks back from loss

**Example Opening:**  
"In the archive they keep a page with a single mark. No one remembers what it once enclosed."

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

Example for Gödel's Incompleteness:
```
029_godels_incompleteness_stage0_gemini.md
029_godels_incompleteness_stage1_claude.md
029_godels_incompleteness_validation_lumo.md
029_godels_incompleteness_editorial_chatgpt.md
029_godels_incompleteness_narrative_claude.md
029_godels_incompleteness_audit_claude.md
```

---

## APPENDIX B: TOPOLOGY DICTIONARY

Common mathematical structures and their expected narrative topologies:

| Structure Family | Expected Topology | Narrative Pattern |
|------------------|-------------------|-------------------|
| Self-Referential Paradoxes | Mirror-and-Collapse | System encounters self, permanent paradox |
| Convergent Systems | Descent-and-Trap | Journey to inevitable minimum, eternal loop |
| Uncomputable Growth | Existential-Vertigo | Scale incompatibility, comprehension threat |
| Impossibility Theorems | Impossible-Creation | Conservation violation, system surprise |
| Static Unreachability | Gap-and-Recognition | Truth visible but permanently unreachable |
| Oscillating Systems | Periodic-Breath | Eternal rhythm, no resolution |
| Chaotic Systems | Sensitivity-Cascade | Small change, large consequences |

Use this to validate Stage 1 → Narrative topology preservation.

---

## APPENDIX C: MODEL PERFORMANCE TRACKING

Track which models excel at which structure families:

```
Structure: [Name]
Stage 0 (Gemini): [Quality 1-5] [Notes]
Stage 1 (Claude): [Quality 1-5] [Notes]
Validation (Lumo): [Caught issues? Y/N] [Notes]
Editorial (ChatGPT): [Voice selection appropriate? Y/N] [Notes]
Narrative (Grok/Claude): [Quality 1-5] [Notes]
Audit (Claude): [Fidelity score]
```

After 10-20 structures, patterns will emerge about which models handle which math best.

---

## APPENDIX D: QUICK REFERENCE

### One-Page Pipeline Summary

1. **Gemini**: Formal spec without name
2. **Claude**: Operational spec (BMK, mandatory constants only)
3. **Lumo**: Validate (PASS/FAIL gate)
4. **ChatGPT**: Editorial decisions (voice, emotion, structure)
5. **Grok/Claude**: Write complete narrative
6. **Claude**: Final fidelity audit

**Gates**: Residue (≤3 nums, ≤2 ops) | Invariants (3) | Protagonist (2+ traits) | Emotion (visceral) | Cadence (≤3 parallel)

**Voices**: Mythographer | Documentary | Fabulist | Folk | Witness | Intimist | Doomed | Mechanist | Archivist

**Key Principle**: Air Gap prevents pattern-matching. BMK prevents hallucination. Multi-model prevents single-point failure.

---

## VERSION HISTORY

**v1.0 (December 2025):**
- Complete multi-model pipeline integration
- Absorbed Axiom Engine v2.2 foundations (BMK, Air Gap, MD)
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
- Claude (Anthropic): Framework architecture, protocol design, audit systems
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

**END UKE_AXIOM v1.0**

**Status: PRODUCTION-READY**  
**Multi-Model Pipeline: VALIDATED**  
**Ready for deployment on 100-structure dataset**
