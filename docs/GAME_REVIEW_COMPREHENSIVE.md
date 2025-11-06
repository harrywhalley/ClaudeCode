# Methodology Match: Comprehensive Game Review

**Date**: 2025-11-06
**Reviewer**: Full System Analysis
**Focus Areas**: Scoring Clarity, Educational Content, Game Balance, Card Coherence

---

## EXECUTIVE SUMMARY

This review identifies **6 critical issues** that must be addressed before the game is playable:

1. ⚠️ **CRITICAL**: Scoring rules are not visible on cards - players cannot calculate scores without constantly referencing rulebook
2. ⚠️ **CRITICAL**: Method cards lack educational descriptions - players don't know what methods are
3. ⚠️ **CRITICAL**: Only 3 Ontology cards for 3-player game - no flexibility for 2 or 4 players
4. ⚠️ **HIGH**: Ontology "Gameplay Effects" mentioned on cards but not in rules
5. ⚠️ **MEDIUM**: Synergy mismatches between Epistemology and Method cards
6. ⚠️ **MEDIUM**: "Object-of-Study Affinity" scoring is completely subjective

---

## ISSUE 1: SCORING NOT CLEAR ON CARDS ⚠️ CRITICAL

### Problem
Players cannot determine scores from looking at cards alone. The game requires constant rulebook reference.

### Current State: Method Cards

Method cards display 4 numerical stats but provide NO indication of what they mean:
- **Ethical Risk**: Rules say -1 point per Method with 7+, but card doesn't show this
- **Reproducibility**: Only matters for final "Objectivity Award", not shown on card
- **Sensibility**: Only matters for final "Insight Award", not shown on card
- **Novelty**: Used for "Cutting-Edge Bonus" if average ≥7, not explained on card

**Example**: A player looking at "Autoethnography" sees:
```
Ethical Risk: 7
Reproducibility: 2
Sensibility: 9
Novelty: 8
```

But has NO IDEA this means:
- -1 point (Ethical Risk ≥7)
- Contributes to potential +5 Insight Award (high Sensibility)
- Contributes to potential +3 Cutting-Edge Bonus (Novelty ≥7)

### Current State: Theory Cards

Theory cards say: *"Points are only awarded if this card's alignment matches the Epistemology in the same stack."*

But they DON'T clearly show:
- +7 points for 1 alignment
- +5 points for 2 alignments
- +3 points for 3 alignments

The "+7 (1 Alignment)" notation exists but is buried in the "Points Bonus" column as CSV data, not clear card text.

### Current State: Ontology Cards

Ontology cards have "Gameplay Effect" text that is **NOT IN THE RULES AT ALL**:

- **Realism**: "+2 points when using causal or quantitative methods"
- **Relativism**: "May hold contradictory findings and blocks generalisation bonuses from Realist players"
- **Constructivism**: "Draw one extra Method after completing a qualitative stack"

The rulebook (docs/rules_v1.md:2-97) **NEVER mentions these effects**. Are they active? Deprecated? Unknown.

### Current State: Epistemology Cards

Epistemology cards show:
- Compatible Ontologies (used for Paradigm Chain scoring)
- Incompatible cards (blocks Coherent Paradigm)
- Synergy list (methods that trigger +10 Coherent Paradigm)

But they DON'T explain:
- That compatible Ontology + synergy method = +10 points
- That incompatible Ontology = -5 points
- That neither = +3 points

### Recommended Solutions

#### Option A: Add Scoring Icons/Text to Cards
Add clear scoring indicators directly on cards:

**Method Card Template**:
```
METHOD NAME
[Description of method - see Issue 2]

Synergies: [List epistemologies]

SCORING IMPACTS:
├─ Ethical Risk: X  [if 7+: -1 point]
├─ Reproducibility: X  [→ Objectivity Award]
├─ Sensibility: X  [→ Insight Award]
└─ Novelty: X  [if avg 7+: +3 Cutting-Edge]

[If Reproducibility or Sensibility ≤2: Discard 1 extra card to play]
```

**Theory Card Template**:
```
THEORY NAME
[Brief description]

Aligns with: [Epistemology list]

POINTS:
• If aligned: +7/+5/+3 [based on # alignments]
• If not aligned: 0 points
```

