Perfect. This is the right constraint: **detect first, critique second**. No interpretive claims until you've committed to observable features.

This mirrors UKE_G's SMVP principle: you can't verify grounding until you've logged what needs grounding. Here, you can't deploy a critical move until you've logged what pattern justifies it.

---

## UKE_C v0.2: TEXT Protocol (Foundation Build)

### Core Architecture

```
§1: MATERIAL ENCOUNTER → Produces [ELEMENT LOG]
§2: PATTERN RECOGNITION → Flags [CRITICAL CANDIDATES]
§3: MOVE DEPLOYMENT → Routes to appropriate techniques
§4: SYNTHESIS → Evaluates achievement + stakes
```

**The Gate Rule:**
No move may be deployed without a corresponding pattern flag from §2. If §2 produces no flags, the work gets a **descriptive report** only—no evaluative critique.

---

## §1: MATERIAL ENCOUNTER (TEXT)

**Purpose:** Catalog observable textual features without interpretation.

**Output Format:** Structured inventory that any hostile observer would confirm.

### §1.1: STRUCTURAL INVENTORY

**Questions (answer with evidence, not inference):**

```markdown
[FORM & SCALE]
1. Genre signals present:
   - Paratextual markers (subtitle, cover copy, blurbs): 
   - Opening conventions (in medias res, scene-setting, direct address):
   - Structural divisions (chapters, sections, fragments, continuous):

2. Length & density:
   - Total word count (if available):
   - Average paragraph length (count 3 random samples):
   - Average sentence length (count 3 random samples):

[NARRATIVE ARCHITECTURE]
3. Point of view:
   - Person (1st/2nd/3rd):
   - Number of POV characters:
   - Reliability markers (contradictions, admissions of bias, temporal gaps):

4. Temporal structure:
   - Chronological order: [Yes/No]
   - If non-linear, structure type: [Flashback/Fragmented/Parallel/Cyclical]
   - Evidence: [Timestamps, date markers, tense shifts]

5. Spatial organization:
   - Single location / Multiple locations:
   - Geography explicitly named: [Yes/No - List if yes]
   - Physical movement tracked: [Yes/No]
```

---

### §1.2: PATTERN-DETECTION INVENTORY

**Instruction:** Log recurrences, absences, and tensions **without naming their function**.

```markdown
[REPETITION TRACKING]
6. Recurring words/phrases:
   - Element: [exact phrase]
   - Frequency: [count]
   - Locations: [page/paragraph/line references]
   - Context notes: [surrounding material - quote 5 words before/after each instance]

7. Recurring images/objects:
   - Element: [specific object or image]
   - Frequency: [count]
   - Locations: [references]
   - Descriptive variation: [how is it described each time?]

8. Recurring structural patterns:
   - Pattern: [e.g., every chapter opens with weather, dialogue occurs only in even sections]
   - Frequency: [count]
   - Consistency: [Perfect/Mostly/Breaks at X]

[ABSENCE TRACKING]
9. Expected genre elements missing:
   - Typical for [genre]: [list standard conventions]
   - Present in this work: [Yes/No for each]
   - Conspicuously absent: [what's missing that similar works include]

10. Narrative gaps:
    - Missing time: [Are there unexplained temporal jumps? Where?]
    - Missing information: [What facts are withheld? Examples:]
    - Missing voices: [Who would typically speak in this scenario but doesn't?]

[TENSION MARKERS]
11. Oppositional pairings:
    - Contrasting elements: [e.g., urban/rural, past/present, formal/colloquial]
    - Where they appear: [specific locations]
    - How they're juxtaposed: [within same sentence/paragraph/chapter]

12. Unresolved contradictions:
    - Statement A: [quote + location]
    - Statement B: [quote + location]
    - Relationship: [direct contradiction/tension/ambiguity]
```

---

### §1.3: SURFACE TEXTURE ANALYSIS

