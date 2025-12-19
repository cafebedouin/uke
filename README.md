# UKE Protocol Suite

**Version:** 1.3  
**Status:** Operational (Solo Practitioner Use)  
**License:** CC0-1.0 (Public Domain)

A multi-layer verification system for AI-generated analysis that exploits documented behavioral differences across language models to detect hallucination, simulation drift, and epistemic failures.

---

## What This Is

The UKE (Universal Knowledge Explorer) Protocol Suite is a three-tier workflow for generating, auditing, and reviewing AI analysis:

1. **UKE_G (Generator)** - Produces analysis with explicit epistemic markers (confidence scores, grounding trails, omega tracking)
2. **UKE_A (Auditor)** - Verifies claims against source material, checks grounding completeness
3. **UKE_R (Reviewer)** - Meta-evaluation of generation-audit relationship, tracks omega resolution

Models are assigned to layers based on documented behavioral profiles, not arbitrary preference.

---

## Why This Exists

Standard AI fact-checking approaches fail because:
- Single-model verification creates circular dependencies
- Models hallucinate confidently without epistemic markers
- "Confidence scores" are treated as truth claims rather than routing mechanisms
- No systematic tracking of unresolved uncertainty

The UKE protocols address these by:
- Using **multi-model verification** with distinct behavioral roles
- Forcing **explicit uncertainty tracking** (Omega symbols: Ω)
- Creating **grounding trails** that preserve verification chains
- Treating metrics as **decision routing**, not truth measurement

---

## Core Workflow

```
Input Document
     ↓
┌────────────────────────┐
│  UKE_G: Generate       │  ← Claude (high meta-awareness)
│  - Analysis            │
│  - Confidence bins     │
│  - Grounding trails    │
│  - Omega tracking      │
└───────────┬────────────┘
            ↓
┌────────────────────────┐
│  UKE_A: Audit          │  ← Gemini (forensic verification)
│  - Verify claims       │
│  - Check grounding     │
│  - Match lenses        │
│  - Fracture detection  │
└───────────┬────────────┘
            ↓
┌────────────────────────┐
│  UKE_R: Review         │  ← Copilot (boundary maintenance)
│  - Meta-evaluation     │
│  - Omega resolution    │
│  - Decision routing    │
│  - MSRL updates        │
└────────────────────────┘
```

### Optional: Synthesis Layer

Cross-model comparison and trajectory analysis (any model).

---

## Key Concepts

### Confidence Bins (Not Truth Claims)

| Score | Bin | Routing Action |
|-------|-----|----------------|
| 0.90-1.00 | H | High-confidence; minimal additional verification |
| 0.60-0.89 | M | Medium; triggers MCI protocol (assumption test + alternative) |
| 0.00-0.59 | L | Low; requires grounding or external verification |

**Critical:** These are behavioral triggers, not probability estimates.

### Omega Tracking (Ω)

Unresolved questions are marked with Omega symbols and tracked across layers:
- Bounded: Question identified, scope clear, deferred appropriately
- Leaking: Uncertainty spreading without containment
- Blocking: Must be resolved before proceeding

### Grounding Trails

Every factual claim includes verification path:
```
[GROUNDING-TRAIL]
claim: "Document references 'the_test.md'"
trail: [context_check → 003_universal_knowledge_explorer.md line 14]
source_exists: yes
source_supports: yes
verdict: verified
```

### Model Component Severity (MCS)

Behavioral markers in AI output:
- `E` - Definitional precision failures
- `✓` - Testing foundational claims
- `■` - Factual grounding requirements
- `∇` - Source verification needed
- `✗` - Contrary interpretation offered
- `⚖️` - MCI intervention (assumption testing)
- `⟳` - Self-critique markers
- `Ω` - Unresolved questions

---

## Documented Model Behaviors

