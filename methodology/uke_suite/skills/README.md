# UKE Suite Skills Package

This package contains 7 skills for the UKE (Universal Knowledge Evaluator) Suite multi-model orchestration workflow.

## Overview

The UKE Suite is a multi-model workflow for creating verified, high-quality content. It routes work through specialized protocols optimized for different AI models and phases.

## Skills Included

### 1. uke-suite.skill (Orchestration)
**For:** You (the practitioner)
**Purpose:** Workflow orchestration, routing decisions, model assignment guidance
**Contains:**
- Complete workflow decision tree
- Model-to-protocol assignments
- Routing logic for failures
- References: Omega Variable documentation, Framing Guide, Fracture↔Omega Matrix

**Use when:** You need to decide which protocols to apply, understand the workflow, or route between phases.

### 2. uke-d.skill (Drafting)
**For:** Claude (primary)
**Purpose:** Synthesize conversations into structured documents with System Architect voice
**Key features:**
- SCQA structure (Situation-Complication-Question-Answer)
- Objective empathy through Recognition Clause
- But/Therefore transitions
- No first/second person pronouns

**Use when:** Converting conversation insights into initial drafts.

### 3. uke-t.skill (Template)
**For:** Claude (default model)
**Purpose:** Optional scaffolding for general audience writing
**Key features:**
- **Required:** Omega (Ω) tracking
- **Optional:** One-Inch Frame, SCQA, tables
- Permissive design - use what fits

**Use when:** Drafting for publication needs structure, but allows flexibility.

### 4. uke-e.skill (Editing)
**For:** Grok (primary), any model
**Purpose:** Logic verification, grounding check, prose compression (30-40%)
**Key features:**
- Source Material Verification Protocol (SMVP)
- Fracture repair (F01-F36)
- Iceberg rule (compression)
- Semantic spine check

**Use when:** Draft needs verification and compression.

### 5. uke-g.skill (Grounding)
**For:** Claude (primary)
**Purpose:** Multi-perspective verification, claim grounding, web search integration
**Key features:**
- T1 behaviors (mandatory): CHECK, CONTRARY, EDGE, FACTS
- T2 format (optional): Glyphs and metadata
- Confidence calibration triggers
- Web search for post-cutoff verification

**Use when:** Claims need verification or multi-perspective analysis required.

### 6. uke-a.skill (Audit)
**For:** Gemini (primary), any model
**Purpose:** Fracture detection, Omega elevation, protocol compliance verification
**Key features:**
- Fracture taxonomy (F01-F36)
- Log-content verification
- Grounding trail checks
- Fracture↔Omega conversion matrix

**Use when:** Verifying UKE_G outputs, detecting simulation vs execution.

### 7. uke-r.skill (Review)
**For:** Copilot (primary), any model
**Purpose:** Governance decisions, routing recommendations
**Key features:**
- Solo audit (lightweight)
- MSRL survivorship evaluation
- Omega resolution protocol
- Safety assessment

**Use when:** Making routing decisions, conducting reviews, resolving Omegas.

## Installation

1. Choose which skills you need based on your workflow tier:
   - **Tier 1** (quick capture): uke-d.skill
   - **Tier 2** (publishable): uke-d, uke-e, uke-g
   - **Tier 3** (full enchilada): all skills

2. Load skills into appropriate platforms:
   - **Claude.ai:** uke-suite, uke-d, uke-g, uke-t
   - **Grok:** uke-e
   - **Gemini:** uke-a
   - **Copilot:** uke-r

3. Skills are loaded via the platform's skill management interface (varies by platform).

## Workflow Quick Reference

### Tier 1: Quick Conversation Capture (~5 min)
```
Conversation → UKE_D → Done
```

### Tier 2: Publishable Content (~20-30 min)
```
Conversation → UKE_D → UKE_E → UKE_G → Done
```

### Tier 3: High-Stakes Content (~60-90 min)
```
Conversation → UKE_D → (UKE_T) → UKE_E → UKE_G → UKE_A → UKE_R → Done
```

## Key Concepts

### The Omega Variable (Ω)
Marks irreducible uncertainty - where analysis cannot progress without external input.

**Format:** `Ω: [Label] — [Question]`

**Why it matters:** Transforms vague uncertainty into actionable questions, points to research directions, enables clean handoffs.

### Pipeline Tracker
Every output includes:
```
[x] uke_d | [ ] uke_e | [ ] uke_g | [ ] uke_a | [ ] uke_r
```
Shows what's been done and what comes next.

### T1 vs T2 (UKE_G)
- **T1 (behaviors):** What actually matters - testing assumptions, generating contrary positions
- **T2 (format):** Scaffolding that makes verification possible

## Critical Frame

These protocols are **routing mechanisms**, not truth measurements:
- Confidence scores trigger behaviors (not probability estimates)
- Formulas create comparable inputs (not objective measurements)
- Thresholds are explicit governance stands (not empirical claims)

See `uke-suite.skill → references/framing_guide.md` for full explanation.

## Model Assignments (Recommended)

| Protocol | Primary Model | Rationale |
|----------|---------------|-----------|
| UKE_D | Claude | Synthesis, structural clarity |
| UKE_T | Claude | Template application |
| UKE_E | Grok | Compression, logic repair |
| UKE_G | Claude | Multi-perspective analysis |
| UKE_A | Gemini | Audit, fracture detection |
| UKE_R | Copilot | Review, routing |

Adjust based on your access and observed performance.

## Support

For questions, issues, or contributions:
- GitHub: https://github.com/cafebedouin/uke/tree/main/methodology/uke_suite
- License: CC0-1.0 (Public Domain)

## Version Information

- uke-suite: v1.0
- uke-d: v1.4
- uke-e: v2.4
- uke-g: v1.4
- uke-a: v1.4
- uke-r: v1.4
- uke-t: v1.5 (Revised - Permissive)

Built with skill-creator from Anthropic's skill examples.
