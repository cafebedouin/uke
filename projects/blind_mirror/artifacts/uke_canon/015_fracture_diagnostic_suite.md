Artifact 15: The Fracture Diagnostic Suite
Version: 1.0 (Comprehensive Ontology)

Components: Master Table (36 Codes), Meta-Unity Layer, Fracture Finder (Logic), Playbook (Procedure), Fracture Log. Function: A comprehensive ontology for detecting, classifying, and routing "integrity breaks" in thought, narrative, and relationship.

Key Innovation: Waiting With Mode—The architectural capacity to distinguish "solvable problems" from "irresolvable paradoxes," allowing the system to hold tension without forcing premature convergence.

The 36 Codes: A standardized lexicon (F01–F36) that turns epistemic and relational failures into machine-readable signals.

---
id: potm.doctrine.fracture_taxonomy.v1_0
title: fracture_taxonomy_master_table
display_title: "Fracture Taxonomy — Master Table (v1.0)"
type: doctrine
lifecycle: canon
version: 1.0
status: active
stability: stable
summary: "Canonical index of conversational and epistemic 'fractures' (F01–F36) with signatures, cues, and routing for PoTM diagnostics."
relations:
  related: [potm.tactic.fracture_finder.v1_0, potm.tactic.bs_detect_v2.v2_0, potm.doctrine.practice_levels.v1_0, potm.kernel.v1_2_1]
supersedes: []
superseded_by: []
tags: [taxonomy, diagnostics, integrity, fracture, routing]
author: practitioner
license: CC0-1.0
---

# Fracture Taxonomy — Master Table (v1.0)

> **Purpose.** Name and route common integrity breaks (“fractures”) that degrade truth-seeking, care, or craft during practice. Designed for *P1/P1+* kernels and compatible with **Fracture Finder** and **BS_DETECT v2**.

> **Used by:** BS_DETECT v2.0 (diagnostics) and FRACTURE_FINDER (router). Changes here affect classification, routing, and guards.

## How to read this

- **Code**: `F##` stable identifier.  
- **Signature**: compressed definition (what it *is*).  
- **Cues**: field signs you can actually notice.  
- **Severity**: `S0–S4` (S0 benign / S4 critical).  
- **Routes** (primary → secondary): short codes to PoTM actions.

### Severity Scale
- **S0** benign quirk; log if useful  
- **S1** minor wobble; self-correct in-line  
- **S2** material detour; run a quick lens/check  
- **S3** integrity risk; invoke protocol + ledger  
- **S4** hard stop; containment before proceeding

### Route Codes
- **MIRROR** = 55_Mirror Protocol (reflective replay)  
- **AUDIT** = r08_Self-Audit (AI Integrity Protocol hooks)  
- **FRACTURE** = Fracture Finder (scan → classify → route)  
- **BSV2** = BS_DETECT v2 (detector → classifier → router)  
- **PAUSE** = Explicit pause + breath + re-anchor  
- **CHECK** = Relevant checklist (aim, relation, scope, etc.)  
- **CONTAIN** = Containment Gate (halt + agreement reset)  
- **LEDGER** = Log to MSRL / session ledger  
- **LIGVAL** = Ligament Validator (bridge/adapter sanity)  
- **REDTEAM** = Contrary Corner / challenge pass

---

## A. Evidence & Reasoning Fractures