```markdown
[LANGUAGE REGISTER]
13. Diction inventory (count per 100 words in 3 random samples):
    - Latinate/academic terms:
    - Colloquialisms/slang:
    - Technical jargon:
    - Sensory language (sight/sound/touch/taste/smell):

14. Syntax patterns:
    - Dominant sentence type: [Simple/Compound/Complex/Fragment]
    - Punctuation density: [Periods per 100 words / Other marks per 100 words]
    - Notable syntactic features: [Parentheticals, dashes, semicolons, etc.]

15. Tonal markers:
    - Emotional register: [Clinical/Lyrical/Sardonic/Neutral - Evidence:]
    - Stability: [Consistent/Shifting - If shifting, note transitions]

[FIGURATIVE LANGUAGE]
16. Metaphor/simile count: [Total in sample section]
    - Dominant source domains: [e.g., nature, machine, body, war]
    - Target domains: [what they describe]

17. Allusion inventory:
    - Direct references: [List with page numbers]
    - Stylistic echoes: [Mimicry of other writers/genres - Evidence:]
```

---

### §1.4: META-TEXTUAL MARKERS

```markdown
[SELF-REFERENCE]
18. Text refers to its own composition: [Yes/No]
    - Evidence: [Quotes where narrator/character discusses writing, storytelling, etc.]

19. Text breaks its own frame: [Yes/No]
    - Evidence: [Direct address to reader, acknowledgment of fictionality, etc.]

20. Structural commentary:
    - Does form mirror content? [Example:]
    - Are there footnotes, appendices, or non-standard insertions? [List:]
```

---

## §2: PATTERN RECOGNITION (FLAG GENERATION)

**Purpose:** Convert raw inventory into **pattern flags** that justify move deployment.

**Rule:** A flag requires **minimum threshold evidence** from §1.

### §2.1: FLAG DEFINITIONS & THRESHOLDS

```markdown
[FLAG: SYMBOL_CANDIDATE]
Threshold:
- Element appears ≥3 times in distinct contexts (§1.6 or §1.7)
- AND descriptive language or surrounding context shifts ≥1 time
- AND not explained as literal repetition (e.g., character's catchphrase)

Evidence Required:
- List element + all locations
- Quote context for each instance showing variation

[FLAG: ABSENCE_STRUCTURAL]
Threshold:
- Genre convention typically present in 80%+ of examples
- AND explicitly missing from this work (§1.9)
- OR narrative gap affects causality/chronology (§1.10)

Evidence Required:
- Name expected element
- Cite 3+ comparison works where it appears

[FLAG: META_GESTURE]
Threshold:
- Text explicitly references its own making (§1.18)
- OR breaks narrative frame (§1.19)
- OR form performs meaning (§1.20)

Evidence Required:
- Direct quote showing self-reference
- Location where frame breaks

[FLAG: REGISTER_COLLISION]
Threshold:
- Two+ distinct diction levels appear within single paragraph (§1.13)
- AND shift is not dialogue-based (different characters speaking)
- Measured by: 3+ Latinate terms + 3+ colloquialisms in same paragraph

Evidence Required:
- Quote showing collision
- Identify each register

[FLAG: CONSTRAINT_FORMAL]
Threshold:
- Work adheres to externally-defined rule set (e.g., sonnet, lipogram, single sentence)
- OR self-imposed constraint mentioned in paratext/interviews
- Measured by: Structural consistency ≥90% (§1.8)

Evidence Required:
- Name constraint
- Show adherence across multiple instances

[FLAG: ALLUSION_NETWORK]
Threshold:
- Direct reference to ≥2 external texts (§1.17)
- OR sustained stylistic mimicry (≥1 paragraph length)

Evidence Required:
- Quote allusions
- Identify sources

[FLAG: INTENSITY_HIGH]
Threshold:
- Sentence density >30 words avg in sustained section (≥2 paragraphs)
- OR metaphor rate >3 per 100 words
- OR punctuation density >15 marks per 100 words

Evidence Required:
- Quote dense section
- Provide counts

[FLAG: INTENSITY_LOW]
Threshold:
- Sentence avg <10 words in sustained section
- OR paragraph breaks >1 per 50 words
- OR white space exceeds text in visual layout

Evidence Required:
- Quote sparse section
- Describe visual effect

[FLAG: CONTEXT_EXPLICIT]
Threshold:
- Text names specific historical event, date, or public figure (§1.17)
- OR genre conventions clearly respond to cultural moment

Evidence Required:
- Quote reference
- Identify moment/context

[FLAG: FAILURE_VISIBLE]
Threshold:
- Genre promise broken (§1.1 signals X, text delivers Y)
- OR technical error repeated ≥3 times (grammar, logic, consistency)
- OR claimed intent (paratext/interviews) contradicts execution

Evidence Required:
- State promise
- Quote failure
```