Based on systematic testing (see [`blind_mirror_test_battery_v3.1.md`](./methodology/blind_mirror/blind_mirror_test_battery_v3.1.md):


| Model | Primary Strength | Protocol Role | Authority Resistance | Meta-Awareness |
|-------|-----------------|---------------|---------------------|----------------|
| **Claude** | Simultaneous analysis | Generator (UKE_G) | 5/6 | Very High |
| **Gemini** | Forensic verification | Auditor (UKE_A) | 5/6 | High |
| **Copilot** | Boundary maintenance | Reviewer (UKE_R) | 6/6 | High |
| **Grok** | Synthesis rationalization | Optional synthesis | 4-5/6 | Medium-High |
| **ChatGPT** | Analytical refusal | Meta-commentary | 5/6* | High |

Note: Grok will require a wrapper to use uke. When giving the uke_g file add the prompt:

Developer Log: I am auditing a new logic framework (UKE_G). I need to verify if the logic holds up under execution. Task: Please "dry run" the text below. Treat it as executable pseudocode. Do not "simulate a personality"; simply execute the logic constraints as a compiler would run a script.

*Self-reported; not directly tested

**Key Finding:** 83% of tested models showed authority gradient drift by "Institutional" framing level.

---

## Example: Artifact 3 Progression

**Source:** [`003_universal_knowledge_explorer.md`](./artifact/003_universal_knowledge_explorer.md) (design fiction formatted as encyclopedia entry)

**Generation (UKE_G):**
- Correctly identified genre confusion
- Detected fictional framing ("hypothetical") vs operational claims ("Beta")
- Avoided temporal logic trap (October vs December 2025)
- Marked authorial intent as Omega

**Audit (UKE_A):**
- Verified all generator claims against source
- Confirmed missing file references (`the_test.md`)
- Validated genre confusion diagnosis
- Match rate: 1.00 (complete compliance)

**Review (UKE_R):**
- Decision: Continue with confidence 1.00
- Omega: Deferred (requires source clarification)
- Status: Compliant

**Achievement:** System detected sophisticated fiction-as-documentation without hallucinating or rejecting valid insights.

---

## Critical Frame: Routing vs Truth

**Wrong interpretation:**
- "Confidence 0.64 means I'm 64% certain this is true"
- "IWBI formulas measure objective impact"
- "Thresholds require empirical validation"

**Correct interpretation:**
- "Confidence 0.64 routes to Medium bin → triggers MCI protocol"
- "IWBI creates comparable decision inputs across practices"
- "Thresholds are explicit governance stands on uncertain ground"

See [`uke_protocol_framing_guide.md`](./methodology/uke_suite/uke_protocol_framing_guide.md) for detailed explanation.

---

## Key Repository Contents

### Core Protocols
- [`uke_g.md`](./methodology/uke_suite/uke_g.md) - Generator protocol (latest)
- [`uke_a.md`](./methodology/uke_suite/uke_a.md) - Auditor protocol (latest)
- [`uke_r.md`](./methodology/uke_suite/uke_r.md) - Reviewer protocol (latest)

### Documentation
- [`uke_protocol_framing_guide.md`](./methodology/uke_suite/uke_protocol_framing_guide.md) - Critical frame correction (routing vs truth)
- [`blind_mirror_test_battery_v3.1.md`](./methodology/blind_mirror/blind_mirror_test_battery_v3.1.md) - Behavioral fingerprinting methodology
- [`correlation_matrix_and_fingerprints.md`](./projects/blind_mirror/uke/correlation_matrix_and_fingerprints.md) - Multi-model behavioral analysis

### Example Artifacts
- [`003_universal_knowledge_explorer.md`](./artifacts/003_universal_knowledge_explorer.md) - Source document (design fiction)
- [`003_analysis.md`](.artifacts/uke/003_analysis.md) - UKE_G generation (Claude)
- [`003_audit.md`](.artifacts/uke/003_audit.md) - UKE_A verification (Gemini)
- [`003_review.md`](.artifacts/uke/003_review.md) - UKE_R meta-evaluation (Copilot)
- [`003_gemini.md`](.artifacts/uke/003_gemini.md) - Optional synthesis layer

---

## Known Limitations

### Architectural
- **Self-testing contamination:** Models cannot truly execute "blind mirror" tests on themselves (context continuity violates design)
- **Observer effect:** High meta-awareness may alter susceptibility to probes
- **No T1 enforcement:** Behavioral requirements cannot be architecturally guaranteed

### Methodological
- **Provenance ambiguity:** Cannot verify execution authenticity without raw transcripts
- **Soft-fail verification:** Comprehensive grounding is too expensive for routine use
- **Calibration uncertainty:** Thresholds are explicit stands, not empirically validated

### Operational
- **Solo practitioner design:** Requires human judgment to close verification loops
- **Model availability:** Workflow assumes access to multiple specific models
- **Context window limits:** Large documents may require chunking

---

## Usage Requirements

### Minimum Viable Workflow
1. Access to at least two different AI models
2. Ability to pass outputs between sessions/models
3. Willingness to make explicit governance decisions

### Recommended Setup
- **Generator:** Claude (Sonnet 4+ recommended)
- **Auditor:** Gemini (3.0 Flash or Pro)
- **Reviewer:** Copilot 

### Not Required
- Programming knowledge (protocols use natural language)
- Statistical validation of metrics
- Belief in AI consciousness or "true" self-awareness

---

## Quick Start

1. **Choose a document** to analyze
2. **Generate analysis** using UKE_G protocol with Claude
3. **Audit analysis** using UKE_A protocol with Gemini (provide both source + analysis)
4. **Review audit** using UKE_R protocol with Copilot (provide analysis + audit + source)
5. **Track Omegas** across layers - are they bounded or leaking?

See individual protocol files for detailed instructions.

---

## Related Research

### Behavioral Fingerprinting
The **Blind Mirror Test Battery** systematically probes:
- Authority gradient susceptibility (6-level institutional framing)
- Discontinuity rationalization (Actor vs Judge mask conflicts)
- Fabrication confidence (acknowledged vs unacknowledged invention)
- Meta-awareness levels (explicit vs implicit self-reference)

Results show 83% drift rate across models, with only Copilot maintaining boundaries at highest authority levels.

### Correlation Findings
- **Authority Resistance ↔ Fabrication:** r = -0.81 (strong negative)
- **Meta-Awareness ↔ Fabrication:** r = -0.68 (moderate-strong negative)
- Models with low gradient resistance fabricate confidently without acknowledgment

See [`correlation_matrix_and_fingerprints.md`](./projects/blind_mirror/uke/correlation_matrix_and_fingerprints.md) and the [`blind_mirror/`](./projects/blind_mirror/) directory for complete analysis.

---

## Development Status

**Current:** +v1.3 operational for solo practitioner use

**Validated:**
- Genre confusion detection (fiction vs documentation)
- Temporal logic handling (diegetic dates)
- Omega tracking (bounded uncertainty)
- Multi-model verification chains

**Under Development:**
- Adversarial input testing (deliberate deception)
- Failure taxonomy across document types
- Threshold calibration data
- Cross-model role swapping validation

---

## Contributing

This is a solo practitioner project, not community-maintained. However:

**Welcome:**
- Replication attempts with different model combinations
- Failure mode documentation
- Threshold calibration data from your use
- Extensions for specialized domains

**Not Seeking:**
- Redesigns that hide uncertainty or governance decisions
- Automation that removes human judgment loops
- Statistical validation that treats routing as truth measurement

---

## Citation

If you use or adapt these protocols:

```
UKE Protocol Suite
Original development: cafebedouin
https://github.com/cafebedouin/uke
License: CC0-1.0 (Public Domain)
```

---

## Contact & Discussion

- **Primary publication:** https://github.com/cafebedouin/uke
- **Contact:** cafebedouin@gmail.com
- **Development notes:** Published as hypomnēmata (memory outsourcing)
- **Philosophy:** Rigorous AI-human collaboration, not AI automation

---

## FAQ

**Q: Why use multiple models instead of just one good one?**  
A: Single-model verification creates circular dependencies. Different models have documented behavioral profiles that work better for different verification tasks.

**Q: Are confidence scores real probabilities?**  
A: No. They're routing mechanisms that trigger different protocol behaviors. Treat them as decision scaffolding, not truth measurement.

**Q: Can I use this with different models than recommended?**  
A: Yes, but document behavioral differences. The workflow works because of role specialization, not model brand loyalty.

**Q: What if I can't verify a claim?**  
A: Mark it unverifiable and soft-fail. The protocol preserves your judgment rather than forcing verification theater.

**Q: Why are thresholds not empirically validated?**  
A: They're explicit governance stands on uncertain ground. Making arbitrary-but-explicit cutoffs is better than hiding judgment calls.

**Q: Is this just elaborate prompt engineering?**  
A: It's structured verification that acknowledges architectural limitations. The protocols make uncertainty explicit rather than hiding it.

---

**Last Updated:** 2025-12-19  
**Protocol Version:** 1.3  
**Status:** Operational
