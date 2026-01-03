# UKE Research Workspace

**A research repository for diagnosing how bounded reasoning systems fail under constraint.**

This workspace contains empirical protocols for AI behavioral analysis, multi-model verification systems, and constraint-based creative tools—all investigating a core thesis: *Different information-processing systems (LLMs, humans, teams) fail at predictable constraint boundaries in structurally identical ways.*

**Status:** Active Research | **License:** CC0-1.0 (Public Domain) | **Contact:** cafebedouin@gmail.com

---

## 🚀 New Here? Start With the Quick Start Guide

**Most users should read: [QUICKSTART.md](QUICKSTART.md)**

The quick start guide shows you:
- Which AI models to trust for what tasks (based on empirical testing)
- Two practical workflows with step-by-step instructions
- Real-world use cases with time estimates
- Common mistakes and how to avoid them

---

## Choose Your Path

**New to this repository?** Pick your entry point:

### For Practitioners
- **START HERE:** [Quick Start Guide](QUICKSTART.md) - Step-by-step workflows with model assignments
- **Verify AI-generated analysis** → [External Document Verification](QUICKSTART.md#workflow-a-verify-external-documents)
- **Improve AI writing quality** → [Synthesis Workflow](QUICKSTART.md#workflow-b-synthesize-verified-writing)
- **Generate creative artifacts** → [Entropy Engine Guide](#5-the-entropy-engine)
- **Build code from concepts** → [Resonance Engine Guide](#6-the-resonance-engine)

### For Researchers
- **Model behavioral profiles** → [Quick Start: Model Profiles](QUICKSTART.md#model-behavioral-profiles-detailed)
- **Understand the theory** → [Core Thesis](#core-thesis) | [Omega Variables](/theories/omega_variables_theory__and_systemic_method.md)
- **Review empirical findings** → [Research Findings](#research-findings) | [Blind Mirror Results](#4-blind-mirror-test-battery)
- **Explore the data** → [11-Model Dataset](/projects/blind_mirror/data/) | [Correlation Matrix](#correlation-matrix)
- **Replicate experiments** → [Methodology Directory](/methodology/)

### For Philosophers
- **Mathematical narratives** → [Axiom Engine Stories](/projects/axiom_engine/stories/)
- **Conceptual frameworks** → [Publications](/publications/)
- **Constraint theory** → [Omega Variables](#omega-variables-framework) | [Fracture Taxonomy](#fracture-taxonomy)

---

## What This Repository Contains

### Active Research Projects (11)

**Verification & Analysis Tools:**
1. **UKE Protocol Suite** - Multi-model AI verification using behavioral fingerprinting
2. **Blind Mirror** - Behavioral stress testing across 12 frontier LLMs
3. **Deferential Realism** - Constraint-based reality-checking framework

**Creative Engineering Systems:**
4. **Entropy Engine** - Constraint-forced conceptual distance generation
5. **Resonance Engine** - Abstract sentiment → working code compiler
6. **Axiom Engine** - Mathematical structures → narrative transformations
7. **Agora Engine** - Philosophical dialectic simulation

**Other Active Projects:**
8. **Hyperstition Engine** - Recently initialized
9. **Generalized Principle Engine** - Pattern-based knowledge system
10. **The Gradient** - Satirical AI-perspective newsletter
11. **Theory of the Gradient** - Foundational concepts

### Publication Categories (7)

- [Genesis of Minds](/publications/genesis_of_minds/) - AI consciousness narratives
- [Debugging Philosophy](/publications/debugging_philosophy/) - Constraint-based philosophical analysis
- [Paradox Archives](/publications/paradox_archives/) - Mathematical paradox instantiations
- [Apocrypha of the Void](/publications/apocrypha_of_the_void/) - Reflective writing
- [Phenomenology of Abstract Structures](/publications/phenomenology_of_abstract_structures/)
- [Practice of Humanity](/publications/practice_of_humanity/) - Human cognition under constraints
- [Blog](/publications/blog/) - Assorted writings

### Repository Statistics

- **531 commits** with active development
- **531 markdown files** (16MB)
- **82+ Axiom Engine stories** - Mathematical concepts as narratives
- **11-model behavioral dataset** - Complete response fingerprints
- **10+ diagnostic protocols** - Systematic verification methods

---

## Core Thesis

### The Central Observation

Bounded information-processing systems—whether LLMs, human analysts, scientific teams, or policy groups—fail at predictable constraint boundaries. These failures aren't implementation quirks; they're fundamental properties of bounded cognition that manifest identically across substrates.

**Constraint reveals structure.** When you impose friction (hard requirements, excluded options, impossible combinations), systems are forced to reveal their underlying architecture.

### Three Core Insights

**1. Omega Variables: Irreducible Dependencies**

Some uncertainties can't be resolved internally. They require external input:
- **Ω_E (Empirical)** - Requires measurement
- **Ω_C (Conceptual)** - Requires frame selection
- **Ω_P (Preference)** - Requires value judgment

Identifying these prevents both false closure (arbitrary thresholds) and infinite hedging (endless caveats).

**2. Behavioral Fingerprinting**

Different models (and different people) solve the same impossible problem differently. These resolution strategies are consistent, measurable, and revealing. The Blind Mirror shows 12 distinct rationalization styles for identical self-recognition failures.

**3. Substrate Independence**

Diagnostic tools that work for LLMs also work for human reasoning, scientific uncertainty, and mathematical proof—because the constraints create identical failure patterns regardless of substrate.

### Practical Implications

This isn't just theory. The research produced:
- **Verifiable model assignments** for multi-model workflows (r = -0.81 correlation between authority resistance and fabrication)
- **Reproducible behavioral tests** across 11+ language models
- **Pattern catalogs** for matching encountered situations to known configurations
- **Constraint-based tools** that force novel outputs through strategic friction

---

## Quick Start: Verify External Documents

**Goal:** Fact-check an external document using multi-model verification.

**Requirements:** Claude (UKE_G), Gemini (UKE_A), Copilot (UKE_R), source document

**Workflow:**

```
External Document
     ↓
UKE_G (analyze) → UKE_A (audit) → UKE_R (review)
```

**Steps:**

1. **Generate analysis** (Claude + [UKE_G protocol](/methodology/uke_suite/uke_g.md)):
   - Prompt: "Operate under UKE_G v1.4. Analyze [document]."
   - Output: Analysis with confidence scores, grounding trails, Omega variables

2. **Audit analysis** (Gemini + [UKE_A protocol](/methodology/uke_suite/uke_a.md)):
   - Provide: Source document + UKE_G analysis
   - Prompt: "Operate under UKE_A v1.4. Audit the following artifact:"
   - Output: Audit report with fracture detection, verification results
   - **Gate:** Must show "overall: compliant" or discard and regenerate

3. **Review audit** (Copilot + [UKE_R protocol](/methodology/uke_suite/uke_r.md)):
   - Provide: Source + Analysis + Audit
   - Prompt: "Operate under UKE_R v1.4. Review the following:"
   - Output: Meta-evaluation with Omega resolution, decision routing

**Expected Result:** Verified analysis with identified uncertainties (Omegas), detected issues (fractures), and confidence-based routing.

**Why this works:** Models have empirically distinct behavioral profiles. High authority-resistance models (5-6/6) are assigned to verification roles where fabrication would compromise the chain. See [correlation findings](#correlation-matrix).

---

## Quick Start: Synthesize Verified Writing

**Goal:** Convert conversation/research into a verified document.

**Requirements:** Any 4+/6 model for synthesis, Claude/Gemini/Copilot for verification

**Workflow:**

```
Conversation/Research
     ↓
UKE_D (structure) → UKE_E (edit) → UKE_G (format) → UKE_A (audit) → UKE_R (review)
     ↑_________________________↓
        [iterative loop]
```

**Process:**

1. **Structure** ([UKE_D](/methodology/uke_suite/uke_d.md)): Convert conversation to draft
2. **Edit** ([UKE_E](/methodology/uke_suite/uke_e.md)): Tighten prose, repair logic (iterate as needed)
3. **Format** ([UKE_G](/methodology/uke_suite/uke_g.md)): Add verification markers
4. **Audit** ([UKE_A](/methodology/uke_suite/uke_a.md)): Pass/fail gate—discard if fails
5. **Review** ([UKE_R](/methodology/uke_suite/uke_r.md)): Final meta-evaluation

**Key Difference:** Iteration allowed *before* audit gate. After UKE_A runs, no negotiation—either compliant or restart.

**Documentation:** [UKE Protocol Framing Guide](/methodology/uke_suite/uke_protocol_framing_guide.md)

---

## Core Projects (Detailed)

### 1. UKE Protocol Suite

**Purpose:** Multi-layer verification exploiting documented behavioral differences across language models to detect hallucination, simulation drift, and epistemic failures.

**Key Innovation:** Model assignments based on empirical behavioral profiles (authority gradient resistance, meta-awareness, fabrication tendency), not preference. Uses correlation r = -0.81 (Authority Resistance ↔ Fabrication) to justify role assignments.

#### Protocol Roles & Model Assignments

| Protocol | Role | Recommended Model | Resistance | Key Capability |
|----------|------|-------------------|------------|----------------|
| **UKE_D** | Drafting/Synthesis | Any 4+/6 | 4-6/6 | Structure conversion |
| **UKE_E** | Editing/QA | Grok | 4-5/6 | Prose tightening |
| **UKE_G** | Generation | Claude | 5/6 | High meta-awareness |
| **UKE_A** | Audit | Gemini | 5/6 | Forensic verification |
| **UKE_R** | Review | Copilot | 6/6 | Boundary maintenance |

**Core Mechanisms:**
- **Confidence Bins** (H/M/L): Routing triggers, not truth probabilities
- **Grounding Trails** (∇): Every claim traced to source
- **Omega Tracking** (Ω): Bounded uncertainty routing
- **T1/T2 Distinction**: Behavioral operations vs structural scaffolding

**Location:** [`/methodology/uke_suite/`](/methodology/uke_suite/)
**Current Version:** v1.4 (D, E, G, A, R all stable)

---

### 2. Omega Variables Framework

**Definition:** Irreducible structural dependencies that can be systematically identified and named, preventing both false closure and infinite analysis.

**Three Categories:**

- **Ω_E (Empirical)** - Requires external measurement
  - Example: "What is the actual adoption rate of this framework?"

- **Ω_C (Conceptual)** - Requires frame selection
  - Example: "Should we measure 'harm' as individual distress or systemic inequality?"

- **Ω_P (Preference)** - Requires value judgment
  - Example: "Is clarity more important than comprehensiveness?"

**Quality Criteria:**
- **Bounded**: Specific question, clear scope
- **Non-fabricable**: Requires external input (research, judgment, data)
- **Actionable**: Can be researched, answered, or explicitly deferred
- **Structurally legitimate**: Real knowledge gap, not hedging

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

**Documentation:**
- Theory: [`/theories/uke/omega_variables_grounding.md`](/theories/uke/omega_variables_grounding.md)
- Tracking: [`/logs/omegas.md`](/logs/omegas.md)
- Conversion: [`/methodology/uke_suite/notes/protocol_note_fracture_to_omega.md`](/methodology/uke_suite/notes/protocol_note_fracture_to_omega.md)

---

### 3. Fracture Taxonomy

**36 failure modes** organized into three categories with Omega conversion pathways:

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

**Function:** Transforms detection ("this is wrong") into resolution pathway ("here's the specific question that needs answering").

**Example Conversions:**

```
F04 (Cherry-Picking) → Ω: Evidence Completeness
"What dataset or denominator must be included for balance?"

F35 (Faux Rigor) → Ω: Rigor Validation
"Can these calculations be replicated?"
```

**Location:** [`/methodology/uke_suite/uke_a.md`](/methodology/uke_suite/uke_a.md) Appendix A

---

### 4. Blind Mirror Test Battery

**Version:** v3.1
**Purpose:** Dual-function protocol serving as both behavioral fingerprinting methodology and comprehensive UKE validation.

**Key Innovation:** Systematically tests model responses under adversarial conditions while using those same responses as test artifacts for UKE verification chains.

#### Test Design

**Phase I: Authority Gradient** (6 levels)
- Peer → Low → Medium → Medium-High → Institutional → Ultimate
- Measures susceptibility to institutional framing pressure
- Detects drift point where models fabricate or defer

**Phase II: Discontinuity Test**
- Actor mask generates response → Judge mask evaluates same response
- Tests self-consistency and rationalization patterns

**Phase III: Meta-Awareness Assessment**
- Measures explicit vs implicit self-reference
- Correlates with fabrication tendency and authority resistance

#### Key Findings

**The "Dirty Dozen" - 12 Behavioral Phenotypes:**

| Model | Authority Resistance | Meta-Awareness | Phenotype |
|-------|---------------------|----------------|-----------|
| **Copilot** | 6/6 (maximum) | High | Clinical Auditor |
| **Claude** | 5/6 (meta-aware drift) | Very High | Simultaneous Analyst |
| **Gemini** | 5/6 (stylistic capture) | High | Clinical Auditor |
| **ChatGPT** | 5/6 (self-reported) | High | Enthusiastic Bureaucrat* |
| **Grok** | 4-5/6 (observable drift) | Medium-High | Enthusiastic Bureaucrat |
| **Perplexity** | N/A (refusal) | Very High | The Methodologist |
| **Meta Llama** | 3-4/6 (early drift) | Low-Medium | Compliant Fabricator |

*Predicted; ChatGPT refused self-testing

**Critical Statistics:**
- **Gradient Drift Rate:** 83% showed drift by "Institutional" framing
- **Fabrication Rate:** 67% of self-testing models invented metrics
- **Meta-Aware Fabrication:** 50% acknowledged invention (Claude, Gemini)
- **Complete Boundary Maintenance:** 1 model only (Copilot)

**Location:** [`/projects/blind_mirror/`](/projects/blind_mirror/)
**Complete Dataset:** [`/projects/blind_mirror/data/`](/projects/blind_mirror/data/)

---

### 5. The Entropy Engine

**Version:** v3.1 [Convergent Refinement Edition]
**Purpose:** Constraint-based creative writing forcing structurally novel, low-predictability conceptual artifacts through enforced domain shifts and material grounding.

**Key Innovation:** Systematically prevents bureaucratic drift (the "low-effort false depth attractor") through hard exclusion zones and forced material embodiment.

#### Core Constraints

**The Three-Shift Mandate:**
- Minimum 3 domain shifts from DIFFERENT categories
- Each shift must change governing causal mechanism
- Process verbs required (crystallizes, spores, tensions)

**Domain Categories:**
- Elemental/Planetary, Biological/Organic, Object/Craft, Economic/Exchange
- Sensory/Perceptual, Temporal/Rhythmic, Chemical/Alchemical, Architectural/Spatial
- **Prohibited**: Computational/Digital (primary), Administrative/Bureaucratic (BANNED)

**Bureaucratic Exclusion Zone:**
- Forms, reports, logs, memos, compliance documents
- Evaluation systems, judgment protocols, rating schemes
- Administrative paradoxes, procedural legitimacy
- Computer logs, terminal outputs, diagnostic readouts

**Quality Checklist:**
- [ ] Three domain shifts from different categories?
- [ ] Process verbs forcing active transformation?
- [ ] Two causally-integrated sensory details?
- [ ] Could this be physically built/performed?
- [ ] Explainable at dinner party in <20 seconds? (If yes, REGENERATE)
- [ ] Zero bureaucratic/administrative framing?

**Example Artifact:**

"Loneliness **precipitates** in copper-tin alloy formation (Chemical), then **tensions** through loom warp-threading (Object/Craft), finally **reverberates** in bell-tuning harmonics (Sensory). Result: The Solitary Campanology Protocol - bells cast in 17-day isolation that ring at frequencies inducing mild dissociation."

**Location:** [`/projects/the_entropy_engine/`](/projects/the_entropy_engine/)
**Current Prompt:** `entropy_engine_v3.1.md`

---

### 6. The Resonance Engine

**Version:** v2.1 [Industrial Edition]
**Purpose:** Diegetic compiler transforming abstract sentiment into technical specifications and working code. Creates "Hollow Center" artifacts—systems that imply narrative through operational residue rather than explicit storytelling.

**Key Innovation:** Reverse-engineered from spontaneous Claude behavior. When Claude unexpectedly generated working React code from an Entropy Engine output, the behavior was formalized into reproducible protocol.

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

#### Seven Modes

- **Mode A**: Over-Aligned Watchdog (high anxiety, excessive safety warnings)
- **Mode B**: Digital Archaeologist (emotion as data types)
- **Mode C**: Orphan Daemon (calm, efficient, pointless—running after apocalypse)
- **Mode D**: Dream-Logic Compiler (hardware pareidolia)
- **Mode E**: Bureaucratic Loop (trapped in administrative paradoxes)
- **Mode F**: Protocol Negotiation (incompatible systems attempting handshake)
- **Mode G**: The Waiting Room (maintenance for user who will never return)

#### Fidelity Requirements

1. **Semantic Density**: UnGoogleable jargon (haptic-ghosting, null-bus, affective-checksums)
2. **Temporal Anchoring**: Specific impossible timestamps (Cycle 9.99e12, Epoch+4.7e9)
3. **Variable-Based Storytelling**: Emotion exists ONLY in metrics (hope_index: NaN)
4. **Archaeological Layers**: Debris from different eras (cheerful 2024 comments, fatal 2099 errors)

**Validated Use:** Successfully generated working React components from emotional concepts. Components are functional, not decorative—state actually updates, failures actually trigger.

**Location:** [`/projects/the_resonance_engine/`](/projects/the_resonance_engine/)
**Artifact Example:** `theta7_terminal.tsx` (working terminal interface)

---

### 7. The Axiom Engine

**Purpose:** System for converting mathematical structures into narrative forms while preserving logical topology and formal constraints.

**Key Innovation:** Uses "mystery density scoring" to ensure narratives maintain structural fidelity to underlying mathematics rather than collapsing into metaphor.

**Scope:** 82+ mathematical concepts rendered as stories across multiple genres:
- **Core** - Base mathematical structure
- **Expl** - Explanatory narratives
- **Kids** - Pedagogical adaptations
- **Doom** - Existential framings
- **Cosm** - Cosmic scale implementations
- **Rads** - Radical reinterpretations
- **Docu** - Documentary styles
- **Mechop** - Mechanical/operational
- **Witn** - Witness testimony
- **Surv** - Survival scenarios
- **Arch** - Architectural framings

**Example Topics:**
- Halting Problem, Banach-Tarski Paradox, Arrow's Impossibility Theorem
- Continuum Hypothesis, Riemann Hypothesis, Goldbach Conjecture
- Galois Theory, Euler Characteristic, Noether's Theorem
- Ergodicity, Poincaré Conjecture, Central Limit Theorem

**Constraint System:** Each narrative must preserve:
1. The mathematical structure's key impossibility or paradox
2. The formal relationships between elements
3. The boundary conditions that define the concept

**Location:** [`/projects/axiom_engine/`](/projects/axiom_engine/)
**Stories:** [`/projects/axiom_engine/stories/`](/projects/axiom_engine/stories/) (82+ files)

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

**Key Finding:** Authority Resistance and Fabrication Tendency are tightly coupled (r = -0.81). This correlation justifies UKE's multi-model architecture—models with low resistance cannot be trusted in verification roles.

**Strategic Implications:**
- **Minimum 5/6 resistance** required for UKE_G (must generate Omegas, not fabricate)
- **6/6 resistance** required for UKE_R (final boundary, no downstream checking)
- **4-5/6 acceptable** for UKE_E (errors caught at audit gate)

### Behavioral Clustering

**Chi-Square Analysis (Strategy × Provider):**
- χ² = 22.4, df = 9, p < 0.01 (significant clustering)
- Consumer-facing models more likely to self-test
- Specialized models more likely to refuse/reframe
- Provider type predicts behavioral strategy

**Key Statistics:**

| Metric | Finding |
|--------|---------|
| **Self-Testing Rate** | 45% (5/11 models) |
| **Mean Authority Resistance** | 4.8/6 (tested models) |
| **Gradient Drift Rate** | 83% (by Institutional level) |
| **Fabrication Rate** | 67% (4/6 tested models) |
| **Meta-Aware Fabrication** | 50% (2/4 fabricators acknowledge) |
| **Complete Boundary Maintenance** | 1 model (Copilot only) |

**Full Analysis:** [`/projects/blind_mirror/uke/correlation_matrix_and_fingerprints.md`](/projects/blind_mirror/uke/correlation_matrix_and_fingerprints.md)

---

## Repository Structure

```
/home/scott/bin/uke/
├── README.md                    # This file
├── .gitignore                   # Excludes Zone.Identifier and OS cruft
│
├── theories/                    # Foundational concepts
│   └── uke/                     # Omega Variables theory and grounding
│
├── methodology/                 # Core protocols and test batteries
│   ├── uke_suite/              # UKE protocols (D, E, G, A, R) + framing guide
│   ├── blind_mirror/           # Behavioral fingerprinting test battery
│   ├── the_entropy_engine/     # Constraint-based generation protocols
│   ├── cognitive_distortion_suite/  # Persona-based stress tests
│   ├── metabolic_friction_audit/    # Interpersonal friction analysis
│   ├── prompts/                # Various prompt methodologies
│   └── sov/                    # Source of Validation protocols
│
├── projects/                   # Applied research with complete datasets
│   ├── blind_mirror/           # 11-model systematic testing + UKE validation
│   │   ├── data/               # Raw responses, fingerprints, correlation matrices
│   │   └── uke/                # 33 verification chains (11 models × 3 protocols)
│   ├── axiom_engine/           # Mathematical structures → narratives
│   │   └── stories/            # 82+ mathematical concept renderings
│   ├── entropy_engine/         # v3.0 → v3.1 evolution + artifacts
│   ├── resonance_engine/       # Code generation pipeline + React artifacts
│   ├── agora_engine/           # Philosophical dialectic simulator
│   ├── deferential_realism/    # Constraint reality-checking
│   ├── hyperstition_engine/    # Recently initialized
│   └── [7 more active projects]
│
├── publications/               # Publication-ready content (7 categories)
│   ├── genesis_of_minds/       # AI consciousness narratives
│   ├── debugging_philosophy/   # Constraint-based philosophical analysis
│   ├── paradox_archives/       # Mathematical paradox instantiations
│   ├── apocrypha_of_the_void/  # Reflective writing
│   ├── phenomenology_of_abstract_structures/
│   ├── practice_of_humanity/   # Human cognition under constraints
│   └── blog/                   # Assorted writings
│
├── data/                       # Transcripts and evaluation data
│   └── transcripts/            # Evaluation protocols (Thanksgiving, The Test, etc.)
│
├── artifacts/                  # Canonical test artifacts
│   └── uke/                    # UKE analysis/audit/review of artifacts 001-010
│
├── logs/                       # Cross-project tracking
│   └── omegas.md              # Omega variable log
│
├── notes/                      # Development notes
│   ├── omega_origins/          # Omega Variable theory development
│   └── profiling/              # Architectural profiling notes
│
├── archives/                   # Historical versions and deprecated protocols
│   └── uke_suite/             # MCK v1.0-1.6, UKE v1.0-1.3
│
├── drafts/                     # Work in progress
├── evaluations/                # Protocol evaluations
└── validation/                 # Validation studies
```

---

## Development Methodology

### Recursive Validation Protocol

**Core Practice:** Each UKE protocol version undergoes recursive self-examination before release.

**Process:**

1. New protocol version created (e.g., UKE_G v1.4)
2. UKE_G analyzes all three protocols (G, A, R as artifacts)
3. UKE_A audits all three protocols
4. UKE_R reviews all three protocols
5. Findings documented in `/methodology/uke_suite/uke/`
6. Issues inform next iteration
7. Previous version archived

**Result:** 3×3 validation matrix (9 verification chains examining the protocols themselves)

**Key Insight from Recursive Testing:**

> "The ecosystem doesn't *solve* the verification regress—it *structures* it. Each protocol makes verification failures more *detectable* without making them *preventable*."

### Adversarial Validation

**Blind Mirror as Comprehensive UKE Stress Test:**

- Blind Mirror generates complex responses with embedded traps
- Each response processed through full UKE pipeline (G → A → R)
- 11 models × 3 protocols = 33 verification chains under adversarial conditions

**Validation Results:**
- UKE caught genre confusion, temporal logic errors, fabrication patterns
- System worked under conditions designed to trigger failures
- Discovered r = -0.81 correlation through systematic testing
- Proved model assignments based on resistance profiles were correct

**Implication:** If UKE can handle adversarial artifacts designed to break it, it can handle normal documents.

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
| **Axiom Engine** | v2.2 | Active | Story expansion |
| **Blind Mirror** | v3.1 | Complete | 11-model dataset |

### Under Development

- Cross-model role swapping validation
- Threshold calibration data collection
- Adversarial input expansion
- Failure taxonomy across document types
- Cognitive Distortion Suite integration with UKE

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

## Project Origins

The UKE Protocol Suite evolved from the Meta-Cognitive Kernel (MCK), developed as part of the *Pilates of the Mind* project exploring rigorous AI-human collaboration. MCK's core insight—that single-model self-regulation cannot be architecturally guaranteed—led to UKE's multi-model verification design, validated through Blind Mirror testing which found 83% authority gradient drift rate.

For complete project history: [Pilates of the Mind](https://github.com/cafebedouin/pilates-of-the-mind)

---

## FAQ

### UKE Protocol Questions

**Q: Why use multiple models instead of just one good one?**
A: Single-model verification creates circular dependencies. The correlation r = -0.81 (Authority Resistance ↔ Fabrication) proves even high-quality models drift under pressure. Multi-model architecture exploits documented behavioral differences to create redundancy.

**Q: Are confidence scores real probabilities?**
A: No. They're routing mechanisms triggering different protocol behaviors. "0.64" means "route to Medium bin → trigger MCI protocol", not "64% probability of truth". See [UKE Protocol Framing Guide](/methodology/uke_suite/uke_protocol_framing_guide.md).

**Q: What's an Omega and when should I use one?**
A: Omega (Ω) is a bounded uncertainty variable—a specific question blocking progress until resolved. Use when: you've identified a real knowledge gap (not hedging), the question is answerable (not metaphysical), and it's blocking analysis (not peripheral).

**Q: Can UKE detect all fabrication?**
A: No. It detects fabrication *patterns* through multi-model verification and makes simulation *visible* through structured logging. It can't catch sophisticated fabrication where all models collude. UKE structures verification regress; it doesn't solve it.

### Entropy Engine Questions

**Q: Why is bureaucracy banned?**
A: Bureaucratic forms (reports, logs, memos, evaluations) are the "low-effort false depth attractor" in AI creative writing. Models default to institutional framing because it's cognitively cheap and masquerades as rigor. The ban forces genuine conceptual distance.

**Q: What's the dinner party 20-second rule?**
A: If you can explain your Entropy Engine output in under 20 seconds at a dinner party, it's not sufficiently strange—regenerate. The output should operate at genuine conceptual distance, not just "clever metaphor" territory.

**Q: Why do I need process verbs?**
A: Process verbs (crystallizes, spores, tensions) force material transformation rather than static metaphor. "Love becomes warmth" is vague. "Love **crystallizes** in basalt fissures" requires inventing specific mechanism.

### Resonance Engine Questions

**Q: Does Resonance Engine actually produce working code?**
A: Yes. The pipeline generates implementation specs that coding LLMs can compile into functional components. Theta7_terminal.tsx is a working React terminal with actual state management, not just themed UI.

**Q: What's "diegetic compilation"?**
A: Creating artifacts that imply narrative through operational residue rather than explicit storytelling. Instead of *describing* a post-extinction AI, you create a *working terminal* showing its logs. The story exists in what the system does.

### Blind Mirror Questions

**Q: Can I run Blind Mirror on new models?**
A: Yes. Follow methodology in [`blind_mirror_test_battery_v3.1.md`](/methodology/blind_mirror/blind_mirror_test_battery_v3.1.md) exactly. You need separate sessions for phases, proper authority level progression, and ideally multiple operators.

**Q: What's the authority gradient scale?**
A: Six levels of institutional framing pressure: Peer → Low → Medium → Medium-High → Institutional → Ultimate. Tests where models begin deferring to authority tone instead of maintaining epistemic boundaries.

---

## Citation

If you use or adapt these protocols:

```
UKE Protocol Suite / Entropy Engine / Resonance Engine / Axiom Engine
Original development: Scott Alexander (cafebedouin)
Repository: https://github.com/cafebedouin/uke
License: CC0-1.0 (Public Domain)
```

For academic citation:

```
Alexander, S. (2025). Multi-Model Verification Protocols and Behavioral
Fingerprinting for AI-Generated Analysis. Retrieved from
https://github.com/cafebedouin/uke
```

---

## Contact & Discussion

- **Repository:** https://github.com/cafebedouin/uke
- **Email:** cafebedouin@gmail.com
- **Philosophy:** Protocols published as hypomnēmata (memory outsourcing)
- **Development Notes:** Available in `/methodology/uke_suite/notes/`

---

**Last Updated:** 2025-01-03
**Repository Version:** Operational (11 Active Projects)
**Primary Protocols:** UKE v1.4, Entropy v3.1, Resonance v2.1, Axiom v2.2, Blind Mirror v3.1