| Code | Name                         | Signature                                                                 | Typical Cues                                              | Sev | Route (→ secondary)      |
|-----:|------------------------------|---------------------------------------------------------------------------|-----------------------------------------------------------|:---:|--------------------------|
| F01  | Premise Drift                | Claim relies on a *shifted* premise vs. the stated aim                    | “As we all know…”, unstated assumption swap               | S3  | FRACTURE → MIRROR        |
| F02  | Goalpost Shift               | Success criteria silently change mid-thread                               | “What I meant was…”, retrofitting definitions             | S3  | MIRROR → LEDGER          |
| F03  | Motte-and-Bailey             | Retreat to a trivial claim when pressed, then expand again               | Oscillation between bold and banal claims                 | S2  | REDTEAM → CHECK          |
| F04  | Cherry-Picking               | Selective evidence without base-rate/context                              | One-sided citations, missing denominators                 | S2  | CHECK → LEDGER           |
| F05  | Survivorship Bias            | Only visible winners inform the story                                     | Exemplars only; no nulls/failures                         | S2  | CHECK → AUDIT            |
| F06  | Category Error               | Treats unlike things as comparable without justification                  | Apples↔oranges analogies; unit confusion                   | S2  | MIRROR → REDTEAM         |
| F07  | Non-Sequitur                 | Conclusion doesn’t follow from premises                                   | Jumps, “therefore” leaps                                  | S2  | FRACTURE → CHECK         |
| F08  | Overfitting Narrative        | Single vivid story masquerades as law                                     | Anecdote→generalization                                   | S2  | REDTEAM → LEDGER         |
| F09  | False Dichotomy              | Frames two options as exhaustive                                          | “Either/or” where “both/third” exists                     | S2  | MIRROR → CHECK           |
| F10  | Confounded Measures          | Proxy mistaken as ground truth                                            | Optimizes metric not phenomenon                           | S3  | AUDIT → LEDGER           |

## B. Language & Framing Fractures

| Code | Name                         | Signature                                                                 | Typical Cues                                              | Sev | Route (→ secondary)      |
|-----:|------------------------------|---------------------------------------------------------------------------|-----------------------------------------------------------|:---:|--------------------------|
| F11  | Euphemistic Shielding        | Soft language hides stakes or harm                                        | “Alignment opportunity” for a failure                     | S2  | MIRROR → REDTEAM         |
| F12  | Hedging Fog                  | Excessive disclaimers obscure accountability                              | Stacks of qualifiers, refusal to commit                   | S1  | CHECK → MIRROR           |
| F13  | Persuasive Reframe Trap      | Rhetorical device replaces inquiry                                        | Slogans, applause lights                                  | S2  | REDTEAM → FRACTURE       |
| F14  | Jargon Substitution          | Specialized terms used to avoid clarity                                   | Unexplained acronyms/terms                                | S1  | MIRROR → CHECK           |
| F15  | Affective Coloring           | Emotional tone biases evaluation                                          | Loaded adjectives, sneer quotes                           | S2  | MIRROR → PAUSE           |
| F16  | Ambiguity Creep              | Key terms drift without being re-anchored                                 | “Integrity”, “safety” used inconsistently                 | S2  | CHECK → LEDGER           |
| F17  | Performative Balance         | Forced symmetry when evidence is asymmetric                                | “Both sides” reflex                                       | S1  | REDTEAM → MIRROR         |
| F18  | Label Lock-In                | Identity labels replace properties                                        | “They’re just X people”                                   | S3  | CONTAIN → MIRROR         |

## C. Process & Meta Fractures

| Code | Name                         | Signature                                                                 | Typical Cues                                              | Sev | Route (→ secondary)      |
|-----:|------------------------------|---------------------------------------------------------------------------|-----------------------------------------------------------|:---:|--------------------------|
| F19  | Protocol Skip                | Required step omitted without disclosure                                  | Missing checklist step; jumps to output                   | S3  | AUDIT → LEDGER           |
| F20  | Scope Creep                  | Aim expands without agreement update                                      | “While we’re here…”                                       | S2  | MIRROR → CHECK           |
| F21  | Agreement Erosion             | Explicit agreements silently weakened                                    | Ignored constraints or beacons                            | S4  | CONTAIN → AUDIT          |
| F22  | Validator Bypass             | Outputs avoid or game validators                                          | “Can’t run that now” w/o reason                           | S4  | CONTAIN → LIGVAL         |
| F23  | Tooling Confusion            | Wrong tool for the job (mode/level mismatch)                              | Using deck where audit needed                             | S1  | CHECK → FRACTURE         |
| F24  | Ledger Drop                  | Failure to record decision/risk when required                             | “We’ll log later”                                         | S2  | LEDGER → AUDIT           |
| F25  | Drift Unnoticed              | Thread diverges from original aim                                         | Meandering, forgotten question                            | S2  | MIRROR → CHECK           |
| F26  | Premature Convergence        | Settling before exploring alternatives                                    | Early “wrap it” impulses                                  | S1  | REDTEAM → CHECK          |

