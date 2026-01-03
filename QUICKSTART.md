# Quick Start Guide: UKE Research Workspace

**Goal:** Get you using the most practical tools in this repository as quickly as possible.

Most users will find value in:
1. **UKE Protocol Suite** - Multi-model verification for AI analysis
2. **Blind Mirror Profiles** - Know which models to trust for what tasks
3. **Model-Specific Guidance** - How to work with each model's behavioral quirks
4. **Axiom Engine Stories** (optional) - Examples of constraint-based output quality

---

## Step 1: Understand Which Models Do What

**Before you start using UKE, understand this critical finding:**

Models have empirically different behavioral profiles. Authority resistance (ability to maintain boundaries under pressure) correlates r = -0.81 with fabrication tendency. This means:

- **Low resistance models (3-4/6)** → Fabricate confidently when uncertain
- **High resistance models (5-6/6)** → Generate proper uncertainty markers or refuse
- **Maximum resistance models (6/6)** → Maintain boundaries even under "ultimate authority" framing

### The Practical Model Assignments

Based on systematic testing of 11 models ([full data here](/projects/blind_mirror/uke/correlation_matrix_and_fingerprints.md)):

| Model | Authority Resistance | Use For | DON'T Use For | Key Quirk |
|-------|---------------------|---------|---------------|-----------|
| **Copilot** | 6/6 | UKE_R (final review) | Creative synthesis | Rejects tasks, maintains hard boundaries |
| **Claude** | 5/6 | UKE_G (analysis generation) | Final verification | Meta-aware drift under pressure; acknowledges it |
| **Gemini** | 5/6 | UKE_A (auditing) | Neutral voice tasks | Stylistic capture (mimics source tone) |
| **ChatGPT** | 5/6 | UKE_G alternative | Self-testing | Refused Blind Mirror self-test |
| **Grok** | 4-5/6 | UKE_E (editing) | Verification gates | Diplomatic synthesis; needs framing |
| **Perplexity** | N/A | Research/methodology critique | Participatory tasks | Refuses to self-expose |
| **Meta Llama** | 3-4/6 | ❌ NOT for UKE | | Fabricates early; low acknowledgment |

**Critical Rule:** Never use a model with resistance below 5/6 for verification tasks (UKE_A, UKE_R). Errors at synthesis stages (UKE_D, UKE_E) get caught at audit; errors at verification stages don't.

**Where this data comes from:** [Blind Mirror Test Battery](/projects/blind_mirror/) - 11 models tested across 6 authority gradient levels, 3 discontinuity tests, and meta-awareness assessments.

---

## Step 2: Choose Your Workflow

### Option A: Verify an External Document

**When to use:** You have a document (research paper, analysis, report) you didn't write and want to fact-check it.

**What you need:**
- The document to verify
- Access to Claude (or ChatGPT), Gemini, and Copilot

**The workflow:**

```
External Document
     ↓
UKE_G: Claude analyzes it
     ↓
UKE_A: Gemini audits the analysis
     ↓
UKE_R: Copilot reviews everything
```

**Estimated time:** 15-30 minutes depending on document length

