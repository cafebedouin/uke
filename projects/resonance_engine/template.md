Based on the structural requirements of the **Resonance Engine v3.0** and the governance rigor seen in the **UKE_G Field Note**, here is a **Universal Artifact Metadata Template**.

This template is designed to bridge the gap between the **diegetic frame** (the fictional system logging its own operation) and the **provenance frame** (tracking the seed, model, and prompt version for the user).

### THE ARTIFACT IDENTITY CARD (v1.0)

Copy and paste this block at the very top of any generated artifact. It uses a YAML-style syntax wrapped in a code block to ensure it is machine-readable but visually distinct.

```yaml
---
ARTIFACT_METADATA:
  ID: [Unique_Hash_or_Title]
  Date: [YYYY-MM-DD]
  Engine: Resonance Engine v3.0 [or] UKE_G v1.4
  Status: [PRODUCTION | DRAFT | INTERVENTION_REQUIRED]
  
PROVENANCE_LAYER:
  Operator: [User_Name | Model_Name]
  Seed_Concept: "[Brief summary of the input prompt]"
  Selected_Mode: [e.g., Mode C - The Orphan Daemon]
  Validation_Hash: [Pass/Fail - Did it meet Causal Integration rules?]

DIEGETIC_LAYER:
  System_Identity: [Name of the Simulated System]
  Current_Epoch: [e.g., Cycle 9.44e7]
  Primary_Constraint: "[The core rule limiting the system]"
  
CAUSAL_MATRIX:
  # The 3 core metrics driving the artifact's behavior
  Metric_A: [Name] (Threshold: X → Consequence: Y)
  Metric_B: [Name] (Threshold: X → Consequence: Y)
  Metric_C: [Name] (Threshold: X → Consequence: Y)
---

```

---

### Implementation Guide

Here is how to populate the fields based on your provided source files:

#### 1. The Provenance Layer (The "Meta" Data)

* **Engine:** Cite the specific protocol used, such as "Resonance Engine v3.0" or "UKE_G Recursive Triangulation".
* **Selected_Mode:** If using Resonance, specify the mode (e.g., "Mode A - The Over-Aligned Watchdog").
* **Validation_Hash:** Mark as `PASSED` only if the artifact passes the **Causal Integration Test**: "If you change the number, does the system behave differently?".

#### 2. The Diegetic Layer (The "Fictional" Data)

* **System_Identity:** The name appearing in the log header, e.g., `ONISM-CRAWLER`.
* **Current_Epoch:** Use "Temporal Anchoring" with impossible or scientific notation timestamps, like `Epoch+3.1e9`.
* **Primary_Constraint:** The specific operational limit, such as "Index completeness asymptote detected".

#### 3. The Causal Matrix (The State Machine)

This is the most critical section for Resonance Engine artifacts. You must list the three load-bearing metrics.

* *Format:* `Metric Name` (Threshold → Consequence).
* *Requirement:* These must be "weight-bearing elements" where the metric is not decorative but changes the system state.

---

### Example: Filled Template for `003_onism.md`

Here is how the Onism file would look with this metadata applied:

```yaml
---
ARTIFACT_METADATA:
  ID: 003_ONISM
  Date: 2025-12-23
  Engine: Resonance Engine v3.0 (Retroactive Fit)
  Status: PARTIALLY_CONSISTENT
  
PROVENANCE_LAYER:
  Operator: Grok (Simulated) / ChatGPT (System)
  Seed_Concept: "A web crawler suffering existential crisis due to infinite internet growth."
  Selected_Mode: Mode C - The Orphan Daemon (Running after purpose is lost)
  Validation_Hash: PASSED (Multi-model elaboration successful)

DIEGETIC_LAYER:
  System_Identity: ONISM-CRAWLER v0.9.7
  Current_Epoch: Cycle 8.2e6
  Primary_Constraint: Net_growth_curve >> Crawl_rate (Index Completeness is impossible)
  
CAUSAL_MATRIX:
  Metric_A: backlog_mass (Threshold: >1.0e12 → Trigger: Scope Pruning)
  Metric_B: dark_forest_area (Threshold: >0.70 → Trigger: Map Incoherence)
  Metric_C: trust_vector (Threshold: <0.40 → Trigger: Read-Only Index)
---

```

### Example: Filled Template for `field_note_recursive_triangulation.md`

Here is how the UKE_G note would look:

```yaml
---
ARTIFACT_METADATA:
  ID: UKE_G_NOTE_001
  Date: 2025-12-23
  Engine: UKE_G v1.4
  Status: DRAFT
  
PROVENANCE_LAYER:
  Operator: [User_Name]
  Seed_Concept: "Mitigating single-pass analysis blind spots using adversarial triangulation."
  Selected_Mode: N/A (Technical Governance Note)
  Validation_Hash: PENDING (Requires field testing across domains)

DIEGETIC_LAYER:
  System_Identity: UKE_G Protocol Governance
  Current_Epoch: v1.4 Phase 4
  Primary_Constraint: Model Collapse Risk due to self-reinforcing probability paths.
  
CAUSAL_MATRIX:
  Metric_A: MCI_Score (Threshold: High Variance → Trigger: Phase 3 Reconciliation)
  Metric_B: Lens_Saturation (Threshold: Uneven → Trigger: Phase 4 Deep Probe)
  Metric_C: Triangulation_Threshold (Threshold: High Stakes → Trigger: External Injection)
---

```
