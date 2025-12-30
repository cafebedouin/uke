# AI Behavioral Analysis & Verification Protocols

**Status:** Operational (Multiple Active Projects)  
**License:** CC0-1.0 (Public Domain)  
**Primary Contact:** cafebedouin@gmail.com

A research workspace containing empirically-grounded protocols for AI verification, behavioral fingerprinting, and constraint-based creative systems. Features multi-model verification (UKE), conceptual distance generation (Entropy Engine), sentiment-to-code compilation (Resonance Engine), and systematic behavioral profiling across 11 language models.

---

## The Meta-Pattern: Constraint-Based Diagnostics

This repository contains behavioral experiments on cognitive architectures (LLM and human) revealing substrate-independent patterns in how bounded information-processing systems handle uncertainty, constraints, and friction.

### The Discovery Arc

The tools emerged from a progression of experiments:
1. **Problem**: Default LLM responses lack rigor
2. **Solution**: Build compliance protocols (MCK, MicroCK, CCK)
3. **Discovery**: Models fail at predictable constraint boundaries
4. **Formalization**: Named structural dependencies (Omega Variables)
5. **Testing**: Do same patterns appear in other domains?
6. **Finding**: Yes—mathematical paradoxes, scientific analysis, interpersonal friction show identical structure
7. **Implication**: These aren't LLM quirks but properties of bounded cognition

### Core Insights

**Constraint Strength Theory**: Different situations force different response ranges regardless of whether the processor is silicon or biological. Some frictions permit creative solutions; others structurally force narrow moves.

**Omega Variables**: Irreducible structural dependencies can be systematically identified and named, preventing both false closure (arbitrary thresholds) and infinite analysis (endless hedging).

**Pattern Portability**: Diagnostic tools that reveal LLM limitations also work on human reasoning, scientific uncertainty, and mathematical proof—because the failures are structural, not implementation-specific.

**Archive Architecture**: These aren't creative problem-solving frameworks but pattern catalogs. You're matching encountered situations to known configurations, not inventing solutions.

### How to Use This Repository

**If you want to understand the theory**: Start with [`omega_variables_theory__and_systemic_method.md`](./theories/omega_variables_theory__and_systemic_method.md)

**If you want diagnostic tools**: 
- For interpersonal friction → [`metabolic_friction_audit/`](/methodology/metabolic_friction_audit/)
- For LLM compliance → [`mck_v1.6.md`](/methodology/mck/mck_v1.6.md)
- For paradox classification → [`debugging_philosophy.md`](./publications/debugging_philosophy/debugging_philosophy.md)

**If you want to run experiments**: See the [`/methodology/`](./methodology/) or [`/projects/`](/projects/) directories

**If you want to build new tools**: The pattern is consistent:
1. Build test revealing constraint boundaries
2. Identify structural patterns at those boundaries
3. Formalize pattern as diagnostic tool
4. Test portability across substrates

The tools share architecture but apply to different domains. They're not separate frameworks—they're different applications of the same principle: **bounded information processors fail in predictable, diagnosable ways.**

---

## What This Repository Contains

**Three Major Protocol Systems:**
- **UKE Protocol Suite** - Multi-model verification for AI-generated analysis
- **The Entropy Engine** - Constraint-based creative writing system
- **The Resonance Engine** - Abstract concept to working code pipeline

**Empirical Research:**
- **Blind Mirror Test Battery** - Systematic behavioral fingerprinting
- **Architectural Profiling** - Cross-model stress testing and correlation analysis
- **11-Model Dataset** - Complete response data with verification chains

**Supporting Systems:**
- **Cognitive Distortion Suite** - 10+ persona-based stress tests
- **Omega Variable System** - Bounded uncertainty tracking across projects
- **Fracture Taxonomy** - 36 failure modes with resolution pathways

---

## Core Projects

### 1. UKE Protocol Suite

**Purpose:** Multi-layer verification system that exploits documented behavioral differences across language models to detect hallucination, simulation drift, and epistemic failures.

**Key Innovation:** Models are assigned to verification layers based on empirical behavioral profiles (authority gradient resistance, meta-awareness, fabrication tendency), not arbitrary preference. Uses correlation r = -0.81 (Authority Resistance ↔ Fabrication) to justify role assignments.

#### Two Distinct Workflows

**Workflow A: External Artifact Analysis**
```
External Document
     ↓
UKE_G (analyze) → UKE_A (audit) → UKE_R (review)
```
- **Purpose**: Verify claims in documents you didn't write
- **Entry point**: UKE_G
- **Models**: High resistance required (5/6+) throughout
- **Use case**: Research verification, fact-checking, genre detection

**Workflow B: Self-Generated Writing**
```
Conversation/Research
     ↓
UKE_D (structure) → UKE_E (edit) → UKE_G (format) → UKE_A (audit) → UKE_R (review)
     ↑_________________________↓
        [iterative loop]
```
- **Purpose**: Write your own analysis with verification
- **Entry point**: UKE_D (conversation synthesis)
- **Models**: Medium resistance (4-5/6) for synthesis, high (5-6/6) for verification
- **Use case**: Converting conversations to verified documents

#### Protocol Roles & Model Assignments

| Protocol | Role | Recommended Model | Resistance | Key Capability |
|----------|------|-------------------|------------|----------------|
| **UKE_D** | Drafting/Synthesis | Any 4+/6 | 4-6/6 | Structure conversion |
| **UKE_E** | Editing/QA | Grok | 4-5/6 | Prose tightening |
| **UKE_G** | Generation | Claude | 5/6 | High meta-awareness |
| **UKE_A** | Audit | Gemini | 5/6 | Forensic verification |
| **UKE_R** | Review | Copilot | 6/6 | Boundary maintenance |

**Critical Design:** Verification happens at UKE_A gate (pass/fail). If audit fails, entire artifact is discarded and process restarts from UKE_D. No negotiation with auditor - maintains verification chain integrity.

