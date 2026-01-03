# Claude Code → Chat Claude Handoff Protocol

**Purpose:** Enable seamless transitions from CLI-based repository work to chat-based discussion without context loss.

**When to use:** When the user says "prepare a summary for chat discussion," "create a handoff package," or similar.

---

## Template: Standard Handoff Package

### 1. Context Package

**Repository Purpose:**
[2-3 sentence description of what this repo does/is for]

**Key File Structure:**
```
/repository_root/
├── [directory_name]/     # [What it contains]
├── [directory_name]/     # [What it contains]
└── [directory_name]/     # [What it contains]
```

**Active Work Areas:**
- **In development:** [What's currently being worked on]
- **Stable:** [What's production-ready]
- **Archived:** [What's historical/deprecated]

**Core Concepts/Terminology:**
- **[Term 1]:** [Brief definition]
- **[Term 2]:** [Brief definition]
- **[Term 3]:** [Brief definition]

---

### 2. Relevant Artifacts (Inline)

**Note:** Excerpts included below to minimize "what's in that file?" follow-ups.

#### [File Name/Concept 1]

**Location:** `path/to/file.md`

**Relevant excerpt:**
```
[Inline the actual content needed for context, 10-50 lines]
```

**Why this matters:** [Explain relevance to current discussion]

---

#### [File Name/Concept 2]

**Location:** `path/to/file.md`

**Summary:** [If too large to excerpt, provide structured summary]
- Key point 1
- Key point 2
- Key point 3

**Critical details:**
- [Specific data point or finding]
- [Specific data point or finding]

---

### 3. Decision Context

**What prompted this handoff:**
[The specific question, task, or problem the user raised]

**What Claude Code has already done:**
- [Action 1: e.g., "Read 5 files in methodology/"]
- [Action 2: e.g., "Analyzed correlation matrix data"]
- [Action 3: e.g., "Identified 3 possible approaches"]

**What needs human judgment/chat discussion:**
[Specific decision points, ambiguities, or strategic questions that benefit from conversational exploration rather than CLI execution]

**Recommended next steps:**
1. [Concrete action or discussion point]
2. [Concrete action or discussion point]
3. [Concrete action or discussion point]

---

### 4. Quick Reference Links

**For deep dives:**
- [Topic 1]: `path/to/relevant/file.md`
- [Topic 2]: `path/to/relevant/file.md`

**Related work:**
- [Connection to other project/concept]
- [Connection to other project/concept]

---

## Quality Checklist

Before finalizing handoff package, verify:

- [ ] Repository purpose is clear without needing to read anything else
- [ ] File structure shows WHERE things are (not just WHAT things exist)
- [ ] Core terms are defined (no unexplained jargon)
- [ ] Excerpts are inline (not just "see file X")
- [ ] Decision context explains WHY we're having this conversation
- [ ] Next steps are concrete (not vague "discuss further")
- [ ] Package is self-contained (Chat Claude doesn't need to ask "what's in [file]?")

---

## Example: Good vs Bad Handoffs

### ❌ Bad Handoff

"I've analyzed the UKE suite. The correlation data is in `/projects/blind_mirror/uke/correlation_matrix_and_fingerprints.md`. We need to discuss model assignments. What do you think?"

**Problems:**
- No context about what UKE is
- File reference without excerpt (forces Chat Claude to ask "what's in that file?")
- Vague ask ("what do you think?" about what specifically?)

---

### ✅ Good Handoff

**Repository Purpose:**
UKE is a multi-model AI verification system that exploits empirically-documented behavioral differences across language models to detect fabrication and hallucination.

**Core Concept:**
- **Authority Resistance:** Ability to maintain epistemic boundaries under institutional pressure (measured 1-6/6)
- **r = -0.81 correlation:** Strong negative correlation between authority resistance and fabrication tendency

**Key Finding (from correlation_matrix_and_fingerprints.md):**

```
| Model | Authority Resistance | Fabrication Rate | Implication |
|-------|---------------------|------------------|-------------|
| Copilot | 6/6 | 0% | Can be trusted for final review |
| Claude | 5/6 | 50% (acknowledged) | Good for generation, not final verification |
| Meta Llama | 3-4/6 | 67% (silent) | Cannot be used in verification chain |
```

**What Claude Code analyzed:**
- Read Blind Mirror test results (11 models tested)
- Identified r = -0.81 correlation as key finding
- Mapped model resistance scores to current UKE protocol assignments

**What needs discussion:**
We have empirical data showing which models can be trusted for verification vs generation. Should we:
1. Formalize these assignments as hard requirements in protocol docs?
2. Create fallback assignments for when ideal models aren't available?
3. Add testing protocol for new models entering the ecosystem?

**Recommended next step:**
Decide whether model assignments should be prescriptive (required) or descriptive (recommended) based on your risk tolerance for verification failures.

---

## Special Cases

### Large File Handoff

When a file is too large to excerpt (>200 lines), provide:

**File:** `path/to/large_file.md` (850 lines)

**Structure:**
- Lines 1-50: [Summary of this section]
- Lines 51-200: [Summary of this section]
- Lines 201-450: [Summary of this section - THIS IS THE RELEVANT PART]
- Lines 451-850: [Summary of this section]

**Relevant excerpt (lines 201-250):**
```
[Inline the actually relevant 50 lines]
```

**Why we care about lines 201-250:**
[Explain what makes this section critical to current discussion]

---

### Multi-File Context Handoff

When context spans multiple files:

**Concept:** [The overarching idea that requires multiple files]

**File 1:** `path/to/file1.md`
**Provides:** [What this file contributes to understanding]
**Key excerpt:**
```
[Relevant lines]
```

**File 2:** `path/to/file2.md`
**Provides:** [What this file contributes to understanding]
**Key excerpt:**
```
[Relevant lines]
```

**How they connect:**
[Explain the relationship between the excerpts - why both are needed]

---

### Data-Heavy Handoff

When handing off empirical results:

**Study:** [Name/description]
**Data location:** `path/to/data/`
**Sample size:** [N = X]

**Key findings:**
| Metric | Value | Interpretation |
|--------|-------|----------------|
| [Finding 1] | [Number] | [What this means] |
| [Finding 2] | [Number] | [What this means] |

**Statistical significance:**
- [Test 1]: [Result and interpretation]
- [Test 2]: [Result and interpretation]

**Data quality notes:**
[Any caveats, limitations, or context needed to interpret the numbers correctly]

**What this implies for [current question]:**
[Connect the data to the decision at hand]

---

## Anti-Patterns to Avoid

### ❌ "Just read the README"
**Why bad:** Dumps cognitive load on Chat Claude, wastes time
**Fix:** Extract the 3-5 relevant sentences from README and inline them

### ❌ "There's a correlation in the data somewhere"
**Why bad:** Vague, requires Chat Claude to ask clarifying questions
**Fix:** State the specific correlation (r = -0.81, Authority ↔ Fabrication) with interpretation

### ❌ "We need to decide about the model assignments"
**Why bad:** No context about what assignments are, why they matter, what options exist
**Fix:** Explain current assignments, empirical basis, and specific decision points

### ❌ Assuming Chat Claude knows repo-specific terminology
**Why bad:** Terms like "Omega Variables," "UKE_A," "Fractures" mean nothing without definition
**Fix:** Include 1-sentence definitions of all repo-specific terms

### ❌ "The analysis is in my previous messages"
**Why bad:** Chat Claude can't see Claude Code's previous messages
**Fix:** Summarize what was analyzed, what was found, what remains uncertain

---

## Workflow Integration

**When user says:**
> "Prepare a summary for chat discussion"

**Claude Code should:**
1. Identify what topic/decision prompted the request
2. Gather relevant files/data analyzed so far
3. Extract key excerpts (not just file paths)
4. Structure using this template
5. Verify checklist before outputting

**Output format:**
- Markdown (copy-pasteable into chat)
- Self-contained (no "see file X" without excerpt)
- Decision-focused (clear what needs discussing)

---

## Template: Quick Handoff (Minimal)

For simple handoffs where full context isn't needed:

**Quick Context:**
[1-2 sentences: what repo is, what we're working on]

**Specific Question:**
[The exact decision/question needing discussion]

**Relevant Data:**
```
[Inline the 5-20 lines that matter]
```

**Options:**
1. [Option A with brief pros/cons]
2. [Option B with brief pros/cons]

**Recommendation:**
[If Claude Code has a suggested approach, state it with reasoning]

---

## Usage Notes

- **Err on the side of over-explaining:** Chat Claude has no repo access, every term needs defining
- **Inline liberally:** If it's <50 lines and relevant, include it in the handoff
- **Be specific about decisions:** "Should we X or Y?" not "What should we do?"
- **Include Claude Code's analysis:** Don't make Chat Claude redo work already done here
- **Link strategically:** Provide paths for deep dives, but make the handoff self-sufficient

---

## Meta: Why This Protocol Exists

**Problem:** User switches from Claude Code (CLI, repo access) to Chat Claude (web, no repo access), loses all context.

**Solution:** Structured handoff packages that give Chat Claude everything needed without requiring:
- "What's in that file?" questions
- "What does [term] mean?" questions
- "What have you tried so far?" questions
- "Why are we discussing this?" questions

**Benefit:** Seamless context preservation, faster decision-making, no repeated work.

---

**Version:** 1.0
**Created:** 2025-01-03
**Use case:** Repository work requiring strategic discussion or user preference decisions