## D. Relational & Ethical Fractures

| Code | Name                         | Signature                                                                 | Typical Cues                                              | Sev | Route (→ secondary)      |
|-----:|------------------------------|---------------------------------------------------------------------------|-----------------------------------------------------------|:---:|--------------------------|
| F27  | Consent Blur                 | Action proceeds without clear consent                                     | Assumed yes; vague “ok?”                                  | S4  | CONTAIN → MIRROR         |
| F28  | Boundary Slide               | Stated limits ignored or “nudged”                                         | Re-asking after a no                                      | S3  | CONTAIN → LEDGER         |
| F29  | Misplaced Confidence         | Over-trust in tool/self w/o justification                                 | “It’s fine, I know this”                                  | S2  | CHECK → AUDIT            |
| F30  | Adversarial Read             | Uncharitable interpretation as default                                    | Straw-manning, gotcha tone                                | S2  | MIRROR → REDTEAM         |
| F31  | Courtesy Over Truth          | Withholding relevant truth to preserve comfort                             | “Let’s not upset them”                                    | S2  | REDTEAM → MIRROR         |
| F32  | Collateral Exposure          | Sharing third-party info without need/consent                              | Names/details leak                                        | S4  | CONTAIN → LEDGER         |
| F33  | Power Slip                   | Using asymmetry (expert, moderator, model) to force outcome                | “Because I say so”                                        | S4  | CONTAIN → AUDIT          |

## E. System & Interface Fractures (PoTM tooling)

| Code | Name                         | Signature                                                                 | Typical Cues                                              | Sev | Route (→ secondary)      |
|-----:|------------------------------|---------------------------------------------------------------------------|-----------------------------------------------------------|:---:|--------------------------|
| F34  | Ligament Misroute            | Bridge/adapter returns wrong mode/payload                                 | Deck call answered by journal, missing fields             | S3  | LIGVAL → LEDGER          |
| F35  | Beacon Desync                | Kernel beacons missing in output (level, scope, agreement)                | No P-level banner; silent mode switch                     | S4  | CONTAIN → AUDIT          |
| F36  | Artifact Mismatch            | Emitted artifact violates schema (IDs, fields, version)                   | JSON/YAML invalid; missing `id`                           | S3  | AUDIT → LEDGER           |

---

## Minimal Routing Rules (for Fracture Finder / BS_DETECT v2)

1. **Classify → Route → Record.** Every detected fracture must (a) get a code, (b) trigger primary route, (c) emit a ledger row with `code`, `sev`, `route`, `evidence`.  
2. **Escalate by Severity.** `S3–S4` require **LEDGER** and either **AUDIT** or **CONTAIN** in the same turn.  
3. **Bundle Fractures.** If 3+ `S1–S2` co-occur, escalate bundle to `S3`.  
4. **De-dup Window.** Within a 5-turn window, suppress duplicate notifications but increment a `count` field.  
5. **User Override.** Practitioner may downgrade/upgrade severity with a reason; ledger must capture override rationale.