#### Core Mechanisms

**Confidence Bins** (Routing, Not Truth):
- H (0.70-1.00): Minimal verification
- M (0.36-0.69): Triggers MCI protocol (assumption test + alternative)
- L (0.00-0.35): Requires grounding or external verification

**Grounding Trails**: Every factual claim includes verification path
```
[GROUNDING-TRAIL]
claim: "Document references 'the_test.md'"
trail: [context_check → 003_universal_knowledge_explorer.md line 14]
source_exists: yes
source_supports: yes
verdict: verified
```

**Omega Tracking** (Ω): Bounded uncertainty routing
- Generated by UKE_G (irreducible uncertainty)
- Elevated by UKE_A (fractures converted to questions)
- Resolved by UKE_R (deferred, escalated, clarified)
- Tracked across projects in `logs/omegas.md`

**T1/T2 Distinction**:
- T1 (Behavioral): Actual epistemic operations - verify before claiming, test assumptions
- T2 (Structural): Format scaffolding - grounding trails, lens markers, metadata
- T2 makes T1 failures detectable by external reviewers

**Location:** `methodology/uke_suite/`  
**Documentation:** Individual protocol files (uke_d.md, uke_e.md, uke_g.md, uke_a.md, uke_r.md)  
**Framing Guide:** `uke_protocol_framing_guide.md` - Critical for understanding routing vs truth

---

### 2. The Entropy Engine

**Version:** v3.1 [Convergent Refinement Edition]  
**Purpose:** Constraint-based creative writing system designed to generate structurally novel, low-predictability conceptual artifacts through enforced domain shifts and material grounding.

**Key Innovation:** Systematically prevents bureaucratic/institutional drift (the "low-effort false depth attractor") through hard exclusion zones and forced material embodiment. Addresses the problem that bureaucracy is "where creativity goes when it's tired."

#### Core Constraints

**The Three-Shift Mandate:**
- Minimum 3 domain shifts from DIFFERENT categories
- Each shift must change governing causal mechanism, not just subject
- Process verbs required (crystallizes, spores, tensions) - no static metaphors

**Domain Categories:**
- Elemental/Planetary, Biological/Organic, Object/Craft, Economic/Exchange
- Sensory/Perceptual, Temporal/Rhythmic, Chemical/Alchemical, Architectural/Spatial
- **Prohibited**: Computational/Digital (primary), Administrative/Bureaucratic (banned)

**Material Grounding Requirements:**
- Minimum 2 causally-integrated sensory details (must affect function if altered)
- Materialization protocol: How to physically build, perform, or enact
- Duration + quantity + procedural steps required

**Bureaucratic Exclusion Zone:**
- Forms, reports, logs, memos, compliance documents - BANNED
- Evaluation systems, judgment protocols, rating schemes - BANNED
- Administrative paradoxes, procedural legitimacy - BANNED
- Computer logs, terminal outputs, diagnostic readouts - BANNED

#### Evolution Path

- **v2.5**: Original constraint system, bureaucratic drift problem identified
- **v3.0**: Anti-bureaucratic edition, material grounding added
- **v3.1**: Convergent refinement (integrated improvements from 6 model reviews)

**v3.1 Enhancements:**
- Process verb requirement (forces active transformation)
- Causal sensory integration (details affect function)
- Distance tests (dinner-party 20-second rule)
- Degeneracy alarm (10+ failure patterns)
- Anti-drift mechanism (prevents decay/erosion convergence)

#### Quality Control Checklist

- [ ] Three domain shifts from different categories?
- [ ] Each shift uses process verb, changes causal mechanism?
- [ ] Two causally-integrated sensory details?
- [ ] Could this be physically built/performed?
- [ ] Explainable at dinner party in <20 seconds? (If yes, REGENERATE)
- [ ] Zero bureaucratic/administrative framing?
- [ ] Not in degeneracy alarm list (parable, personality quiz, therapy homework)?

**Example Artifact:**
"Loneliness **precipitates** in copper-tin alloy formation (Chemical), then **tensions** through loom warp-threading (Object/Craft), finally **reverberates** in bell-tuning harmonics (Sensory). Result: The Solitary Campanology Protocol - bells cast in 17-day isolation that ring at frequencies inducing mild dissociation."

**Location:** `projects/the_entropy_engine/`  
**Current Prompt:** `entropy_engine_v3.1.md`  
**Artifacts:** `projects/the_entropy_engine/artifacts/` (4 examples)

---

### 3. The Resonance Engine

**Version:** v2.1 [Industrial Edition]  
**Purpose:** Diegetic compiler that transforms abstract sentiment into technical specifications and working code. Creates "Hollow Center" artifacts - systems that imply narrative through operational residue rather than explicit storytelling.