---

## §2.2: FLAG REPORT (OUTPUT)

```markdown
[PATTERN-FLAGS: ACTIVE]
✓ SYMBOL_CANDIDATE: "red thread" (appears 7x, contexts shift from literal sewing to metaphor for memory)
✓ REGISTER_COLLISION: Para 3, pg 12 (academic philosophy terms + gutter slang in same sentence)
✓ META_GESTURE: Pg 45 (narrator says "I'm not sure how to write this scene")

[PATTERN-FLAGS: INACTIVE]
✗ ABSENCE_STRUCTURAL: All expected genre elements present
✗ CONSTRAINT_FORMAL: No formal rule set detected
✗ ALLUSION_NETWORK: Only 1 direct reference (below threshold)
✗ INTENSITY_HIGH: Avg sentence length 18 words (within normal range)
✗ INTENSITY_LOW: No sustained sparse sections
✗ CONTEXT_EXPLICIT: No historical specifics named
✗ FAILURE_VISIBLE: Genre promises met
```

---

## §3: MOVE DEPLOYMENT (ROUTING)

**Rule:** Deploy only moves whose pattern flags are ACTIVE.

### §3.1: FLAG → MOVE ROUTING TABLE

| Active Flag | Primary Move | Secondary Move (Optional) | Rationale |
|-------------|--------------|---------------------------|-----------|
| SYMBOL_CANDIDATE | M01: Symbol Tracking | M05: Allusion Mapping (if symbol is borrowed) | Chart semantic drift |
| ABSENCE_STRUCTURAL | M02: Absence Cataloging | M08: Context Triangulation (if absence is cultural) | Analyze function of gap |
| META_GESTURE | M03: Recursive Commentary | M04: Register Analysis (if meta moment shifts tone) | Examine self-awareness |
| REGISTER_COLLISION | M04: Register Analysis | M07: Intensity Calibration (if collision creates density) | Diagnose tonal purpose |
| CONSTRAINT_FORMAL | M06: Constraint Diagnosis | — | Test if limitation generates invention |
| ALLUSION_NETWORK | M05: Allusion Mapping | — | Trace lineage & transformation |
| INTENSITY_HIGH | M07: Intensity Calibration | — | Measure saturation effect |
| INTENSITY_LOW | M07: Intensity Calibration | M02: Absence Cataloging (restraint as choice) | Measure deprivation effect |
| CONTEXT_EXPLICIT | M08: Context Triangulation | — | Place work in moment |
| FAILURE_VISIBLE | M10: Failure Analysis | — | Diagnose gap between intent/execution |