**Epistemology Card Template**:
```
EPISTEMOLOGY NAME

Compatible Ontologies: [List]
Incompatible Ontologies: [List]

Synergy Methods: [List]

PARADIGM CHAIN SCORING:
• Compatible Ontology + Synergy Method: +10
• Incompatible Ontology: -5
• Other: +3
```

#### Option B: Create Reference Cards
Create 2-3 player reference cards summarizing all scoring rules.

**Recommendation**: Do BOTH Option A and Option B. Cards should be self-explanatory, but reference cards help during learning.

---

## ISSUE 2: METHOD CARDS LACK DESCRIPTIONS ⚠️ CRITICAL

### Problem
Method cards have NO educational content. They only show:
- Title
- Alignment/Synergy (vague references)
- 4 numerical stats

Players looking at "Phenomenology" or "Corpus Linguistics" have no idea what these methods are.

### Educational Value Lost
This game is designed for PhD researchers (rules_v1.md:5) as an **educational tool**. Without descriptions, it's just numbers and names.

### Current vs. Needed

| Current | Needed |
|---------|--------|
| Method: Phenomenology | Method: Phenomenology |
| Alignment: Embodied | **Description**: A qualitative method focusing on lived experience and consciousness. Researchers conduct in-depth interviews to understand how people experience phenomena from their perspective. |
| Stats: 6, 3, 9, 5 | Alignment: Embodied, Interpretivism |
| | Ethical Risk: 6, Reproducibility: 3, Sensibility: 9, Novelty: 5 |

### Recommendations

**SHORT-TERM**: Add 1-2 sentence descriptions to all Method cards (and ideally Theory cards too).

**PROPOSED METHOD DESCRIPTIONS** (see Section 8 below for full list of all 47 methods)

---

## ISSUE 3: ONLY 3 ONTOLOGY CARDS ⚠️ CRITICAL

### Problem
The game has exactly 3 Ontology cards:
- Realism
- Relativism
- Constructivism

According to rules_v1.md:24: *"Deal one face-down to each player. Place any unused Ontology cards back in the box."*

This means:
- ✅ 3-player game: Each player gets 1 Ontology (0 left over)
- ❌ 2-player game: Each player gets 1 Ontology (1 left over) - PLAYABLE but reduced variety
- ❌ 4-player game: **IMPOSSIBLE** - not enough Ontology cards

### Impact
- Game is locked to 3 players
- No replay variability (in 3p game, all Ontologies are always in play)
- Second Research Stack uses Epistemology, not Ontology (rules_v1.md:42), so Ontology choice is critical

### Are 3 Ontologies Philosophically Sufficient?

**Analysis of Current Ontologies**:

| Ontology | Philosophical Tradition | Coverage |
|----------|------------------------|----------|
| **Realism** | Objectivism, Scientific Realism | Covers: positivist, empirical, quantitative research |
| **Relativism** | Cultural Relativism, Social Constructionism | Covers: interpretive, critical, historical research |
| **Constructivism** | Social Constructionism | Covers: qualitative, participatory, embodied research |

**Overlap Problem**: Relativism and Constructivism are very similar. Both support:
- Relativism compatible with: Relativism, Constructivism epistemologies
- Constructivism compatible with: Relativism, Constructivism epistemologies

In practice, these two Ontologies play almost identically.

**Missing Ontologies**:
- **Critical Realism**: Combines realist ontology with interpretive epistemology (important in social sciences)
- **Phenomenological Ontology**: Focuses on consciousness and lived experience
- **Materialist Ontology**: Focuses on material conditions and physical reality
- **Pragmatist Ontology**: Truth is what works practically
- **Relational Ontology**: Reality exists in relationships (Indigenous, feminist thought)

### Recommendations

#### Option A: Add 2 More Ontology Cards → 5 Total
Add:
- **Critical Realism**: Compatible with all Epistemologies. Effect: +2 points for combining quantitative and qualitative methods in same stack.
- **Relational Ontology**: Compatible with Constructivism, Relativism, Feminist, Critical. Effect: +3 points if stack includes Participatory Methods.