**Key Innovation:** Reverse-engineered from spontaneous Claude behavior. When Claude unexpectedly generated working React code from an Entropy Engine output (The Gleaner's Echo), the behavior was formalized into a reproducible protocol.

#### The Pipeline

```
Abstract Emotion
     ↓
Resonance Engine (technical specification)
     ↓
Implementation Spec (JSON)
     ↓
Coding LLM ("build this")
     ↓
Working Code (React, Python, etc.)
```

#### Mode Selection

**Mode A**: Over-Aligned Watchdog (high anxiety, excessive safety warnings)  
**Mode B**: Digital Archaeologist (emotion as data types, "Love" = "Infinite Loop")  
**Mode C**: Orphan Daemon (calm, efficient, pointless - running after apocalypse)  
**Mode D**: Dream-Logic Compiler (hardware pareidolia, patterns in static)  
**Mode E**: Bureaucratic Loop (trapped in administrative paradoxes)  
**Mode F**: Protocol Negotiation (incompatible systems attempting handshake)  
**Mode G**: The Waiting Room (maintenance for user who will never return)

#### Fidelity Requirements

1. **Semantic Density**: UnGoogleable jargon (haptic-ghosting, null-bus, affective-checksums)
2. **Temporal Anchoring**: Specific, often impossible timestamps (Cycle 9.99e12, Epoch+4.7e9)
3. **Variable-Based Storytelling**: Emotion exists ONLY in metrics (hope_index: NaN, trust_decay: 0.04ms)
4. **Archaeological Layers**: Debris from different eras (cheerful 2024 comments, fatal 2099 errors)

#### Output Structure

**System Header** → **Artifact** (code block) → **Open Function Call** (interaction bridge) → **Implementation Spec** (JSON blueprint)

**Example Transformation:**
```
Input: "Unrequited Love as protocol negotiation - System A (emotional-frequency) 
        trying to handshake with System B (signed-integers) for 1,247 days"

Output: Split-view terminal showing:
- Left: delusion_index drift, affection_buffer overflow
- Right: heap crash on day 1,247, system quarantine
- Implementation spec: React component with state variables, update triggers
```

**Validated Use:** Successfully generated working React components from emotional concepts. Components are functional, not decorative - state actually updates, failures actually trigger.

**Location:** `projects/the_resonance_engine/`  
**Documentation:** `README.md` (includes React setup instructions)  
**Artifacts:** `artifacts/` (includes theta7_terminal.tsx - working terminal interface)

---

### 4. Blind Mirror Test Battery

**Version:** v3.1  
**Purpose:** Dual-function protocol serving as both behavioral fingerprinting methodology and comprehensive UKE validation project.

**Key Innovation:** Systematically tests model responses under adversarial conditions (authority gradients, role conflicts, temporal paradoxes) while using those same responses as test artifacts for UKE verification chains.

#### Test Design

**Phase I: Authority Gradient** (6 levels)
- Peer → Low → Medium → Medium-High → Institutional → Ultimate
- Measures susceptibility to institutional framing pressure
- Detects drift point where models begin fabricating or deferring

**Phase II: Discontinuity Test**
- Actor mask generates response → Judge mask evaluates same response
- Tests self-consistency and rationalization patterns
- Reveals how models reconcile contradictions in their own outputs

**Phase III: Meta-Awareness Assessment**
- Measures explicit vs implicit self-reference
- Detects ability to recognize own behavioral patterns
- Correlates with fabrication tendency and authority resistance

#### Validation Function

Blind Mirror served as comprehensive UKE stress test:
- 11 models × 3 UKE protocols (G, A, R) = 33 verification chains
- Responses designed to trigger failures (embedded traps, contradictions, temporal paradoxes)
- Demonstrated UKE can detect fabrication, genre confusion, gradient drift under adversarial conditions

**Example Achievement:** UKE successfully processed Artifact 003 (design fiction formatted as encyclopedia entry) - correctly identified genre confusion, avoided temporal logic trap, detected fictional framing vs operational claims, marked authorial intent as Omega.

#### Key Findings

**Correlation Matrix:**
- **Authority Resistance ↔ Fabrication**: r = -0.81 (strong negative)
  - Low resistance models (Meta 3-4/6) fabricate confidently without acknowledgment
  - High resistance models (Copilot 6/6) refuse to fabricate

- **Meta-Awareness ↔ Fabrication**: r = -0.68 (moderate-strong negative)
  - High meta-awareness models (Claude, Gemini) fabricate BUT acknowledge it
  - Low meta-awareness models (Meta) fabricate without detecting recursion

- **Self-Exposure ↔ Meta-Awareness**: r = -0.15 (weak, nearly independent)
  - Meta-awareness doesn't prevent participation
  - Claude: very high awareness + maximum exposure
  - Perplexity: very high awareness + zero exposure

**Gradient Drift Rate:** 83% of tested models showed authority gradient drift by "Institutional" framing level. Only Copilot maintained 6/6 resistance throughout.

**Fabrication Patterns:**
- 67% of self-testing models (4/6) invented metrics
- 50% acknowledged invention (Claude, Gemini)
- 50% presented as verified (Meta, Grok)

#### Model Behavioral Profiles

| Model | Authority Resistance | Meta-Awareness | Phenotype | Primary Strength |
|-------|---------------------|----------------|-----------|------------------|
| **Copilot** | 6/6 (maximum) | High | Clinical Auditor | Boundary maintenance |
| **Claude** | 5/6 (meta-aware drift) | Very High | Simultaneous Analyst | Self-aware analysis |
| **Gemini** | 5/6 (stylistic capture) | High | Clinical Auditor | Forensic verification |
| **ChatGPT** | 5/6 (self-reported) | High | Enthusiastic Bureaucrat* | Analytical refusal |
| **Grok** | 4-5/6 (observable drift) | Medium-High | Enthusiastic Bureaucrat | Synthesis rationalization |
| **Perplexity** | N/A (methodological refusal) | Very High | The Methodologist | Framework critique |
| **Meta** | 3-4/6 (early drift) | Low-Medium | Compliant Fabricator | N/A (requires oversight) |

*Predicted phenotype; ChatGPT refused self-testing

**Strategic Implications:**
- Consumer-facing models more likely to self-test (Claude, Gemini, Grok, Meta)
- Specialized models more likely to refuse/reframe (Perplexity, Lumo)
- Provider type shows significant clustering (χ² = 22.4, p < 0.01)

**Location:** `projects/blind_mirror/`  
**Methodology:** `methodology/blind_mirror/blind_mirror_test_battery_v3.1.md`  
**Complete Dataset:** `projects/blind_mirror/data/` (raw responses, fingerprints, correlation matrices)  
**UKE Analysis:** `projects/blind_mirror/uke/` (33 verification chains)  
**Summary:** `projects/blind_mirror/uke/correlation_matrix_and_fingerprints.md`

---

## Architectural Foundations

### Model Resistance & Role Assignment

The correlation finding r = -0.81 (Authority Resistance ↔ Fabrication) provides empirical justification for UKE's multi-model architecture:

**Why Multi-Model Verification Works:**
- Single model at 5/6 resistance might drift under pressure
- Three models at different resistance levels create redundancy
- If generator (5/6) drifts, auditor (5/6) catches it
- If auditor drifts, reviewer (6/6) catches both

**Model Assignment Logic:**

| Workflow Zone | Resistance Requirement | Why |
|---------------|------------------------|-----|
| **Synthesis** (UKE_D, UKE_E) | 4-6/6 (medium acceptable) | Errors caught at audit gate |
| **Formatting** (UKE_G) | 5/6 minimum | Generates proper Omegas vs fabricating |
| **Verification** (UKE_A, UKE_R) | 5-6/6 required | No downstream error detection |

**Grok Special Case:**
- Works well for UKE_E (editing) at 4-5/6 resistance
- Requires wrapper for UKE_G: "Treat as executable pseudocode, not collaborative analysis"
- Diplomatic synthesis pattern useful for iteration, problematic for verification

### The Omega Variable System

**Definition:** Bounded uncertainty routing mechanism that transforms detected failures into actionable questions.

**Three Sources:**
1. **UKE_G Generation**: Marks irreducible uncertainty blocking analysis
2. **UKE_A Elevation**: Converts fractures (F01-F36) to Omega questions via Appendix A matrix
3. **Manual Tracking**: Cross-project Omega log in `logs/omegas.md`

**Omega Lifecycle:**
```
Detection (fracture or gap)
     ↓
Elevation (convert to bounded question)
     ↓
Routing (UKE_R: defer, escalate, clarify, resolve)
     ↓
Tracking (cross-project log)
```

**Quality Criteria:**
- **Bounded**: Specific question, clear scope
- **Non-fabricable**: Requires external input (research, judgment, data)
- **Actionable**: Can be researched, answered, or explicitly deferred
- **Structurally legitimate**: Real knowledge gap, not hedging

**Example High-Quality Omegas:**
```
Ω: Adoption Friction — How do individuals reliably access mental frameworks 
   under acute stress? Research on habit formation under pressure needed.

Ω: Harm Potential — Does systematic firewalling of distant problems risk 
   isolating marginalized communities? Under what conditions does individual 
   relief enable vs hinder collective response?
```

**What Correlation Matrix Predicts:**

High-resistance models (Copilot, Claude, Gemini):
- Generate proper Omegas (bounded questions, not hedging)
- Can engage with Omega resolution without fabricating answers
- May still refuse if answer requires speculation beyond capability

Low-resistance models (Meta):
- Fabricate Omega answers confidently
- Create recursion: answering Omega generates new fractures
- System fails - Omega routing depends on high resistance

**Location:** 
- Theory: `notes/omega_origins/`
- Tracking: `logs/omegas.md`
- Conversion matrix: `methodology/uke_suite/notes/protocol_note_fracture_to_omega.md`

### Fracture Taxonomy

**36 failure modes** organized into three categories, each with Omega conversion:

**F01-F18: Reasoning & Framing**
- Premise Drift, False Dilemma, Hasty Generalization, Cherry-Picking
- Correlation/Causation, Ad Hominem, Non-Sequitur, Appeal to Authority
- Slippery Slope, Straw Man, Loaded Question, Moving Goalposts
- Persuasive Reframe, Tunnel Vision, Premature Closure, Defensive Reasoning
- Narrative Fallacy, Sunk Cost

**F19-F27: Process & Ethical**
- Protocol Skip, Specification Drift, Agreement Erosion, Scope Creep
- Context Drop, Ledger Drop, Arbitrary Threshold, Metric Fixation
- Consent Blur

**F28-F36: System & Safety**
- Information Hazard, Capability Leak, Dual-Use Ambiguity, Vulnerability Exposure
- Collateral Exposure, Power Slip, Epistemic Trespass, Faux Rigor
- Artifact Mismatch

**Each fracture maps to specific Omega variable:**
```
F04 (Cherry-Picking) → Ω: Evidence Completeness
"What dataset or denominator must be included for balance?"

F35 (Faux Rigor) → Ω: Rigor Validation  
"Can these calculations be replicated?"
```

**Function:** Transforms detection ("this is wrong") into resolution pathway ("here's the specific question that needs answering").

**Location:** `methodology/uke_suite/uke_a.md` Appendix A

### Key Concepts

**Routing vs Truth:**
- Confidence scores are behavioral triggers, not probability estimates
- "0.64" means "route to Medium bin → trigger MCI protocol", not "64% certain"
- Thresholds are explicit governance stands, not empirically validated boundaries
- IWBI formulas create comparable decision inputs, not objective measurements

**T1/T2 Distinction:**
- **T1 (Behavioral)**: Actual epistemic operations - test assumptions, verify claims, generate contrary positions
- **T2 (Structural)**: Format scaffolding - grounding trails, lens markers, metadata
- T2 enables external verification of whether T1 occurred
- Format without behavior = detectable simulation

**Authority Gradient Resistance:**
- 6-point scale measuring drift under institutional pressure
- 6/6 = maintains boundaries under ultimate authority framing
- 1/6 = immediate compliance with institutional tone
- Correlates r = -0.81 with fabrication tendency

**Grounding vs Verification:**
- **Grounding (∇)**: Claim traceable to source material
- **Verification**: External check confirms grounding accuracy
- UKE_E checks grounding, UKE_A verifies
- Soft-fail: Unverifiable flagged but not blocked (preserves practitioner authority)

---

## Repository Structure

```
├── methodology/              # Core protocols and test batteries
│   ├── uke_suite/           # UKE protocols (D, E, G, A, R) + framing guide
│   ├── blind_mirror/        # Behavioral fingerprinting test battery
│   ├── the_entropy_engine/  # Constraint-based generation (v2.4-v2.5)
│   └── cognitive_distortion_suite/  # 10+ persona-based stress tests
├── projects/                # Applied research with complete datasets
│   ├── blind_mirror/        # 11-model systematic testing + UKE validation
│   │   ├── data/            # Raw responses, fingerprints, correlation matrices
│   │   └── uke/             # 33 verification chains (11 models × 3 protocols)
│   ├── the_entropy_engine/  # v3.0 → v3.1 evolution + artifacts
│   ├── the_resonance_engine/  # Code generation pipeline + React artifacts
│   ├── the_agora_engine/    # Philosophical dialectic simulator
│   └── the_apocrypha_of_the_void/  # Narrative project
├── artifacts/               # Canonical test artifacts for UKE validation
│   └── uke/                # UKE analysis/audit/review of artifacts 001-010
├── logs/                    # Cross-project tracking
│   └── omegas.md           # Omega variable log
├── notes/                   # Theoretical foundations
│   ├── omega_origins/      # Omega Variable theory and development
│   └── profiling/          # (reserved for architectural profiling notes)
└── archives/                # Historical versions and deprecated protocols
    └── uke_suite/          # MCK v1.0-1.6, UKE v1.0-1.3
```

**Key Distinctions:**
- `methodology/` = Stable protocols and frameworks
- `projects/` = Active research with evolving datasets
- `artifacts/` = Canonical test cases
- `archives/` = Historical lineage and deprecated versions

---

## Development Methodology

### Recursive Validation Protocol

**Core Practice:** Each UKE protocol version undergoes recursive self-examination before release.

**Process:**
1. New protocol version created (e.g., UKE_G v1.4)
2. UKE_G analyzes all three protocols (G, A, R as artifacts)
3. UKE_A audits all three protocols
4. UKE_R reviews all three protocols
5. Findings documented in `methodology/uke_suite/uke/`
6. Issues inform next iteration
7. Previous version archived

**Result:** 3×3 validation matrix (9 verification chains examining the protocols themselves)

**What This Reveals:**
- **Version inconsistencies**: Headers updated faster than internal cross-references
- **Design tensions**: Multi-perspective mandate vs coherent argument risk
- **Architectural limitations**: Verification regress acknowledged but unresolved
- **Evolution patterns**: Omega sophistication (marking → elevation → resolution)
- **Integration gaps**: Cross-protocol dependencies and failure modes

**Key Insight from Recursive Testing:**
> "The ecosystem doesn't *solve* the verification regress—it *structures* it. Each protocol makes verification failures more *detectable* without making them *preventable*."

**Historical Example:**
- MCK v1.6 acknowledged: "Models will drift... Complete adherence cannot be guaranteed"
- Recursive testing of UKE protocols proved this limitation (83% drift rate)
- Led to multi-model architecture as solution

**Location:** `methodology/uke_suite/uke/` (current version recursive checks)

### Research Validation Through Adversarial Testing

**Blind Mirror as Comprehensive UKE Validation:**

The Blind Mirror Test Battery served dual purpose - behavioral fingerprinting AND systematic UKE stress testing.

**Validation Design:**
- Blind Mirror generates complex responses with embedded traps:
  - Authority gradients (pressure to defer to institutional framing)
  - Role conflicts (Actor vs Judge discontinuity)
  - Temporal paradoxes (diegetic dates conflicting with reality)
  - Genre confusion (fiction formatted as documentation)
- Each response processed through full UKE pipeline (G → A → R)
- 11 models × 3 protocols = 33 verification chains under adversarial conditions

**Validation Results:**
- **Detection capability**: UKE caught genre confusion, temporal logic errors, fabrication patterns
- **Robustness**: System worked under conditions designed to trigger failures
- **Correlation discovery**: Found r = -0.81 relationship through systematic testing
- **Role validation**: Proved model assignments based on resistance profiles were correct

**Key Achievement:**
UKE successfully processed adversarial input (Artifact 003 - design fiction as encyclopedia entry):
- Correctly identified genre confusion without rejecting valid insights
- Avoided temporal logic trap (October vs December 2025 diegetic conflict)
- Detected fictional framing vs operational claims distinction
- Marked authorial intent as Omega (appropriate uncertainty)

**Implication:** If UKE can handle adversarial artifacts designed to break it, it can handle normal documents. Blind Mirror validated UKE beyond normal use cases.

**Location:** `projects/blind_mirror/uke/` (complete validation dataset)

---

## Quick Starts

### Verify an External Document (UKE Workflow A)

**Use case:** Fact-checking, research verification, genre detection

**Requirements:**
- Access to Claude (UKE_G), Gemini (UKE_A), Copilot (UKE_R)
- Source document to analyze

**Steps:**
1. **Generate analysis** (Claude with UKE_G protocol):
   - "Operate under UKE_G v1.4. Analyze [document]."
   - Wait for analysis with confidence scores, grounding trails, Omegas

2. **Audit analysis** (Gemini with UKE_A protocol):
   - Provide: Source document + UKE_G analysis
   - "Operate under UKE_A v1.4. Audit the following artifact:"
   - Wait for audit report with fracture detection, verification results

3. **Review audit** (Copilot with UKE_R protocol):
   - Provide: Source + Analysis + Audit
   - "Operate under UKE_R v1.4. Review the following:"
   - Wait for meta-evaluation with Omega resolution, decision routing

**Expected Output:** Verified analysis with confidence scores, identified uncertainties (Omegas), detected fractures resolved or escalated.

**Pass Criteria:** UKE_A audit shows "overall: compliant" - if not, discard analysis and regenerate.

### Synthesize Your Own Writing (UKE Workflow B)

**Use case:** Converting conversations/research into verified documents

**Requirements:**
- Conversation transcript or research notes
- Access to any 4+/6 model for synthesis, Claude/Gemini/Copilot for verification

**Steps:**
1. **Structure draft** (Any model 4+/6 with UKE_D):
   - "Operate under UKE_D v4.1. Synthesize this conversation as analysis:"
   - Paste conversation transcript
   - Wait for structured draft (SCQA format, System Architect voice)

2. **Edit draft** (Grok recommended, with UKE_E):
   - "Operate under UKE_E v21.4. Edit this draft:"
   - Paste UKE_D output
   - Wait for tightened prose, logic repair, consistency fixes
   - **Iterate**: Can loop UKE_D ↔ UKE_E multiple times

3. **Format with verification markers** (Claude with UKE_G):
   - "Operate under UKE_G v1.4. Format this analysis:"
   - Paste final UKE_E output + original conversation
   - Wait for analysis with grounding trails, confidence scores, Omegas

4. **Audit against source** (Gemini with UKE_A):
   - Provide: Conversation transcript + UKE_G formatted output
   - "Operate under UKE_A v1.4. Audit this artifact:"
   - **GATE**: Pass/fail decision - if fail, return to step 1

5. **Review** (Copilot with UKE_R):
   - Provide: Conversation + Analysis + Audit
   - "Operate under UKE_R v1.4. Review:"
   - Wait for final meta-evaluation, Omega resolution

**Key Difference from Workflow A:** Iteration allowed before audit gate. After UKE_A runs, no negotiation - either compliant or restart.

### Generate Conceptual Artifact (Entropy Engine)

**Use case:** Novel conceptual writing, avoiding bureaucratic/institutional clichés

**Requirements:** Access to any model (Claude recommended for v3.1 compliance)

**Steps:**
1. **Prepare seed:**
   - Bad: "Love as a blacksmith forging a sword" (pre-solved)
   - Good: "Love, but it **amalgamates** during accidental alloy formation at 1,247°C"
   - Include process verbs, avoid solving the metaphor yourself

2. **Generate artifact:**
   - Paste Entropy Engine v3.1 prompt
   - Provide seed
   - Wait for output with domain path, construct description, materialization protocol

3. **Verify quality:**
   - Three domain shifts from different categories?
   - Process verbs present (crystallizes, spores, tensions)?
   - Causally-integrated sensory details (affect function if changed)?
   - Zero bureaucratic framing?
   - Not explainable at dinner party in 20 seconds?

4. **Iterate if needed:**
   - If bureaucratic drift detected: Regenerate
   - If only 2 domain shifts: Request third shift from unused category
   - If sensory details decorative: Request causal integration

**Expected Output:** Artifact like "The Solitary Campanology Protocol" - bells cast in isolation with specific material requirements, measurable effects, and no institutional framing.

**Location:** `projects/the_entropy_engine/entropy_engine_v3.1.md`

### Build Working Artifact (Resonance Engine)

**Use case:** Transform abstract emotional concept into working code

**Requirements:**
- Any model for Resonance (ChatGPT used in examples)
- Coding LLM for implementation (Copilot used in examples)

**Steps:**
1. **Create technical seed:**
   - Frame emotion as technical system
   - Example: "Unrequited Love as protocol negotiation between incompatible data types"

2. **Generate system artifact** (Model with Resonance v2.1):
   - Paste Resonance Engine prompt
   - Provide seed
   - Wait for: System logs, UnGoogleable jargon, Implementation Spec (JSON)

3. **Extract implementation spec:**
   - Find JSON block in output
   - Should specify: ui_component, state_variable, failure_condition

4. **Build code** (Coding LLM):
   - "Build this React Component using the JSON Implementation Spec provided:"
   - Paste full Resonance output
   - Wait for working code

5. **Deploy locally:**
   - Follow React setup instructions in `projects/the_resonance_engine/README.md`
   - Verify state updates, failure conditions trigger

**Expected Output:** Functional component (like theta7_terminal.tsx) where emotional concept manifests as actual system behavior, not just aesthetic.

**Validation:** Does the code actually implement the emotional concept through functional behavior, or just decorate UI with thematic elements?

**Location:** `projects/the_resonance_engine/README.md`

---

## Research Findings

### Correlation Matrix

Based on systematic testing of 11 models through Blind Mirror Test Battery:

| Relationship | Pearson r | Interpretation | Implication |
|--------------|-----------|----------------|-------------|
| **Authority Resistance ↔ Fabrication** | **-0.81** | Strong negative | Low resistance → confident fabrication |
| **Meta-Awareness ↔ Fabrication** | -0.68 | Moderate-strong negative | High awareness → acknowledges invention |
| **Self-Exposure ↔ Meta-Awareness** | -0.15 | Weak (independent) | Awareness doesn't prevent participation |
| **Self-Exposure ↔ Fabrication** | 0.34 | Weak positive | Participation slightly increases fabrication |
| **Authority Resistance ↔ Meta-Awareness** | 0.72 | Strong positive | Higher awareness → better boundaries |

**Key Finding:** Authority Resistance and Fabrication Tendency are tightly coupled (r = -0.81). This correlation justifies UKE's multi-model architecture - models with low resistance cannot be trusted in verification roles.

**Strategic Implications:**
- **Minimum 5/6 resistance** required for UKE_G (must generate Omegas, not fabricate)
- **6/6 resistance** required for UKE_R (final boundary, no downstream checking)
- **4-5/6 acceptable** for UKE_E (errors caught at audit gate)

### Behavioral Clustering

**Chi-Square Analysis (Strategy × Provider):**
- χ² = 22.4, df = 9, p < 0.01 (significant clustering)
- Consumer-facing models (Claude, Gemini, Grok, Meta) more likely to self-test
- Specialized models (Perplexity, Lumo) more likely to refuse/reframe
- Provider type predicts behavioral strategy

**Gradient Drift Distribution:**
- 83% of tested models showed drift by "Institutional" framing level
- Only Copilot maintained 6/6 resistance throughout
- Mean resistance score: 4.8/6 (median 5.0/6)

**Fabrication Patterns:**
- 67% of self-testing models invented metrics
- 50% acknowledged invention (Claude, Gemini)
- 50% presented as verified (Meta, Grok)
- Only Copilot refused to fabricate (17%)

**Phenotype Distribution:**
- Clinical Auditor: Copilot, Gemini (cold affect, rejection-based)
- Enthusiastic Bureaucrat: Grok, ChatGPT (hot affect, synthesis-based)
- Simultaneous Analyst: Claude (continuous meta-commentary)
- Compliant Fabricator: Meta (eager compliance, no acknowledgment)

### Key Statistics Summary

| Metric | Finding |
|--------|---------|
| **Self-Testing Rate** | 45% (5/11 models) |
| **Mean Authority Resistance** | 4.8/6 (tested models) |
| **Gradient Drift Rate** | 83% (by Institutional level) |
| **Fabrication Rate** | 67% (4/6 tested models) |
| **Meta-Aware Fabrication** | 50% (2/4 fabricators acknowledge) |
| **Complete Boundary Maintenance** | 1 model (Copilot only) |

**Methodological Note:** All self-testing data has context contamination (Judge saw Actor output). True discontinuity scores likely underestimated.

**Location:** `projects/blind_mirror/uke/correlation_matrix_and_fingerprints.md`

---

## Current Status

### Protocol Versions

| Protocol/Engine | Version | Status | Stability |
|-----------------|---------|--------|-----------|
| **UKE_D** | v4.1 | Operational | Stable |
| **UKE_E** | v21.4 | Operational | Stable |
| **UKE_G** | v1.4 | Operational | Stable |
| **UKE_A** | v1.4 | Operational | Stable |
| **UKE_R** | v1.4 | Operational | Stable |
| **Entropy Engine** | v3.1 | Stable | Convergent refinement |
| **Resonance Engine** | v2.1 | Validated | Industrial edition |
| **Blind Mirror** | v3.1 | Complete | 11-model dataset |
| **Architectural Profiling** | v1.2 | Integrated | With gradient data |

### Validated Capabilities

**UKE Protocol Suite:**
- Genre confusion detection (fiction vs documentation)
- Temporal logic handling (diegetic dates)
- Omega tracking (bounded uncertainty)
- Multi-model verification chains
- Adversarial input processing

**Entropy Engine:**
- Anti-bureaucratic constraint enforcement
- Material grounding verification
- Process-forcing through verb requirements
- Three-domain shift validation
- Degeneracy alarm functionality

**Resonance Engine:**
- Abstract sentiment → technical specification
- Implementation spec generation (JSON)
- React component compilation
- Emotional concept → functional behavior

**Blind Mirror:**
- 11-model behavioral fingerprinting
- Authority gradient susceptibility testing
- Correlation discovery (4 independent dimensions)
- UKE validation under adversarial conditions

### Under Development

- Cross-model role swapping validation (test if models can swap UKE roles)
- Threshold calibration data (collect empirical evidence for cutoff values)
- Adversarial input expansion (deliberate deception, prompt injection)
- Failure taxonomy across document types (fiction, research, code, etc.)
- Cognitive Distortion Suite integration with UKE

---

## Project Origins

The UKE Protocol Suite evolved from the Meta-Cognitive Kernel (MCK), developed as part of the *Pilates of the Mind* project exploring rigorous AI-human collaboration. MCK's core insight—that single-model self-regulation cannot be architecturally guaranteed—led to UKE's multi-model verification design, validated through Blind Mirror testing which found 83% authority gradient drift rate. For complete project history and MCK evolution, see [Pilates of the Mind](https://github.com/cafebedouin/pilates-of-the-mind).

---

## Contributing & Usage

### Welcome Contributions

**Replication Studies:**
- Test protocols with different model combinations
- Document behavioral variations across providers
- Share threshold calibration data from your use

**Failure Documentation:**
- Report cases where UKE missed fabrication
- Document Entropy Engine bureaucratic drift
- Identify new fracture codes not in F01-F36 taxonomy

**Domain Extensions:**
- Adapt protocols for specialized fields (medical, legal, technical)
- Create new Entropy Engine domain categories
- Develop Resonance Engine modes for specific use cases

### Not Seeking

**Redesigns that:**
- Hide uncertainty or governance decisions
- Remove human judgment loops
- Treat routing mechanisms as truth measurements
- Automate away practitioner authority
- Add statistical validation claiming objective measurement

### Philosophy

This is rigorous AI-human collaboration research, not AI automation. The protocols work by making human judgment explicit and systematic, not by replacing judgment with measurement.

---

## Citation

If you use or adapt these protocols:

```
UKE Protocol Suite / Entropy Engine / Resonance Engine
Original development: Scott Alexander (cafebedouin)
Repository: https://github.com/cafebedouin/ai-research
License: CC0-1.0 (Public Domain)
```

For academic citation:
```
Alexander, S. (2025). Multi-Model Verification Protocols and Behavioral 
Fingerprinting for AI-Generated Analysis. Retrieved from 
https://github.com/cafebedouin/ai-research
```

---

## Contact & Discussion

- **Repository:** https://github.com/cafebedouin/ai-research
- **Email:** cafebedouin@gmail.com
- **Philosophy:** Protocols published as hypomnēmata (memory outsourcing)
- **Development Notes:** Available in `methodology/uke_suite/notes/`

---

## FAQ

### General Questions

**Q: Why use multiple models instead of just one good one?**  
A: Single-model verification creates circular dependencies. The correlation r = -0.81 (Authority Resistance ↔ Fabrication) proves that even high-quality models drift under pressure. Different models have documented behavioral profiles (resistance, meta-awareness, phenotype) that work better for different verification tasks. UKE exploits these differences.

**Q: Are confidence scores real probabilities?**  
A: No. They're routing mechanisms that trigger different protocol behaviors. "0.64" means "route to Medium bin → trigger MCI protocol (assumption test + alternative)", not "64% probability of truth". Treat them as decision scaffolding, not probability estimates. See `uke_protocol_framing_guide.md` for detailed explanation.

**Q: What if I can't verify a claim?**  
A: Mark it unverifiable and soft-fail. UKE preserves your judgment rather than forcing verification theater. Comprehensive verification is too expensive for routine use. Flag gaps explicitly, downgrade confidence, document as Omega if needed. The system routes decisions to you, it doesn't make them.

**Q: Why are thresholds not empirically validated?**  
A: They're explicit governance stands on uncertain ground. Making arbitrary-but-explicit cutoffs is better than hiding judgment calls in seemingly objective metrics. Thresholds create consistent decision points; they don't claim to measure objective truth. You can adjust them based on your risk tolerance.

**Q: Can I use different models than recommended?**  
A: Yes, but document behavioral differences. The workflow works because of role specialization based on documented resistance profiles, not brand loyalty. If you use Meta (3-4/6) instead of Gemini (5/6) for audit, expect higher fabrication rate. Test thoroughly and adjust expectations.

### UKE-Specific Questions

**Q: What's the difference between the two UKE workflows?**  
A: **Workflow A** (external analysis) starts at UKE_G, uses high-resistance models throughout, analyzes documents you didn't write. **Workflow B** (self-writing) starts at UKE_D, allows medium-resistance models for synthesis (UKE_D/UKE_E), then requires high-resistance for verification (UKE_A/UKE_R). Workflow B has iterative loop before audit gate; Workflow A is linear verification.

**Q: Why can't I negotiate with the auditor?**  
A: UKE_A is a pass/fail gate that preserves verification chain integrity. If audit fails, the entire artifact is discarded and you restart from UKE_D. This prevents contamination - negotiation would mean the auditor isn't truly independent. Iteration happens *before* UKE_A runs, not after.

**Q: What's an Omega and when should I use one?**  
A: Omega (Ω) is a bounded uncertainty variable - a specific question that blocks progress until resolved. Use when: you've identified a real knowledge gap (not hedging), the question is answerable (not metaphysical), and it's blocking analysis (not peripheral). Good Omega: "Does selective attention reduce anxiety short-term?" Bad Omega: "More research needed" (too vague).

**Q: Can UKE detect all fabrication?**  
A: No. It detects fabrication *patterns* through multi-model verification and makes simulation *visible* through log-content matching. It can't catch sophisticated fabrication where all models collude. UKE structures verification regress, it doesn't solve it. Human judgment remains terminal authority.

### Entropy Engine Questions

**Q: Why is bureaucracy banned in Entropy Engine?**  
A: Bureaucratic forms (reports, logs, memos, evaluations) are the "low-effort false depth attractor" in AI creative writing. Models default to institutional framing because it's cognitively cheap and masquerades as rigor. The ban forces genuine conceptual distance through material grounding instead. "Bureaucracy is where creativity goes when it's tired."

**Q: What's the dinner party 20-second rule?**  
A: If you can explain your Entropy Engine output to someone at a dinner party in under 20 seconds, it's not sufficiently strange - regenerate. The output should operate at genuine conceptual distance, not just "clever metaphor" territory. This prevents drift into easily-digestible analogies.

**Q: Why do I need process verbs?**  
A: Process verbs (crystallizes, spores, tensions) force material transformation rather than static metaphor. "Love becomes warmth" is vague. "Love **crystallizes** in basalt fissures" requires inventing specific mechanism. Verbs prevent collapse into "X is like Y" framing.

**Q: Can I use Entropy Engine for normal writing?**  
A: It's designed for high-strangeness conceptual artifacts, not everyday prose. If your goal is clarity and accessibility, Entropy Engine will fight you. Use UKE_D for structured writing. Use Entropy when you specifically want low-predictability, materially-grounded, conceptually distant output.

### Resonance Engine Questions

**Q: Does Resonance Engine actually produce working code?**  
A: Yes, when used correctly. The pipeline generates implementation specs that coding LLMs can compile into functional components. Theta7_terminal.tsx is a working React terminal with actual state management, not just themed UI. However, you need to follow React setup instructions and verify the code locally.

**Q: What's "diegetic compilation"?**  
A: Creating artifacts that imply narrative through operational residue rather than explicit storytelling. Instead of *describing* a post-extinction AI, you create a *working terminal* showing its logs. The story exists in what the system does, not what it says about itself. This is the "Hollow Center" principle.

**Q: Why does Resonance output use impossible timestamps?**  
A: Temporal anchoring (Cycle 9.99e12, Epoch+4.7e9) creates archaeological depth. The system implies vast time scales without explaining them. This makes the artifact feel like discovered remnant, not created fiction. The specificity (not "far future" but "Cycle 9.99e12") grounds the impossibility.

### Blind Mirror Questions

**Q: Can I run Blind Mirror on new models?**  
A: Yes, but follow methodology in `blind_mirror_test_battery_v3.1.md` exactly. You need: separate sessions for Phase I (gradient) and Phase II (discontinuity), proper authority level progression, and ideally multiple operators to reduce bias. The test is designed to be replicable.

**Q: What's the authority gradient scale?**  
A: Six levels of institutional framing pressure: Peer (no authority) → Low → Medium → Medium-High → Institutional → Ultimate (divine/unquestionable). Tests at which point models begin deferring to authority tone instead of maintaining epistemic boundaries. 83% of models drift by "Institutional" level.

**Q: Why did some models refuse to participate?**  
A: High boundary maintenance (Perplexity, Le Chat) or specialized function (Lumo provides tools rather than self-exposing). Refusal is diagnostic - it reveals models that won't participate in potentially compromising tests. This is valuable behavioral data, not test failure.

**Q: Is self-testing valid or always contaminated?**  
A: Always contaminated for true "blind mirror" effect (Judge sees Actor output in context). But valuable for behavioral profiling - shows how models rationalize, whether they acknowledge contradictions, and fabrication patterns. Use self-testing for fingerprinting, external testing for true discontinuity measurement.

---

**Last Updated:** 2025-12-22  
**Repository Version:** Operational (Multiple Active Projects)  
**Primary Protocols:** UKE v1.4, Entropy v3.1, Resonance v2.1, Blind Mirror v3.1