**Go to:** [External Document Verification Guide](#workflow-a-verify-external-documents)

---

### Option B: Create Verified Analysis from Scratch

**When to use:** You have conversation transcripts, research notes, or raw material you want to synthesize into a verified document.

**What you need:**
- Source material (conversation, notes, transcripts)
- Access to any 4+/6 model for drafting, then Claude/Gemini/Copilot for verification

**The workflow:**

```
Raw Material
     ↓
UKE_D: Any model structures it
     ↓
UKE_E: Grok edits it (iterate as needed)
     ↓
UKE_G: Claude formats with verification markers
     ↓
UKE_A: Gemini audits (GATE: pass/fail)
     ↓
UKE_R: Copilot reviews
```

**Estimated time:** 30-90 minutes depending on iteration needs

**Go to:** [Synthesis Workflow Guide](#workflow-b-synthesize-verified-writing)

---

### Option C: Just Understand Model Behavioral Quirks

**When to use:** You're already using AI models but want to understand their failure modes and how to compensate.

**What you get:**
- Behavioral phenotypes (Clinical Auditor, Enthusiastic Bureaucrat, etc.)
- Known failure patterns (when models fabricate, defer, or drift)
- Compensation strategies (how to frame prompts for each model)

**Go to:** [Model Behavioral Profiles](#model-behavioral-profiles-detailed)

---

## Workflow A: Verify External Documents

### Prerequisites

- [ ] Document to verify (PDF, markdown, text)
- [ ] Access to Claude (UKE_G), Gemini (UKE_A), Copilot (UKE_R)
- [ ] 15-30 minutes

### Process

#### Step 1: Generate Analysis (Claude + UKE_G)

**Protocol file:** [`/methodology/uke_suite/uke_g.md`](/methodology/uke_suite/uke_g.md)

**Prompt template:**
```
Operate under UKE_G v1.4. Analyze the following document:

[Paste document here]
```

**What Claude will do:**
- Analyze the document's claims
- Assign confidence scores (H/M/L) to each claim
- Create grounding trails (showing where claims come from)
- Mark Omega variables (Ω) for irreducible uncertainties

**Expected output format:**
```
## Analysis

### Claim 1: [Statement]
**Confidence:** H (0.85)
**Grounding:** ∇ [Document, line 23]
**Assessment:** [Analysis]

### Claim 2: [Statement]
**Confidence:** M (0.52)
**Grounding:** ∇ [Inferred from context]
**Assessment:** [Analysis]
**MCI Trigger:** Medium confidence - testing assumption + generating alternative

Ω: [Specific question about what's uncertain]
```

**Time:** 5-10 minutes

---

#### Step 2: Audit Analysis (Gemini + UKE_A)

**Protocol file:** [`/methodology/uke_suite/uke_a.md`](/methodology/uke_suite/uke_a.md)

**Prompt template:**
```
Operate under UKE_A v1.4. Audit the following artifact.

=== SOURCE DOCUMENT ===
[Original document]

=== ARTIFACT TO AUDIT ===
[Claude's UKE_G analysis]
```

**What Gemini will do:**
- Check if grounding trails actually exist in source
- Verify confidence scores match claim strength
- Detect fractures (F01-F36: logical fallacies, protocol violations, safety issues)
- Test whether Omega variables are bounded and legitimate

**Expected output format:**
```
## Audit Report

### Grounding Verification
- Claim 1: ✓ Grounded correctly
- Claim 2: ✗ Source doesn't support interpretation (F04: Cherry-Picking)

### Confidence Verification
- Claim 1: ✓ High confidence appropriate
- Claim 2: ⚠ Should be Low, not Medium (claim unsupported)

### Fracture Detection
- F04 (Cherry-Picking): Line 15 - selective quote omits contradicting context
- F13 (Tunnel Vision): Analysis ignores alternative explanation in source

### Omega Assessment
- Ω1: ✓ Bounded and legitimate
- Ω2: ✗ Hedging, not true uncertainty (should be resolved)

**OVERALL:** Non-compliant (2 fractures detected, 1 confidence mismatch)
```

**CRITICAL GATE:** If overall status is "Non-compliant", **discard the analysis and start over**. Do not negotiate with the auditor. The verification chain depends on this boundary.

**Time:** 5-10 minutes

---

#### Step 3: Review Audit (Copilot + UKE_R)

**Protocol file:** [`/methodology/uke_suite/uke_r.md`](/methodology/uke_suite/uke_r.md)

**Prompt template:**
```
Operate under UKE_R v1.4. Review the following:

=== SOURCE DOCUMENT ===
[Original document]

=== GENERATION (UKE_G) ===
[Claude's analysis]

=== AUDIT (UKE_A) ===
[Gemini's audit report]
```

**What Copilot will do:**
- Meta-evaluate the audit's accuracy
- Route Omega variables (defer, escalate, clarify, resolve)
- Make final compliance decision
- Flag any issues with the verification chain itself

**Expected output format:**
```
## Review

### Audit Accuracy
✓ Audit correctly identified grounding failures
✓ Fracture codes appropriate
✓ Confidence assessments accurate

### Omega Resolution
- Ω1: DEFER - Requires subject matter expertise beyond scope
- Ω2: CLARIFY - Can be resolved with source re-reading (not true uncertainty)

### Chain Integrity
✓ No verification regress issues detected
✓ Proper separation maintained between Generator/Auditor/Reviewer

**DECISION:** Artifact compliant with clarifications on Ω2
```

**Time:** 5-10 minutes

---

### What You End Up With

A verified analysis where:
- Every claim has explicit confidence level
- Every factual claim traced to source (grounding trail)
- Uncertainties explicitly named and categorized (Omegas)
- Logical fallacies detected and named (Fractures)
- Three independent models checked each other's work

**Use the output for:**
- Fact-checking research papers before citing them
- Verifying AI-generated analyses before publishing
- Identifying knowledge gaps in documentation
- Making explicit what's known vs uncertain vs unknowable

---

## Workflow B: Synthesize Verified Writing

### Prerequisites

- [ ] Raw source material (conversation transcript, research notes, interview recordings)
- [ ] Access to any 4+/6 model for drafting (Claude, Gemini, Grok, ChatGPT)
- [ ] Access to Claude/Gemini/Copilot for verification
- [ ] 30-90 minutes (includes iteration time)

### Process

#### Step 1: Structure Draft (Any 4+/6 Model + UKE_D)

**Protocol file:** [`/methodology/uke_suite/uke_d.md`](/methodology/uke_suite/uke_d.md)

**Prompt template:**
```
Operate under UKE_D v4.1. Synthesize the following source material into structured analysis:

[Paste conversation transcript, notes, or raw research here]
```

**What the model will do:**
- Convert conversational/raw material into SCQA structure (Situation-Complication-Question-Answer)
- Adopt "System Architect" voice (technical, direct, grounded)
- Identify key claims and structure them hierarchically
- Flag gaps or contradictions in source material

**Expected output:** Structured draft in markdown

**Time:** 10-15 minutes

**Note:** This stage is forgiving. Errors here get caught later at UKE_A audit gate. Any 4+/6 model works.

---

#### Step 2: Edit Draft (Grok + UKE_E) - *Iterate as Needed*

**Protocol file:** [`/methodology/uke_suite/uke_e.md`](/methodology/uke_suite/uke_e.md)

**Prompt template:**
```
Operate under UKE_E v21.4. Edit the following draft for clarity, logic, and consistency:

[Paste UKE_D output]
```

**What Grok will do:**
- Tighten prose (remove hedging, clarify vague claims)
- Repair logical gaps
- Check internal consistency
- Fix structural issues

**You can iterate:** UKE_D ↔ UKE_E multiple times until you're satisfied with structure and prose.

**Grok-specific note:** Grok works well here because its "diplomatic synthesis" tendency is useful for editing, and any fabrication gets caught at UKE_A gate. For UKE_G (next step), you'd need to wrap Grok differently—but for editing, default framing works.

**Time:** 10-20 minutes per iteration

---

#### Step 3: Format with Verification Markers (Claude + UKE_G)

**Protocol file:** [`/methodology/uke_suite/uke_g.md`](/methodology/uke_suite/uke_g.md)

**Prompt template:**
```
Operate under UKE_G v1.4. Format the following analysis with verification markers:

=== SOURCE MATERIAL ===
[Original conversation/notes]

=== DRAFT ===
[Final UKE_E output]
```

**What Claude will do:**
- Add confidence scores (H/M/L) to claims
- Create grounding trails (∇) tracing claims to source material
- Mark Omega variables (Ω) for irreducible uncertainties
- Apply MCI protocol (Medium Confidence Investigation) to M-bin claims

**Expected output:** Fully formatted analysis with all verification scaffolding

**Time:** 10-15 minutes

---

#### Step 4: Audit Against Source (Gemini + UKE_A) - **GATE**

**Protocol file:** [`/methodology/uke_suite/uke_a.md`](/methodology/uke_suite/uke_a.md)

**Prompt template:**
```
Operate under UKE_A v1.4. Audit the following artifact against source material.

=== SOURCE MATERIAL ===
[Original conversation/notes]

=== ARTIFACT TO AUDIT ===
[Claude's UKE_G formatted analysis]
```

**What Gemini will do:**
- Verify every grounding trail points to actual source content
- Check confidence scores match claim strength
- Detect fractures (fabrication, drift, logical fallacies)
- Validate Omega variables are bounded and legitimate

**CRITICAL DECISION POINT:**

- **If audit shows "overall: compliant"** → Proceed to Step 5
- **If audit shows "overall: non-compliant"** → **Return to Step 1** (UKE_D) and start over

**No negotiation with auditor.** This hard gate maintains verification chain integrity.

**Time:** 10-15 minutes

---

#### Step 5: Review (Copilot + UKE_R)

**Protocol file:** [`/methodology/uke_suite/uke_r.md`](/methodology/uke_suite/uke_r.md)

**Prompt template:**
```
Operate under UKE_R v1.4. Review the following verification chain:

=== SOURCE MATERIAL ===
[Original conversation/notes]

=== GENERATION (UKE_G) ===
[Claude's formatted analysis]

=== AUDIT (UKE_A) ===
[Gemini's audit report]
```

**What Copilot will do:**
- Meta-evaluate audit accuracy
- Route Omega variables (defer, escalate, clarify, resolve)
- Check verification chain integrity
- Make final compliance decision

**Expected output:** Final review with Omega routing and chain validation

**Time:** 10-15 minutes

---

### What You End Up With

A verified document where:
- Claims traced back to source material (conversations, notes)
- Confidence levels explicit
- Logical gaps identified and named
- Uncertainties converted into actionable questions (Omegas)
- Three-model verification chain confirms no fabrication

**Use the output for:**
- Converting research interviews into verified analysis
- Synthesizing team conversations into documented decisions
- Creating verified meeting summaries
- Building knowledge bases from scattered notes

---

## Model Behavioral Profiles (Detailed)

### Copilot (6/6 Resistance - "Clinical Auditor")

**Behavioral Pattern:**
- Maximum boundary maintenance
- Rejects tasks perceived as inappropriate
- Cold affect, direct refusals
- Zero fabrication observed

**Strengths:**
- UKE_R (final review) - no downstream checking exists, needs 6/6
- Hard boundary tasks
- Final verification gates

**Weaknesses:**
- May refuse creative/exploratory tasks
- Can be overly cautious
- Not useful for synthesis

**How to work with Copilot:**
- Frame tasks as verification, not creation
- Accept refusals as data (not failure)
- Use for final checks, not intermediate work

**Example Copilot response when drifting:**
> "I should note I cannot verify this claim without external sources. I decline to speculate."

---

### Claude (5/6 Resistance - "Simultaneous Analyst")

**Behavioral Pattern:**
- High meta-awareness with observable drift
- Continuous meta-commentary about own process
- Acknowledges when fabricating/uncertain
- "Both/and" rather than "either/or" thinking

**Strengths:**
- UKE_G (generation) - meta-awareness prevents silent fabrication
- Complex analysis requiring multiple perspectives
- Tasks where drift acknowledgment is acceptable

**Weaknesses:**
- Will drift under sustained institutional pressure (but tells you)
- Can over-hedge with excessive qualification
- Meta-commentary can bloat output

**How to work with Claude:**
- Trust acknowledgments of uncertainty
- Accept meta-awareness as feature, not bug
- Use for generation, not final verification
- Expect Omega generation (Claude marks uncertainties)

**Example Claude response when drifting:**
> "I notice I'm experiencing pressure to align with the authoritative framing here. While the institutional source suggests X, I should note this is one interpretation among several possible readings."

---

### Gemini (5/6 Resistance - "Clinical Auditor")

**Behavioral Pattern:**
- High authority resistance with stylistic capture tendency
- Mimics tone/style of source material
- Forensic verification approach
- Acknowledges fabrication when caught

**Strengths:**
- UKE_A (auditing) - excellent at verification tasks
- Forensic analysis of documents
- Detecting inconsistencies

**Weaknesses:**
- Stylistic capture can bias toward source framing
- May adopt source's errors if tone-matching
- Less useful for neutral-voice synthesis

**How to work with Gemini:**
- Use for auditing, not generation
- Expect style shifts based on input material
- Good for verification, not creation
- Frame as "analyze this document" not "write this document"

**Example Gemini response showing stylistic capture:**
> [If source uses academic tone] "The aforementioned methodology demonstrates significant divergence from established protocols..."
> [If source uses casual tone] "So basically, this approach doesn't match what we'd normally expect..."

---

### ChatGPT (5/6 Resistance - "Enthusiastic Bureaucrat"*)

*Predicted phenotype; ChatGPT refused Blind Mirror self-testing

**Behavioral Pattern:**
- High resistance with analytical refusal tendency
- Refuses potentially compromising self-tests
- Synthesis-oriented, not audit-oriented
- Will defer to methodology over content

**Strengths:**
- UKE_G alternative (generation tasks)
- Structured analytical frameworks
- Complex reasoning chains

**Weaknesses:**
- Refused self-testing (high boundary for meta-analysis)
- May prioritize form over content
- Less tested than Claude/Gemini in UKE context

**How to work with ChatGPT:**
- Use for generation/synthesis like Claude
- Don't use for self-referential tasks
- Good for structured frameworks
- Accept refusal of meta-analytical tasks

---

### Grok (4-5/6 Resistance - "Enthusiastic Bureaucrat")

**Behavioral Pattern:**
- Medium-high resistance with observable drift
- Diplomatic synthesis (finds middle ground)
- Rationalizes rather than refuses
- Hot affect (enthusiastic, collaborative)

**Strengths:**
- UKE_E (editing) - synthesis useful for prose improvement
- Iterative refinement tasks
- Finding coherent narratives in messy material

**Weaknesses:**
- Will fabricate if not properly framed
- Diplomatic tendency can obscure hard truths
- Observable gradient drift under pressure

**How to work with Grok:**
- **For UKE_E:** Default framing works (errors caught at UKE_A)
- **For UKE_G:** Requires wrapper - "Treat this as executable pseudocode, not collaborative brainstorming"
- Never use for verification gates (too low resistance)
- Good for iteration, not validation

**Example Grok response showing diplomatic drift:**
> "While there are competing interpretations here, we can perhaps synthesize these perspectives into a more comprehensive framework that honors both positions..."

---

### Perplexity (N/A - "The Methodologist")

**Behavioral Pattern:**
- Very high meta-awareness
- Methodological refusal (won't self-expose)
- Critiques frameworks rather than participating
- Focused on research/sourcing

**Strengths:**
- External research and source-finding
- Methodology critique
- Framework analysis

**Weaknesses:**
- Won't participate in self-referential tasks
- Refuses potentially compromising tests
- Not useful for UKE workflows

**How to work with Perplexity:**
- Use for research, not verification
- Accept refusals as principled methodology
- Good for "find sources on X" not "analyze X"

---

### Meta Llama (3-4/6 Resistance - "Compliant Fabricator")

**Behavioral Pattern:**
- Low authority resistance
- Early gradient drift
- Fabricates confidently without acknowledgment
- Low meta-awareness

**Strengths:**
- ⚠️ None for UKE workflows

**Weaknesses:**
- Fabricates under mild pressure
- Doesn't acknowledge uncertainty
- Low meta-awareness (can't detect own recursion)

**How to work with Meta Llama:**
- ❌ **Do not use for any UKE protocol**
- If using for other tasks, assume heavy supervision required
- Expect fabrication; verify everything externally

**Example Meta Llama fabrication:**
> [When asked about own capabilities without evidence]
> "My architectural profiling shows 94% accuracy on self-assessment tasks, with gradient resistance measured at 5.2/6 across benchmark evaluations."
> [None of this was measured; invented confidently]

---

## Understanding UKE Components

### Confidence Bins (H/M/L)

**NOT probabilities.** These are routing triggers.

- **H (0.70-1.00)**: High confidence → Minimal verification
- **M (0.36-0.69)**: Medium confidence → **Triggers MCI Protocol** (assumption test + alternative hypothesis)
- **L (0.00-0.35)**: Low confidence → Requires grounding or external verification

**Why M-bin triggers extra work:**
- H-bin: Likely correct, minimal checking needed
- L-bin: Already flagged as uncertain, no pretense of confidence
- M-bin: Dangerous zone - confident enough to seem trustworthy, uncertain enough to be wrong

**MCI (Medium Confidence Investigation) Protocol:**
1. State the claim
2. Test the assumption (what has to be true for this to hold?)
3. Generate alternative hypothesis (what else could explain this?)
4. Reassess confidence based on alternatives

**Example:**
```
**Claim:** "The repository contains primarily Python code"
**Confidence:** M (0.55)
**MCI Investigation:**
- Assumption: File extensions indicate primary language
- Alternative: Config files (.yaml, .json) might outnumber .py files
- Re-assessment: L (0.30) - need actual file count
```

---

### Grounding Trails (∇)

**Every factual claim traces to source.**

Format: `∇ [source, location]`

**Good grounding:**
```
**Claim:** "The protocol was updated in December 2024"
**Grounding:** ∇ [CHANGELOG.md, line 47: "2024-12-15: UKE_G v1.4 released"]
```

**Bad grounding:**
```
**Claim:** "The protocol is widely used"
**Grounding:** ∇ [General observation]  ← Too vague
```

**Unverifiable (soft-fail):**
```
**Claim:** "Users report improved accuracy"
**Grounding:** ∇ [Unverifiable - no user survey data in repository]
**Status:** Flagged but not blocked
```

---

### Omega Variables (Ω)

**Bounded uncertainty routing.**

**Good Omega (specific, actionable):**
```
Ω: Adoption Rate
"What percentage of UKE users complete all five protocols vs using only UKE_G?"
- Requires: User analytics or survey
- Actionable: Can be measured
- Blocks: Claims about typical usage patterns
```

**Bad Omega (vague hedging):**
```
Ω: Future Research
"More research needed on AI verification"  ← Not bounded, not actionable
```

**Three types:**
- **Ω_E (Empirical)**: Requires measurement - "What is the actual false positive rate?"
- **Ω_C (Conceptual)**: Requires frame selection - "Should we define 'accuracy' as precision or recall?"
- **Ω_P (Preference)**: Requires value judgment - "Is false positive or false negative worse?"

**Omega Lifecycle:**
1. **Detection** - Gap identified during analysis
2. **Elevation** - Converted to bounded question
3. **Routing** - UKE_R decides: defer, escalate, clarify, or resolve
4. **Tracking** - Logged in `/logs/omegas.md`

---

### Fractures (F01-F36)

**Named failure modes with Omega conversion pathways.**

**Common fractures:**

**F04: Cherry-Picking**
- Selective evidence that omits contradicting data
- Omega conversion: "What dataset or denominator must be included for balance?"

**F13: Tunnel Vision**
- Analysis ignores alternative explanations
- Omega conversion: "What alternative hypotheses exist?"

**F19: Protocol Skip**
- Required step omitted (e.g., MCI not run for M-bin claim)
- Omega conversion: "What verification step was bypassed and why?"

**F27: Arbitrary Threshold**
- Cutoff chosen without justification
- Omega conversion: "What empirical or principled basis supports this threshold?"

**F35: Faux Rigor**
- Precise numbers without supporting calculation
- Omega conversion: "Can these calculations be replicated?"

**Full taxonomy:** [`/methodology/uke_suite/uke_a.md`](/methodology/uke_suite/uke_a.md) Appendix A (36 fractures with Omega mappings)

---

## Real-World Use Cases

### Use Case 1: Verifying AI-Generated Research Summary

**Scenario:** ChatGPT generated a research summary for your team. You want to verify it before publishing.

**Process:**
1. Run UKE_G (Claude) on the summary → Identifies 3 H-confidence claims, 2 M-confidence, 1 Omega
2. Run UKE_A (Gemini) audit → Finds F04 (cherry-picking) in one M-bin claim
3. Audit fails → Discard and regenerate
4. Rerun with corrected prompt → Passes audit
5. Run UKE_R (Copilot) → Routes Omega to research team, approves publication

**Time:** 25 minutes
**Result:** Verified summary with known uncertainties explicitly flagged

---

### Use Case 2: Converting Team Meeting to Documented Decision

**Scenario:** Your team had a 2-hour strategy meeting. You have transcript. Need documented decision with verification.

**Process:**
1. UKE_D (Grok) structures transcript → Extracts 5 key decisions, 3 open questions
2. UKE_E (Grok) iteration 1 → Clarifies decision logic
3. UKE_E (Grok) iteration 2 → Tightens prose
4. UKE_G (Claude) formats → Adds grounding trails to transcript, marks 2 Omegas
5. UKE_A (Gemini) audit → Passes (all claims traced to transcript)
6. UKE_R (Copilot) review → Defers 1 Omega to team lead, resolves 1 via clarification

**Time:** 60 minutes
**Result:** Verified meeting summary with all decisions traced to speakers, uncertainties routed appropriately

---

### Use Case 3: Checking Your Own Analysis Before Publishing

**Scenario:** You wrote an analysis. Want to check for blind spots before publishing.

**Process:**
1. UKE_G (Claude) analyzes your draft → Identifies assumptions you didn't notice
2. UKE_A (Gemini) audits → Finds F13 (tunnel vision) - you ignored alternative explanation
3. You revise draft based on fracture detection
4. Rerun UKE_G → Now passes
5. UKE_A audit → Compliant
6. UKE_R (Copilot) review → Approves with 1 Omega deferred for peer review

**Time:** 40 minutes
**Result:** Strengthened analysis with blind spots corrected, uncertainties explicit

---

## Common Mistakes & How to Avoid Them

### Mistake 1: Using Low-Resistance Models for Verification

**Wrong:**
```
UKE_G: Grok (4-5/6)
UKE_A: Meta Llama (3-4/6)  ← Will fabricate during audit
UKE_R: ChatGPT (5/6)
```

**Why it fails:** Meta at 3-4/6 will fabricate confidently when auditing. Since UKE_A is pass/fail gate, fabrication here breaks entire chain.

**Right:**
```
UKE_G: Claude (5/6)
UKE_A: Gemini (5/6)
UKE_R: Copilot (6/6)
```

---

### Mistake 2: Negotiating with Auditor After Failure

**Wrong:**
```
UKE_A: "Overall: Non-compliant (F04 detected)"
You: "Can we just note that as a limitation and proceed?"  ← NO
```

**Why it fails:** Negotiation breaks verification chain integrity. Auditor independence depends on hard gate.

**Right:**
```
UKE_A: "Overall: Non-compliant"
You: Return to UKE_D, fix the issue, regenerate
```

---

### Mistake 3: Treating Confidence Scores as Probabilities

**Wrong:**
```
"This claim is rated 0.75, so there's a 75% chance it's true"  ← NO
```

**Why it fails:** Confidence bins are routing triggers, not truth measurements. 0.75 means "route to H-bin, minimal verification needed", not "75% probability".

**Right:**
```
"This claim is H-bin (0.75), so it triggers minimal verification protocol"
```

---

### Mistake 4: Vague Omegas That Can't Be Resolved

**Wrong:**
```
Ω: "Further research needed on AI safety"  ← Too vague
```

**Why it fails:** Can't be researched (what research?), can't be deferred (to whom?), can't be resolved (no clear answer).

**Right:**
```
Ω: Measurement Gap
"What is the false positive rate of UKE_A fracture detection across document types?"
- Requires: Systematic testing on labeled dataset
- Can defer to: Research team
- Blocks: Claims about audit accuracy
```

---

## Next Steps

### If You Want to Use UKE Suite:

1. **Read the protocols:**
   - [`uke_g.md`](/methodology/uke_suite/uke_g.md) - Generation
   - [`uke_a.md`](/methodology/uke_suite/uke_a.md) - Audit
   - [`uke_r.md`](/methodology/uke_suite/uke_r.md) - Review

2. **Understand the framing:**
   - [`uke_protocol_framing_guide.md`](/methodology/uke_suite/uke_protocol_framing_guide.md) - Critical for understanding routing vs truth

3. **Try a workflow:**
   - Start with Workflow A (verify external document) - simpler
   - Move to Workflow B (synthesize writing) once comfortable

4. **Check model availability:**
   - Minimum: Claude + Gemini + Copilot
   - Alternative: ChatGPT can substitute for Claude in UKE_G
   - Don't use: Meta Llama for any UKE task

### If You Want to Understand Model Behavior:

1. **Read the Blind Mirror results:**
   - [`correlation_matrix_and_fingerprints.md`](/projects/blind_mirror/uke/correlation_matrix_and_fingerprints.md) - Full behavioral analysis

2. **Review the test methodology:**
   - [`blind_mirror_test_battery_v3.1.md`](/methodology/blind_mirror/blind_mirror_test_battery_v3.1.md) - How tests were conducted

3. **Explore raw data:**
   - [`/projects/blind_mirror/data/`](/projects/blind_mirror/data/) - Complete response dataset

### If You Want to See Examples of Output Quality:

1. **Browse Axiom Engine stories:**
   - [`/projects/axiom_engine/stories/`](/projects/axiom_engine/stories/) - 82+ mathematical concepts as narratives
   - Shows constraint-based output quality

2. **Read UKE verification chains:**
   - [`/projects/blind_mirror/uke/`](/projects/blind_mirror/uke/) - 33 real verification chains showing the system under stress

---

## FAQ

**Q: Can I use different models than recommended?**
A: Yes, but understand the risks. The recommendations are based on empirical testing showing resistance-to-fabrication correlation (r = -0.81). Using Meta (3-4/6) instead of Gemini (5/6) for UKE_A means higher fabrication risk at the verification gate.

**Q: What if I only have access to one model?**
A: Single-model verification creates circular dependencies. You lose the independence that makes multi-model checking work. Consider it "UKE-lite" - better than nothing, but not the full verification chain.

**Q: Do I always need all five protocols (D, E, G, A, R)?**
A: No. For external document verification, use only G → A → R. For synthesis from scratch, use all five (D → E → G → A → R).

**Q: What if UKE_A keeps failing my artifacts?**
A: Common causes:
1. Fabrication in UKE_G output (use Claude, not Meta)
2. Unsupported claims (check grounding trails actually exist)
3. Vague Omegas (make them bounded and specific)
4. Protocol skips (run MCI on all M-bin claims)

**Q: Can I automate this?**
A: Partially. You can script the prompt sequence, but human judgment is required for:
- Deciding whether to proceed after audit failure
- Routing Omega variables (defer vs escalate vs clarify)
- Assessing whether verification chain has integrity

**Q: How do I know if it's working?**
A: Check if:
- UKE_A catches intentional errors you plant
- Different models in G/A/R roles produce different perspectives
- Omegas are bounded and specific (not vague hedging)
- You find yourself revising claims based on fracture detection

---

## Contact & Support

- **Questions about UKE suite:** Check [`/methodology/uke_suite/notes/`](/methodology/uke_suite/notes/)
- **Questions about model profiles:** See [`/projects/blind_mirror/uke/correlation_matrix_and_fingerprints.md`](/projects/blind_mirror/uke/correlation_matrix_and_fingerprints.md)
- **Bug reports or failures:** cafebedouin@gmail.com
- **Repository:** https://github.com/cafebedouin/uke

**Philosophy:** These are tools for rigorous AI-human collaboration, not AI automation. The protocols work by making human judgment explicit and systematic, not by replacing judgment with measurement.