This allows:
- 2-3 player games: Each player has choice/variety
- 4-5 player games: Possible
- Replay value: Different Ontology combinations each game

#### Option B: Allow Players to Choose Ontology (Draft)
Instead of random deal, players draft Ontologies:
- Lay out all 3 (or 5) Ontology cards face-up
- Players take turns selecting
- Creates strategic choice

#### Option C: Make Ontology Multi-Use
Allow multiple copies of each Ontology (2 of each = 6 total):
- Ensures 2-4 player games work
- Players might have same Ontology (less variety but functional)

**Recommendation**: **Option A** (add 2 ontologies to 5 total) + **Option B** (draft them). This maximizes strategic depth and educational value.

---

## ISSUE 4: ONTOLOGY "GAMEPLAY EFFECTS" NOT IN RULES ⚠️ HIGH

### Problem
Ontology cards have text describing gameplay effects, but these effects are **not mentioned anywhere in the rulebook**.

### Current Ontology Card Text:

#### Realism (cards_master.csv:2)
*"Gameplay Effect: +2 points when using causal or quantitative methods."*

**Issues**:
- Not in scoring rules (rules_v1.md:61-96)
- What counts as "causal or quantitative methods"?
- Is this +2 per method, or +2 total for the stack?

#### Relativism (cards_master.csv:3)
*"Gameplay Effect: May hold contradictory findings and blocks generalisation bonuses from Realist players."*

**Issues**:
- "Generalisation bonuses" are never defined anywhere in the game
- "Blocks...from Realist players" - this is an attack/interaction mechanic not in rules
- Extremely unclear

#### Constructivism (cards_master.csv:4)
*"Gameplay Effect: Draw one extra Method after completing a qualitative stack."*

**Issues**:
- What is a "qualitative stack"?
- Is this +1 card draw per stack, or once per game?
- Might break the "7 cards in hand" rule (rules_v1.md:50)

### Recommendations

#### Option A: Remove These Effects Entirely
If they're not in the rules, they may be deprecated design ideas. Remove the text from cards to avoid confusion.

#### Option B: Add These Effects to Rules
Clarify and integrate them properly:

**Realism** (Revised):
- *"+2 points if your stack includes a Method with Reproducibility 8 or higher."*

**Relativism** (Revised):
- *"Your stack scores +2 points if it includes Methods from conflicting paradigms (e.g., one Positivist and one Critical method)."*

**Constructivism** (Revised):
- *"When you complete a stack containing at least 2 Methods with Sensibility 7+, draw 1 card (then discard to 7)."*

**Recommendation**: **Option B** - properly define and integrate these effects. They add strategic variety to Ontology choices.

---

## ISSUE 5: SYNERGY MISMATCHES BETWEEN EPISTEMOLOGY & METHOD CARDS ⚠️ MEDIUM

### Problem
Epistemology cards list method synergies that don't exactly match the Method card names or alignments.

### Specific Mismatches

#### Positivism (cards_master.csv:5)
**Epistemology card says synergizes with**:
- "Surveys, Experiments, Statistical Modelling, Content Analysis, Social Media Mining"

**Actual Method cards with Positivism alignment**:
- ✅ Content Analysis (match)
- ✅ Social Media Mining (match)
- ❌ "Surveys" → Method card is called **"Survey (Quantitative)"**
- ❌ "Experiments" → Method card is called **"Experimental Design"**
- ❌ "Statistical Modelling" → Method card is called **"Statistical Analysis"**
- ➕ **Archival Research** has Positivism alignment but isn't listed
- ➕ **Corpus Linguistics** has Positivism alignment but isn't listed

#### Feminist Epistemology (cards_master.csv:8)
**Epistemology card says synergizes with**:
- "Autoethnography, Narrative Inquiry, Participatory Methods, Zine-Making, Voice-Centred Method"

**Issues**:
- ❌ "Zine-Making" - NO METHOD CARD EXISTS
- ❌ "Voice-Centred Method" - NO METHOD CARD EXISTS
- Other listed methods exist and match ✅

#### Embodied Epistemology (cards_master.csv:10)
**Epistemology card says synergizes with**:
- "Performance Ethnography, Walking Interview, Embodied Mapping, Soundwalk Method, Affect Theory"