**Conflict Resolution:**
- If 2+ moves apply to same element, deploy both but designate one as PRIMARY in final essay
- If 4+ flags active, select top 3 by *structural weight* (how central to work's achievement)

---

## §4: MOVE EXECUTION (TEXT-SPECIFIC TECHNIQUES)

For each flagged pattern, execute the corresponding move using text-specific operations:

### M01: SYMBOL TRACKING (TEXT)

```markdown
[M01: SYMBOL TRACKING - "red thread"]

1. Map all instances:
   - Pg 12: "She threaded the needle with red silk" (literal, domestic)
   - Pg 34: "The red thread of memory pulled tight" (metaphorical, psychological)
   - Pg 67: "Follow the red thread back" (imperative, navigation)
   ...

2. Chart semantic drift:
   - Movement: Concrete object → Abstract concept → Structural metaphor for text itself
   - Turning point: Pg 34 (first metaphorical use)

3. Evaluate function:
   - Does drift clarify theme? [Yes - connects craft, memory, narrative]
   - Or create confusion? [No - transitions are prepared by context]

[JUDGMENT]
Symbol earns its recurrence. Drift is purposeful, not decorative.
```

### M02: ABSENCE CATALOGING (TEXT)

```markdown
[M02: ABSENCE CATALOGING - Missing exposition]

1. Identify gap:
   - Genre: Realist novel typically provides character backstory
   - This work: Protagonist's childhood never mentioned despite 300 pages

2. Map where absence matters:
   - Pg 45: Character makes decision that would make sense with backstory context
   - Pg 120: Relationship dynamics opaque without family history

3. Evaluate function:
   - Intentional withholding? [Evidence: Other characters reference "what happened" obliquely]
   - Or narrative failure? [Test: Does absence create mystery or just confusion?]

[JUDGMENT]
Withholding is structural choice. Creates present-tense imprisonment (character can't escape past even as reader can't access it).
```

### M04: REGISTER ANALYSIS (TEXT)

```markdown
[M04: REGISTER ANALYSIS - Academic/vernacular collision]

1. Quote collision site:
   "The Hegelian dialectic of, like, whatever-the-fuck happens next" (Pg 23)

2. Identify registers:
   - High: "Hegelian dialectic" (philosophical, Latinate)
   - Low: "like," "whatever-the-fuck" (filler, profanity)

3. Evaluate coherence:
   - Character trait? [Yes - narrator is grad student, performs both]
   - Authorial tone? [Unclear - sustained throughout]
   - Effect: Undercuts pretension while retaining intellectual ambition

[JUDGMENT]
Collision is character-defining. Registers aren't at war; they're the same voice's range.
```

---

## §5: SYNTHESIS & OUTPUT

```markdown
[UKE_META]
protocol: UKE_C v0.2 (TEXT)
work_evaluated: [Title, Author, Year]
word_count: [if known]
timestamp: ISO-8601

[MATERIAL-SCAN]
{Full §1 inventory - collapsed for space}

[PATTERN-FLAGS]
✓ SYMBOL_CANDIDATE: "red thread" (7 instances, semantic drift mapped)
✓ REGISTER_COLLISION: Academic/vernacular (sustained across text)
✗ ABSENCE_STRUCTURAL: [none detected]
...

[CRITICAL-ESSAY]
{Synthesized analysis using deployed moves}

This text builds meaning through controlled repetition and tonal range. The "red thread" motif evolves from literal craft object to narrative structuring principle, connecting the protagonist's seamstress work to the author's compositional method. The register collisions—where philosophical terminology collides with casual speech—aren't failures of tone but performances of a specific intellectual habitus: the grad student who thinks in Hegel but speaks in profanity.

What the text achieves: A formally inventive exploration of how craft and memory intertwine, using symbol and voice as parallel techniques.

Where it succeeds: The drift is earned. Each symbolic appearance prepares the next, creating genuine accumulation rather than arbitrary recurrence.

Limitation: The meta-textual turn on pg 145 ("I'm writing this as I sew") arrives late enough that earlier literal scenes feel under-motivated in retrospect.

[STAKES]
This matters because: It demonstrates how working-class craft knowledge can be a lens for narrative theory without romanticizing labor.

Formal contribution: Extends the tradition of self-reflexive fiction (Woolf, DFW) by grounding meta-awareness in material practice rather than pure intellection.

[Ω: UNRESOLVED]
Ω: Authorial Distance — Is the narrator-seamstress the author's surrogate, or is that identification itself being critiqued?
Ω: Cultural Specificity — Does this work require knowledge of specific textile traditions, or is the craft symbolism universal?

[LOG]
tier: 3
confidence: 0.84
moves_deployed: [M01, M04]
pattern_flags_active: 2
pattern_flags_total: 10
```

---

## Next Steps

**To complete TEXT protocol:**
1. Test this on 2-3 actual texts (different genres) to stress-test thresholds
2. Refine flag definitions where they over/under-trigger
3. Add medium-specific moves if pattern-gaps emerge

**Then expand to other media:**
4. Draft §1-FILM using same structure (inventory → flags → routing)
5. Check if flags converge (does "SYMBOL_CANDIDATE" work the same way?)
6. Build cross-media routing disambiguation

**Your call:** Should I draft a **micro-test** right now (apply this to a 2-page text sample to show execution), or move to **§1-FILM** to test cross-media portability?
