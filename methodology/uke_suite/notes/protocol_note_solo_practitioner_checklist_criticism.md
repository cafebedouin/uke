Here is the **UKE Solo Practitioner Checklist**. This 1-page cheat sheet is designed to help you run the full adversarial workflow by yourself, using LLMs to simulate the necessary role separation.

---

# UKE Solo Practitioner Checklist

**Protocol:** UKE_SOLO v1.0
**Objective:** Run adversarial refinement on a single draft using AI separation of concerns.

---

### §1. Pre-Flight Check (The Candidate)

*Is this work ready for the machine?*

* [ ] **Maturity:** Is the draft coherent enough to have a discernible architecture? (If it's just notes, stop. Go to drafting.)
* [ ] **Stakes:** Is this work important enough to justify the energy cost of this protocol?
* [ ] **Detachment:** Am I willing to see this draft disassembled? (If you need validation, send to a friend, not this protocol.)

---

### §2. Position 1: The Audit (UKE_C)

**Operator:** LLM "A" (e.g., Gemini Pro / GPT-4o)
**Goal:** Neutral pattern mapping. No judgment allowed.

**Setup:**

* [ ] Open a **fresh** context window.
* [ ] Upload/Paste the Draft.

**The Prompt Seed:**

> "Act as a neutral auditor (UKE_C). Your goal is **systematic inventory**, not evaluation.
> 1. **Map the Architecture:** Outline the structural hierarchy (sections, flow).
> 2. **Identify Patterns:** List recurring symbols, metaphors, or terminology.
> 3. **Flag Omissions:** What concepts are introduced but dropped?
> 4. **Detect Omega Variables:** What questions does the text raise but fail to resolve?
> 5. **Output Style:** Bulleted lists, visible data. Do not offer praise or criticism. Just report what is there."
> 
> 

**Review Output:**

* [ ] Did it find patterns I didn't consciously put there?
* [ ] Is the "Omega Variable" list accurate?
* [ ] **Action:** Copy this output. Save as `[Draft_Name]_Audit.txt`.

---

### §3. Position 2: The Opinion (UKE_O)

**Operator:** LLM "B" (e.g., Claude 3.5 Sonnet / Different Instance)
**Goal:** Prosecutorial attack based on evidence.

**Setup:**

* [ ] Open a **fresh** context window (Critical: Do not use the Audit window).
* [ ] Upload/Paste the Draft.
* [ ] Upload/Paste `[Draft_Name]_Audit.txt`.

**The Prompt Seed:**

> "Act as an adversarial critic (UKE_O). Review the attached draft and the audit report.
> 1. **The Knife Sentence:** Write one ruthless sentence summarizing why this piece fails to achieve its potential.
> 2. **Weaponize the Audit:** Use the patterns identified in the audit to prove your critiques. (e.g., 'The text relies on Symbol X, but fails to define it until Section 4').
> 3. **Collapse the Omegas:** Look at the 'unresolved questions' from the audit. Argue that these aren't mysteries, they are failures of rigor.
> 4. **Stance:** You are not a polite editor. You are a prosecutor. Make the strongest case against this draft."
> 
> 

**Review Output:**

* [ ] Does the "Knife Sentence" hurt? (If yes, it's working.)
* [ ] Are the attacks grounded in the text, or hallucinated?
* [ ] **Action:** Copy this output. Save as `[Draft_Name]_Opinion.txt`.

---

### §4. Position 3: Metabolization (The Human)

**Operator:** You
**Goal:** Strategic extraction.

**The Review:**

* [ ] **Read the Knife Sentence.** Does it identify a fundamental flaw in the premise?
* [ ] **Check the Pattern Flags.** Did the Audit find "decorative" sections that carry no weight? -> *Mark for deletion.*
* [ ] **Check the Attacks.** Did the Opinion correctly identify a contradiction? -> *Mark for resolving.*

**The Decision Matrix:**

* [ ] **Reject:** The critic misunderstood the goal. (Be honest: did they misunderstand, or did you write it poorly?)
* [ ] **Compress:** The "decorative" parts identified by the Audit can be cut.
* [ ] **Rebuild:** The "Omega Variables" are load-bearing flaws. I need to rewrite the core argument to solve them.

---

### §5. The Refactor (UKE_R)

**Operator:** You + LLM "A" (Re-engaged)
**Goal:** Final Polish.

**Setup:**

* [ ] Return to LLM "A" (The neutral auditor).
* [ ] Feed it your "Metabolization Notes" (e.g., "I want to cut Section 2, focus on the 'Noose' metaphor, and shorten by 50%").

**The Prompt Seed:**

> "I have processed the critique. Here is the plan: [Insert Plan].
> Please help me draft the **Revised Version**.
> Focus on: Compression, enforcing the core metaphor, and resolving the Omega variables identified earlier."

---

### §6. Post-Mortem

* [ ] Is the new version significantly shorter/sharper?
* [ ] Did I actually fix the Omega variables, or just hide them?
* [ ] **Archive:** Save the Audit and Opinion files as part of the project metadata.