**Issues**:
- ❌ "Affect Theory" is a **THEORY card**, not a Method
- All other methods exist and match ✅

### Impact
- Players will be confused trying to match names
- Coherent Paradigm (+10 points) requires "at least one Method card has a listed synergy with that Epistemology" (rules_v1.md:69)
- If names don't match, players won't know if they qualify

### Recommendations

#### Fix 1: Standardize Names
Update Epistemology synergy lists to match exact Method card names:
- "Surveys" → "Survey (Quantitative)"
- "Experiments" → "Experimental Design"
- "Statistical Modelling" → "Statistical Analysis"

#### Fix 2: Add Missing Method Cards or Remove from Lists
Either:
- Add "Zine-Making" and "Voice-Centred Method" as new Method cards, OR
- Remove them from Feminist Epistemology synergy list

#### Fix 3: Distinguish Methods from Theories
Remove "Affect Theory" from Embodied Epistemology synergy list (it's a Theory, not a Method).

#### Fix 4: Add Missing Synergies
Add Archival Research and Corpus Linguistics to Positivism synergy list.

**Recommendation**: Do all 4 fixes. Create a complete synergy matrix spreadsheet to verify all connections.

---

## ISSUE 6: OBJECT-OF-STUDY AFFINITY IS SUBJECTIVE ⚠️ MEDIUM

### Problem
Rules_v1.md:79 states:
*"Object-of-Study Affinity: Add +2 points if your stack is thematically aligned with the shared Object-of-Study card."*

**No criteria for "thematically aligned" are provided.**

### Example Ambiguity

**Object-of-Study**: "Digital Media & Online Communities"

**Player's Stack**:
- Interpretivism
- Hermeneutics
- Ethnography
- Thematic Analysis

**Question**: Does this qualify for +2 points?
- Player argues: "Ethnography can study online communities, so yes!"
- Opponent argues: "You're not using digital methods like Netnography or Social Media Mining, so no!"

With no clear criteria, this becomes a source of arguments and inconsistency.

### Current Object-of-Study Cards

All 20 Object-of-Study cards have brief descriptions (e.g., "Research into how people interact on the internet") but NO keywords or tags for matching.

### Recommendations

#### Option A: Add Keywords to All Cards
Add 2-3 keywords to each Object-of-Study card and matching keywords to Method/Theory cards.

**Example**:
```
Object-of-Study: Digital Media & Online Communities
Keywords: #Digital, #Contemporary, #Social

Method: Netnography
Keywords: #Digital, #Social, #Ethnographic
→ 2 keyword matches = +2 points!

Method: Historical Method
Keywords: #Archival, #Temporal, #Documentary
→ 0 keyword matches = 0 points
```

#### Option B: Make It Automatic
Remove the subjective judgment - ALL stacks get +2 points for Object-of-Study (it's always in play, so it's always relevant).

#### Option C: Remove Object-of-Study Scoring Entirely
Keep Object-of-Study cards as thematic flavor but don't award points. Simplifies scoring.

**Recommendation**: **Option A** (keywords). This makes scoring objective while rewarding thoughtful method-object alignment. Educational value: teaches appropriate method-subject matching.

---

## ISSUE 7: CARD DATA QUALITY ISSUES ⚠️ LOW

### Minor Issues Found

#### Inconsistent Alignment Notation
Method cards use various formats for alignments:
- "Positivism, Foucauldian" (mixing epistemology and theory)
- "Critical, Pragmatist" (abbreviations without "Epistemology")
- "Embodied/Aesthetic" (using / instead of ,)
- "Deleuzian/Aesthetic" (references philosopher not in game)

**Recommendation**: Standardize all alignments to use full Epistemology names consistently.

#### Missing Alignments
Some Method cards have vague or incomplete alignments:
- "Material Culture" (what epistemology is this?)
- "Historical Method" (vague)
- "New Materialism" (this is a theory, not an epistemology)

**Recommendation**: Every Method must list at least one clear Epistemology alignment.

#### Event Card Balance (already noted in IMPROVEMENT_PLAN.md)
Some Event cards are extremely powerful, others are weak. Needs playtesting.

---

## SECTION 8: PROPOSED METHOD CARD DESCRIPTIONS

Below are concise 1-2 sentence educational descriptions for all 47 Method cards. These should be added to the cards.

### Quantitative & Positivist Methods

**Experimental Design**
A controlled research method where the researcher manipulates variables to test cause-and-effect relationships. Commonly uses randomization, control groups, and statistical analysis to ensure validity.

**Survey (Quantitative)**
Structured questionnaires administered to large samples to collect numerical data. Results are analyzed statistically to identify patterns and test hypotheses.

**Statistical Analysis**
Mathematical techniques for analyzing numerical data, identifying patterns, and testing hypotheses. Includes regression, correlation, and significance testing.

**Content Analysis**
Systematic coding and quantification of text, images, or media to identify patterns. Can be quantitative (counting) or qualitative (thematic).

**Social Media Mining**
Computational analysis of large-scale social media data to identify trends, networks, and behaviors. Uses algorithms and natural language processing.

**Corpus Linguistics**
Computer-aided analysis of large text collections (corpora) to study language patterns, frequencies, and usage. Combines computational and linguistic methods.

**Longitudinal Study**
Research that follows the same subjects over an extended period to observe changes over time. Can be quantitative or qualitative.

### Qualitative & Interpretive Methods

**Interview (Qualitative)**
In-depth, semi-structured conversations with participants to explore their experiences, perspectives, and meanings. Data is analyzed thematically or narratively.

**Ethnography**
Immersive fieldwork where the researcher participates in and observes a community or culture over time. Produces rich, contextual understanding of social practices.

**Case Study**
In-depth investigation of a single instance, event, or bounded system to understand complexity and context. Uses multiple data sources.

**Thematic Analysis**
A flexible qualitative method for identifying, analyzing, and reporting patterns (themes) across a dataset. Widely used across disciplines.

**Grounded Theory**
An iterative qualitative method where theory emerges from systematic data collection and analysis. Researchers develop concepts grounded in empirical data.

**Narrative Inquiry**
Analysis of stories and narratives to understand how people make sense of their experiences. Focuses on plot, characters, and temporal structure.

**Oral History**
Recording and analyzing first-person accounts of historical events or lived experiences. Preserves memory and subjective historical knowledge.

**Biographical Method**
In-depth study of individual lives through interviews, documents, and life stories. Explores how personal trajectories intersect with social contexts.

**Focus Groups**
Facilitated group discussions with 6-10 participants to explore collective views, experiences, and interactions. Generates data through group dynamics.

### Critical & Participatory Methods

**Discourse Analysis**
Analysis of language use in texts, speech, or media to reveal power relations, ideologies, and social constructions. Examines how meaning is produced.

**Critical Discourse Analysis**
Examines how language perpetuates power inequalities and social injustice. Combines linguistic analysis with critical social theory.

**Action Research**
Collaborative research where participants and researchers work together to solve real-world problems and create change. Cycles of action and reflection.

**Participatory Methods**
Research conducted with (not on) participants, who help design, conduct, and interpret the study. Emphasizes empowerment and co-production of knowledge.

### Embodied & Aesthetic Methods

**Autoethnography**
A reflexive research method where the researcher uses their own lived experience as primary data to explore cultural phenomena. Combines autobiography and ethnography.

**Performance Ethnography**
Research method using embodied performance to represent and analyze cultural experiences. The body becomes a site of knowledge production.

**Phenomenology**
Philosophical method exploring how people experience and make sense of phenomena through consciousness. Uses in-depth interviews and first-person accounts.

**Embodied Mapping**
Creating maps through bodily movement and sensory experience. Combines cartography with phenomenological attention to how space is lived.

**Walking Interview**
Interviews conducted while walking through a place relevant to the research. Movement and place elicit memories and situated knowledge.

**Soundwalk Method**
Research method involving attentive listening while moving through an environment. Produces knowledge about sonic experiences and acoustic ecology.

**Sensory Ethnography**
Ethnographic approach emphasizing non-visual senses (sound, smell, touch, taste) in understanding culture. Challenges ocularcentrism in research.

**Practice-Based Research**
Research where creative practice (art, design, performance) is itself a method of inquiry. The artwork generates knowledge.

**Drawing as Inquiry**
Using drawing as a research method to explore, represent, and generate knowledge. The act of drawing produces insights beyond words.

**Creative Writing as Inquiry**
Using creative writing (fiction, poetry, narrative) as a method to explore and represent research findings. Writing as thinking and discovery.

### Digital & Contemporary Methods

**Netnography**
Ethnographic research adapted for online communities and digital cultures. Observes and participates in internet-based social interactions.

**Digital Humanities Methods**
Computational approaches to humanities questions, including text mining, network analysis, and digital archives. Combines technology with interpretation.

**VR Ethnography**
Ethnographic research conducted in virtual reality environments. Studies how people interact, socialize, and create meaning in VR spaces.

### Arts & Cultural Analysis Methods

**Textual Analysis**
Close reading and interpretation of texts (literary, cultural, media) to understand meaning, structure, and significance. Central to literary studies.

**Film Analysis**
Critical examination of films considering cinematography, narrative, editing, and cultural context. Combines formal and contextual analysis.

**Visual Analysis**
Systematic study of visual objects (art, photos, design) examining composition, symbolism, and cultural meaning. Combines formal and semiotic approaches.

**Semiotic Analysis**
Study of signs and symbols to understand how meaning is created and communicated. Analyzes texts, images, and cultural phenomena as sign systems.

**Material Culture Analysis**
Study of physical objects to understand culture, values, and social practices. Objects are read as texts that reveal cultural meaning.

**Artefact Analysis**
Close examination of physical objects considering materiality, design, use, and cultural significance. Objects as evidence and meaning-makers.

### Archival & Historical Methods

**Archival Research**
Research using primary source documents from archives, libraries, or collections. Requires critical evaluation of historical sources.

**Historical Method**
Systematic investigation of the past using primary and secondary sources. Emphasizes chronology, causation, and context.

**Documentary Analysis**
Critical examination of documents (texts, images, recordings) as evidence. Considers authorship, purpose, and historical context.

### Mixed & Speculative Methods

**Mixed-Methods Research**
Combines quantitative and qualitative approaches in a single study. Integration occurs at design, data collection, or interpretation stages.

**Speculative Design**
Design method that uses fictional scenarios and prototypes to explore possible futures and provoke critical thinking about technology and society.

**Cultural Probes**
Design research method giving participants kits (cameras, diaries, maps) to document their lives. Generates evocative, subjective data about lived experience.

**Exhibition-as-Research**
Curating and staging exhibitions as a method of knowledge production. The exhibition itself is the research output and argument.

**Memory-Work Method**
Feminist collective inquiry method where groups analyze their own memories to understand how social forces shape personal experience. Developed by Frigga Haug.

---

## SECTION 9: SCORING EXAMPLE WALKTHROUGH

To demonstrate the scoring clarity problem, here's a complete example:

### Example Stack

**Player's Completed Stack**:
- Ontology: Constructivism (secret)
- Epistemology: Interpretivism
- Theory: Hermeneutics (+7 for 1 alignment with Interpretivism)
- Theory: Phenomenology (+5 for 2 alignments)
- Method: Interview (Qualitative) - Stats: 6, 4, 8, 4
- Method: Ethnography - Stats: 7, 3, 8, 5
- Method: Thematic Analysis - Stats: 4, 6, 6, 4

**Object-of-Study** (shared): "Memory & Oral Histories"

### Scoring Calculation

**1. Paradigm Chain Bonus**:
- Constructivism compatible with Interpretivism? YES (cards_master.csv:6)
- Does at least one Method have Interpretivism synergy?
  - Interview: YES (cards_master.csv:56)
  - Ethnography: YES (cards_master.csv:49)
  - Thematic Analysis: YES (cards_master.csv:74)
- **Result: Coherent Paradigm = +10 points**

**2. Theory Bonuses**:
- Hermeneutics aligns with Interpretivism: +7 points
- Phenomenology aligns with Interpretivism: +5 points
- **Result: +12 points**

**3. Object-of-Study Affinity**:
- Is this stack thematically aligned with "Memory & Oral Histories"?
- Probably yes (qualitative methods studying memory)
- **Result: +2 points** (but this is subjective - Issue #6!)

**4. Ethical Penalty**:
- Interview: Ethical Risk 6 (not ≥7, no penalty)
- Ethnography: Ethical Risk 7 (-1 point)
- Thematic Analysis: Ethical Risk 4 (no penalty)
- **Result: -1 point**

**5. Cutting-Edge Bonus**:
- Average Novelty: (4 + 5 + 4) / 3 = 4.33
- Is 4.33 ≥ 7? NO
- **Result: 0 points**

**Total Stack Score: 10 + 12 + 2 - 1 + 0 = 23 points**

**Plus Later**:
- Objectivity Award: Reproducibility total = 4 + 3 + 6 = 13 (might win +5)
- Insight Award: Sensibility total = 8 + 8 + 6 = 22 (might win +5)

### Problem
The player had to:
1. Reference the rulebook 5+ times
2. Look up Ontology-Epistemology compatibility
3. Look up Method synergies
4. Calculate averages
5. Guess at "thematic alignment"

**None of this is clear from the cards themselves.**

---

## SECTION 10: RECOMMENDATIONS SUMMARY

### Must-Fix Before Playable (Critical Priority)

1. **Add scoring text/icons to all cards** - Players must be able to score without rulebook
2. **Add educational descriptions to all Method cards** - Players should learn what methods are
3. **Add 2 more Ontology cards (to 5 total)** - Enable 2-4 player games and add strategic depth
4. **Decide on Ontology Gameplay Effects** - Either remove them or properly integrate into rules
5. **Fix synergy mismatches** - Method names must match Epistemology synergy lists exactly
6. **Create objective Object-of-Study scoring** - Add keywords or remove scoring entirely

### Should-Fix for Better Experience (High Priority)

7. **Create player reference cards** - Quick-reference for scoring rules
8. **Standardize alignment notation** - All Methods use full Epistemology names
9. **Playtest Event cards** - Some are too powerful, needs balance
10. **Add Theory card descriptions** - Educational value for theoretical frameworks

### Nice-to-Have (Medium Priority)

11. **Create synergy matrix spreadsheet** - Visual chart of all Method-Epistemology connections
12. **Add Ontology descriptions** - Explain what each ontological position means
13. **Consider reducing Ethical Penalty** - Currently -1 per high-risk method is harsh
14. **Add more specific scoring examples in rulebook** - Help players learn the game

---

## SECTION 11: NEXT STEPS

### Phase 1: Data Fixes (1-2 days)
- [ ] Fix all Method-Epistemology synergy name mismatches
- [ ] Standardize alignment notation across all Method cards
- [ ] Add descriptions to all 47 Method cards
- [ ] Add descriptions to all 22 Theory cards
- [ ] Decide on Ontology Gameplay Effects (keep or remove)

### Phase 2: Ontology Expansion (2-3 days)
- [ ] Design 2 new Ontology cards (Critical Realism, Relational Ontology suggested)
- [ ] Add descriptions to all Ontology cards
- [ ] Update rules for Ontology draft mechanic
- [ ] Update rules to include Ontology Gameplay Effects if kept

### Phase 3: Scoring Clarity (3-4 days)
- [ ] Design card layouts with scoring text integrated
- [ ] Create player reference cards (2-3 pages)
- [ ] Add keywords to all Object-of-Study cards
- [ ] Add keywords to Method and Theory cards for Object matching
- [ ] Update rules with objective Object-of-Study scoring

### Phase 4: Playtesting (ongoing)
- [ ] Playtest with complete card descriptions
- [ ] Playtest with 2, 3, and 4 players
- [ ] Test if scoring is clear from cards alone
- [ ] Balance Event cards based on play experience

---

## CONCLUSION

**Methodology Match has a brilliant core design** - the Paradigm Chain scoring system and methodological synergies are clever and educational. However, **the game is not currently playable** due to critical issues with scoring clarity and educational content.

The good news: All issues are fixable with content additions rather than fundamental redesign.

**Estimated effort**: 5-10 days of focused work to address all critical issues.

**Priority**: Fix scoring clarity and Method descriptions first. These are blockers to any meaningful playtesting.

---

*End of Review*