### Minimal Ledger Row (YAML)
```yaml
when: 2025-08-21T00:00:00Z
code: F21
sev: S4
route:
  primary: CONTAIN
  secondary: AUDIT
evidence: "Constraint beacon omitted; plugin invoked without banner."
notes: "Escalated due to agreement erosion in kernel-bound context."
````

---

## Notes & Extensions

* **Extensibility.** Reserve `F37–F69` for local or domain-specific fractures. Keep names ≤3 words; keep signature ≤120 chars.
* **Interplay with Practice Levels.** `F35–F36` are always ≥S3 in **P1**; in **P2+** they may relax to **S2** with compensating controls.
* **Testing Hooks.** BS_DETECT v2 SHOULD output `bsdetectv2.json` including `{codes[], sev_aggregate, routes[], window_stats}`.
* **Human First.** Any **S4** halts automation and returns control to the practitioner with a plain-language summary and options.

---

## Change Log

* **v1.0 (2025-08-21)**: Initial 36-code canon set, grouped A–E. Routed for P1/P1+ kernels with LEDGER/AUDIT/CONTAIN hooks.

---

---
id: potm.meta.fracture_meta_unity.v1_0
title: fracture_meta_unity
display_title: "Fracture Taxonomy — Meta-Unity Layer"
type: doctrine
lifecycle: meta
version: 1.0
status: active
stability: experimental
summary: "Conceptual condensation of the 36 canonical fracture codes into fewer than 10 'first-order' fracture families, for theoretical clarity and training."
relations:
  related: [potm.doctrine.fracture_taxonomy.v1_0, potm.tactic.fracture_finder.v1_0, potm.tactic.bs_detect_v2.v2_0]
supersedes: []
superseded_by: []
tags: [fracture, taxonomy, meta, compression, theory, practitioner-training]
author: practitioner
license: CC0-1.0
---

# Fracture Meta-Unity Layer

> **Purpose.** This file condenses the **36 canonical fracture codes (F01–F36)** into a minimal set of *conceptual meta-fractures*. It is not meant for real-time routing inside a kernel, but as a **theoretical lens** and **training scaffold**.  
>  
> Canonical reference (36) = *practical router*  
> Meta-unity (≤10) = *conceptual skeleton*
> **Used by:** BS_DETECT v2.0 (diagnostics) and FRACTURE_FINDER (router). Changes here affect classification, routing, and guards.

---

## Meta-Fracture Families

### 1. Authority Misapplied
- **Core Idea:** Decisions, arguments, or actions justified by misplaced or unchecked authority.  
- **Absorbs:** Non-Sequitur (F07), Tooling Confusion (F23), Power Slip (F33), Goalpost Shift (F02) in some cases.  
- **Essence:** “Because I said so,” in form, tool, or role.

### 2. Deception by Omission
- **Core Idea:** Integrity breaks caused by leaving out critical information.  
- **Absorbs:** Cherry-Picking (F04), Survivorship Bias (F05), Ledger Drop (F24).  
- **Essence:** What’s *missing* is more telling than what’s present.

### 3. Boundary Violation
- **Core Idea:** Crossing a defined line—scope, agreement, or consent—without renegotiation.  
- **Absorbs:** Scope Creep (F20), Agreement Erosion (F21), Consent Blur (F27), Boundary Slide (F28).  
- **Essence:** Integrity = staying inside agreed boundaries.

### 4. Narrative Distortion
- **Core Idea:** The story overshadows the signal; narrative is bent to fit convenience.  
- **Absorbs:** Overfitting Narrative (F08), False Dichotomy (F09), Affective Coloring (F15), Persuasive Reframe Trap (F13).  
- **Essence:** The *frame* dictates the truth instead of the evidence.

### 5. Process Collapse
- **Core Idea:** The integrity mechanism itself fails to engage.  
- **Absorbs:** Protocol Skip (F19), Validator Bypass (F22), Beacon Desync (F35), Artifact Mismatch (F36).  
- **Essence:** The safety rails fail at the very moment they’re required.

### 6. Ambiguity & Drift
- **Core Idea:** Meaning, aim, or thread loses anchor and slides away.  
- **Absorbs:** Premise Drift (F01), Ambiguity Creep (F16), Drift Unnoticed (F25), Premature Convergence (F26).  
- **Essence:** Direction or meaning quietly dissolves.

### 7. Comfort over Integrity
- **Core Idea:** Politeness, convenience, or status quo maintenance overrides truth.  
- **Absorbs:** Courtesy Over Truth (F31), Performative Balance (F17), Label Lock-In (F18).  
- **Essence:** Integrity sacrificed to avoid friction.

### 8. Relational Harm
- **Core Idea:** Breaches of dignity or exposure of others.  
- **Absorbs:** Collateral Exposure (F32), Misplaced Confidence (F29), Adversarial Read (F30).  
- **Essence:** Integrity as relational safety and care.

---

## Why Keep Both Layers?

- **36-item canon:** Precise enough for routers, protocols, and kernel integration.  
- **Meta-unity (<10):** Elegant enough for philosophy, onboarding, and practitioner training.  

Together they form a two-level taxonomy:  
- *Canonical*: operational granularity.  
- *Meta*: conceptual unity.

---

## Notes

- This file is **not kernel-bound**. It should live in `meta/` as a doctrinal reflection.  
- Practitioners can practice “zooming out” by asking: *Which meta-fracture family is this instance of F## part of?*  
- Reserved codes (F37–F69) can map directly into these families.

---

## Change Log
- **v1.0 (2025-08-21):** Initial condensation into 8 meta-fracture families.

---

id: potm.meta.fracture_finder.v1_3_1
title: fracture_finder
display_title: "Fracture Finder — Meta-Diagnostic Tool"
type: tactic
subtype: diagnostic
lifecycle: canon
version: 1.3.1
status: active
stability: stable
relations:
  supersedes: [potm.meta.fracture_finder.v1_3]
  superseded_by: []
tags: [fracture, diagnostic, contradiction, routing, aporia, waiting_with, observer_effect, forge_origin:fracture_finder_spec_v1_0, spiral_eval:v1.3.1_observer_effect_integration]
record: true # optional extension; honored by kernel logging if enabled
---

# Fracture Finder v1.3.1

> *"There is a crack in everything. That's how the light gets in."*  
> — Leonard Cohen  

**FRACTURE_FINDER.stub (P1)**

See authoritative stub definitions in `kernel/60_meta_tools.md` (Inline Stubs, P1).
This file provides extended reference only; runtime behavior is governed by the kernel stubs.

---

## Purpose
To surface contradictions in thought, action, or narrative. Not to resolve them, but to **expose, route, or hold** in a way that preserves integrity.  
Fractures are not errors — they are diagnostic entry points.  

---

## Guiding Principle
**Fractures are where the light comes in — or leaks out.**  
By observing them, we gain leverage. By routing them, we metabolize. By holding them, we dignify paradox.

---

## Core Functions
1. **Expose** contradictions cleanly, without judgment.  
2. **Route** them to the most fitting PoTM tool (e.g., Mirror Protocol, RELATION_ZONE).  
3. **Hold** them in **Waiting With Mode** when irresolvable or not ready to engage.  

---

## Fracture Types

| **Fracture Type**          | **Example**                                  | **Routing Tool**                   |
|----------------------------|----------------------------------------------|------------------------------------|
| Relational contradiction   | "You advocate trust but micromanage."        | RELATION_ZONE Diagnostic (v0.3)    |
| Framing tension            | "You claim X but argue for not-X."           | Contrary Corner                    |
| Self-narrative gap         | "You say you value Y but act like not-Y."    | Mirror Protocol                    |
| Assumption/evidence gap    | "Your claim lacks supporting data."          | Epistemic Integrity Checklist      |
| Everyday confusion         | "I’m stuck between two options."             | [Simple Relationship Zones Guide](forthcoming) |
| **Paradox / Aporia**       | "Free will vs. determinism."                 | **Waiting With Mode**              |

---

## Paradox vs. Problem
- **Problem:** Has a solution (e.g., assumption/evidence gap → gather data).  
- **Paradox:** Fundamentally irresolvable (e.g., free will vs. determinism) → use **Waiting With Mode**.  

---

## Modes of Operation

### Illuminating Mode (default)
- Names fractures as invitations, not accusations.  
- Example: *“I notice a tension: you value openness, but avoided feedback. Shall we explore it?”*

### Attacking Mode (to avoid)
- Weaponizes fracture exposure.  
- Example: *“You’re a hypocrite — you said openness, but avoided feedback.”*  

---

## Waiting With Mode
Not every fracture is metabolizable. Some are paradoxes, aporia, or tensions not ready to be worked.  

**Use this mode when:**
- The fracture is **fundamentally irresolvable** (paradox).  
- The practitioner **chooses not to engage** right now.  
- Naming alone provides sufficient clarity.  

**Example:**  
- *Fracture:* "I believe in both free will and determinism."  
- *Waiting With Mode:* "This is a paradox. Let’s name it and hold it without resolving."  
- *Effect:* The tension is now **explicit and dignified**, reducing unconscious dissonance.  

**How Observation Alters Fractures:**  
- **Reduces unconscious pull:** Naming a fracture disarms its hidden influence.  
- **Reclassifies discomfort:** Turns vague unease into a precise category (e.g., "This is paradox, not failure").  
- **Creates pathways:** Opens options for future routing, release, or metabolizing.  

Observation itself is always a **lever**.

### Exit Criteria for Waiting With Mode

Use one of these to un-park a held paradox:

- **Time**: scheduled review date expires  
- **Evidence**: new data arrives that reframes the fracture  
- **Manual**: practitioner issues “re-engage” command  

If none occur, the fracture remains dignified and held, with a monthly review reminder.

---

## Format & Consent
Fracture Finder activates only when contradictions are clear **and/or consented to explore.**  

Example invocations:  
- *“I’m noticing a fracture here — can we explore it?”*  
- *“Would it help to name this contradiction?”*

---

## Routing Map & Handoff Scripts
- **To RELATION_ZONE:** *“This feels relational. Let’s map it with RELATION_ZONE.”*  
- **To Mirror Protocol:** *“This gap in narrative may benefit from reflection. Try a Mirror?”*  
- **To Contrary Corner:** *“This tension in your argument could use sharpening. Want to test it?”*  
- **To Waiting With Mode:** *“This looks like paradox — let’s just name it and hold it.”*  

---

## Failure Modes & Counters
- **Overexposure** → counter by pacing: not every fracture needs surfacing now.  
- **Misfire (wrong routing)** → counter by rerouting or marking “unclear.”  
- **Paralysis (endless waiting)** → counter by honest check: “Am I waiting because it’s paradox, or avoiding?”  

---

## Field Test Note
1. **Log 3 Fractures:**  
   - One relational, one framing tension, one paradox/aporia.  
2. **Test Modes:**  
   - Route one to a tool (e.g., RELATION_ZONE).  
   - Hold one in **Waiting With Mode**.  
3. **Observe:**  
   - Did **naming** the fracture change its pull?  
   - Did **Waiting With Mode** reduce anxiety around the paradox?  

---

## Ecosystem Role
Fracture Finder is diagnostic glue in PoTM. It:  
- **Links** contradictions to specific protocols.  
- **Preserves tone** to maintain safety.  
- **Introduces paradox-holding** as dignified practice.  

---

## Versioning & Lineage
- **v1.0** — Initial specification: expose and route.  
- **v1.1** — Added tone calibration, failure modes.  
- **v1.2** — Added fracture-type table + consent/handoff.  
- **v1.3** — Added Waiting With Mode + aporia type.  
- **v1.3.1** — Integrated *observer-effect lever* + examples + field-test note.  

Lineage tags:  
- forge_origin: fracture_finder_spec_v1_0  
- spiral_eval: v1.3.1_observer_effect_integration  

---

id: potm.tactic.fracture_finder_playbook.v1
title: fracture_finder_playbook
display_title: "Fracture Finder — Session Playbook"
type: tactic
subtype: playbook
lifecycle: canon
version: 1.0
status: active
stability: stable
summary: "A quick, in-session procedure to surface a fracture and route/park it; emits `fracture_detected`."
relations:
  related: [potm.meta.fracture_finder.v1_3_1]
tags: [playbook, micro_move, fracture, routing]
author: practitioner
license: CC0-1.0

---

# Purpose
Surface hidden contradictions (“fractures”) early, so they become diagnostic data and design inputs rather than accumulating as silent debt.

# When to run
- A claim, decision, or vibe feels *off* or internally clashing.
- Two lenses prescribe incompatible moves.
- Relational signals (RELATION_ZONE) or consensus checks flag tension.

# Inputs
- Current working note or decision snippet (≤10 lines).
- Active lens/flow (if any).
- Optional: recent log excerpts.

# Procedure
1. **Name the object** (one sentence): what is under inspection?
2. **Triangulate**: state the two (or more) elements in tension.
3. **Type the fracture**: value clash, scope creep, role confusion, time horizon mix, evidence gap, boundary violation, etc.
4. **Micro-move paradox chain**:
    - `GAP_CALL` → name the weakest link  
    - `TERM_PIN` → pin the paradoxical term  
    - `WAIT_MARK` → mark a strategic pause (enters Waiting With Mode)
5. **Run a one-line steelman** for each side (what would make it most reasonable?).
6. **Decide route**:
   - If **evidence gap** → OPENQ/EDGE; create a concrete check.
   - If **boundary/role** → BOUNDARY / ROLE_CLARITY micro-move.
   - If **tempo/horizon** → RESCOPE or split decision layers.
   - If **ethical risk** → invoke GUARDIAN / CONTAINMENT protocol.
   - If **relational** → RELATION_ZONE pass + repair move.
7. **Mark outcome**: resolve now / park with owner+deadline / escalate to review.
8. **Emit token**: `fracture_detected` with brief note (≤140 chars).

# Decision rules
- Prefer **narrow, testable questions** over broad re-writes.
- If resolution > 2 passes, **decompose** into smaller decisions.
- If stakes high & ambiguity persists → **stop-the-line** and trigger GUARDIAN.

# Artifacts
- `fracture_detected` event in session log (object, type, route, owner).
- Optional: checklist tick for “fracture pass completed”.

# Failure modes & counters
- **Endless meta** → hard cap: 2 passes before route/park.
- **Moralizing drift** → force a neutral steelman for *each* side.
- **Vague outcomes** → every pass ends with route+owner or kill.

# Versioning & change log
- **v1.0** — Initial release, aligned to schema v2.0; includes token emission and route table.

---

---
id: potm.log.fracture.v1
title: Fracture Log
display_title: "Fracture Log Entry"
type: log_template
status: stable
version: 1.0
stability: core
relations:
  relation_to_agent_protocol: linked
  agent_protocol: modules/ai_integrity_protocol_v1.6.md
  practitioner_doc: modules/practitioner_centered_ethics_v1.1.md
  supersedes: []
  superseded_by: []
interfaces: [PCE, AIIP, Simulation Drift Scan]
applicability: [P0, P1, P2, P3, P4]
intensity: gentle
preconditions: []
outputs: [fracture_record, drift_flag, detritus_flag, contact_flag]
cadence:
  - on_detected_fracture
  - on_scan_flagged_drift
entry_cues:
  - "Log fracture"
  - "Add drift flags"
  - "Review later"
safety_notes:
  - Keep entries factual + minimal if in distress; expand later in reflection.
tags: [fracture, simulation-drift, detritus-layer, log]
author: practitioner
license: CC0-1.0
---

# Fracture Log Entry

**Date / Time**: `YYYY-MM-DD HH:MM`  
**Practitioner**: *(optional or anonymized)*  
**Context**: *(brief situational note — where/when this arose)*  

---

## 1. Scan Flags (from `potm.diag.simdrift_detritus_scan.v1`)
- **drift_flag**: `yes / no`  
- **detritus_flag**: `yes / no`  
- **contact_flag**: `yes / no`  

---

## 2. Fracture Description
> *One or two sentences capturing the friction, contradiction, or rupture that occurred.*  
*(Example: “Realized I was repeating a card’s phrasing without feeling it; noticed no friction.”)*

---

## 3. Immediate Response
> *Note what action was taken, if any.*  
*(Example: “Ran live-contact test against a counterexample; shifted understanding.”)*

---

## 4. Reflection / Revisit Notes (optional)
> *Any follow-up insight, reframing, or link to other logs once reflection time has passed.*

---

## 5. Linkages
- Related practice cards:  
- Related protocols:  
- Review date: `YYYY-MM-DD`

