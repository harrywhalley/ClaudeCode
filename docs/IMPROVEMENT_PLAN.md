# Methodology Match - Improvement & Expansion Plan

## Overview
This document outlines recommendations for improving and expanding the Methodology Match card game based on a comprehensive review of the current structure.

---

## 1. IMMEDIATE FIXES (Priority: High)

### 1.1 Card Count Issues
**Problem**: Rules state 47 Method cards, but CSV only contains 41.

**Action Items**:
- [ ] Add 6 new Method cards to reach the stated 47
- [ ] Suggested additions:
  - **Cultural Probes** (Design Research, Pragmatist, Embodied)
  - **Corpus Linguistics** (Digital Humanities, Positivism)
  - **Photo Elicitation** (Interpretivism, Visual Methods)
  - **Critical Discourse Analysis** (Critical Epistemology, Foucauldian)
  - **Memory-Work Method** (Feminist Epistemology)
  - **Sensory Ethnography** (Embodied, Aesthetic Epistemology)

### 1.2 Complete Missing Synergy Data
**Problem**: Some Method cards have vague or missing alignment information.

**Action Items**:
- [ ] Review all Method card alignments
- [ ] Ensure every Method lists at least 1-2 compatible epistemologies
- [ ] Create a synergy matrix spreadsheet for game balancing

### 1.3 Clarify Object-of-Study Rules
**Problem**: "Thematic alignment" is subjective (rules_v1.md:79).

**Action Items**:
- [ ] Add explicit tags/keywords to each Object-of-Study card
- [ ] Add matching tags to Method and Theory cards
- [ ] Create objective matching rules (e.g., "if any card in your stack shares a tag with the Object-of-Study")

---

## 2. CONTENT EXPANSIONS (Priority: Medium)

### 2.1 Expand Method Cards (+20 cards → 67 total)
**Rationale**: More variety = more replayability and strategic options.

**Suggested New Methods**:
- **From Social Sciences**: Focus Groups (Qualitative), Q-Methodology, Social Network Analysis
- **From Design**: Service Design, Co-Design Workshops, Speculative Futures
- **From Digital Humanities**: Topic Modeling, Network Analysis, Distant Reading
- **From Arts Practice**: Sound Art Research, Installation as Method, Choreographic Research
- **From Anthropology**: Multi-Sited Ethnography, Sensory Ethnography, Digital Ethnography
- **From History**: Microhistory, Prosopography, Counterfactual History

### 2.2 Expand Theory/Framework Cards (+10 cards → 30 total)
**Suggested Additions**:
- **New Materialism** (Embodied, Aesthetic)
- **Practice Theory** (Pragmatist, Constructivist)
- **Assemblage Theory** (Constructivist, Critical)
- **Object-Oriented Ontology** (Realism, Aesthetic)
- **Crip Theory** (Feminist, Critical)
- **Ecocriticism** (Critical, Interpretivism)
- **Decolonial Theory** (Critical, Feminist)
- **Posthumanism** (Aesthetic, Critical)
- **Systems Theory** (Objectivism, Pragmatist)
- **Critical Disability Studies** (Critical, Feminist)

### 2.3 Add New Epistemology Cards (+3 cards → 12 total)
**Suggested Additions**:
- **Indigenous Epistemology** (Compatible: Constructivism, Relativism)
- **Anarchist Epistemology** (Compatible: Critical, Constructivism)
- **Speculative Epistemology** (Compatible: Aesthetic, Constructivism)

### 2.4 Expand Event Cards (+10 cards → 25 total)
**Categories to Balance**:
- **Beneficial Events** (5 new): Summer School, Archive Digitization, Mentorship Grant, Research Group, Open Access Fund
- **Challenging Events** (3 new): Journal Rejection, Scope Creep, Incomplete Data
- **Interactive Events** (2 new): Method Swap (trade cards with opponent), Peer Review Circle (all players gain benefits)

### 2.5 More Diverse Object-of-Study Cards (+10 cards → 30 total)
**Suggested Additions**:
- **Disability Representation in Media**
- **Colonial Architecture & Urban Planning**
- **Sonic Branding & Audio Logos**
- **Memes & Internet Culture**
- **Climate Fiction (Cli-Fi)**
- **Surveillance Technologies**
- **Trans Narratives in Film**
- **Refugee & Migration Stories**
- **Platform Capitalism**
- **Indigenous Knowledge Systems**

---

## 3. NEW CARD TYPES (Priority: Low)

### 3.1 Advisor Cards (New type: 10 cards)
**Mechanic**: Play alongside a stack to provide ongoing benefits.

**Examples**:
- **Critical Theorist**: Methods in this stack ignore Ethical Penalties
- **Data Scientist**: +2 Reproducibility to all Methods in this stack
- **Creative Practitioner**: +2 Sensibility to all Methods in this stack
- **Methodologist**: May include 4 Methods instead of max 3
- **Interdisciplinary Scholar**: May use Theory cards from any alignment

### 3.2 Publication Cards (New type: 8 cards)
**Mechanic**: Play after completing a stack for bonus scoring.

**Examples**:
- **Peer-Reviewed Journal**: +5 points if Reproducibility ≥ 6
- **Arts Monograph**: +5 points if Sensibility ≥ 7
- **Public Engagement**: +3 points and draw 2 cards
- **Open Access**: Score immediately without completing stack (50% points)

---

## 4. FILE STRUCTURE IMPROVEMENTS

### 4.1 Create Organized Directory Structure
```
/MethodologyMatch
├── /docs
│   ├── rules_v1.md (move here)
│   ├── rules_v2.md (expanded rulebook)
│   ├── quick_start_guide.md
│   ├── FAQ.md
│   └── design_philosophy.md
├── /cards
│   ├── cards_master.csv (rename from Methodology_Match_cards_02.csv)
│   ├── cards_v2_expanded.csv
│   ├── /exports
│   │   ├── ontology_cards.json
│   │   ├── epistemology_cards.json
│   │   ├── theory_cards.json
│   │   ├── method_cards.json
│   │   └── event_cards.json
│   └── synergy_matrix.csv
├── /assets
│   ├── /card-templates
│   └── /icons
├── /tools
│   ├── card_validator.py
│   ├── score_calculator.html
│   └── deck_builder.py
├── /web-app (future)
│   ├── index.html
│   ├── game.js
│   └── styles.css
└── README.md
```

### 4.2 Create Player Aid Documents
- [ ] **Reference Sheet**: One-page summary of scoring rules
- [ ] **Epistemology Compatibility Chart**: Visual matrix of compatibilities
- [ ] **Method Quick Reference**: All methods with their scores
- [ ] **Theory Alignment Guide**: Which theories work with which epistemologies

### 4.3 Digital Tools
- [ ] **Card Database Website**: Searchable, filterable card list
- [ ] **Score Calculator**: Web tool for calculating stack scores
- [ ] **Deck Validator**: Script to check card counts and balance
- [ ] **Print-and-Play Generator**: Generate printable card sheets

---

## 5. GAMEPLAY IMPROVEMENTS

### 5.1 Enhanced Object-of-Study Mechanics
**Current**: Vague +2 for "thematic alignment"

**Proposed**:
- Add **Keywords** to Object-of-Study cards (e.g., "Visual", "Historical", "Digital", "Political")
- Add matching **Keywords** to Methods and Theories
- **Scoring**: +1 point per keyword match (max +3)

### 5.2 Paradigm Chain Refinement
**Current Issue**: "Incompatible Paradigm" is too punishing (-5 points)

**Proposed**:
- Reduce penalty to **-3 points** (still discourages but not devastating)
- Add **"Risky Research" bonus**: If you complete an incompatible paradigm AND have high novelty (avg ≥ 7), gain +5 points instead of -5

### 5.3 Two-Player Variant
**Current**: Game designed for 3 players

**Proposed**:
- Reduce starting hand to **5 cards**
- Use **2 Object-of-Study cards** instead of 1 (both in play)
- Add **Draft Phase**: Draw 3, keep 1, pass 2 (for more control)

### 5.4 Solo/Co-op Mode
**Proposed "Publish or Perish" Solo Mode**:
- Goal: Complete 2 stacks with combined score ≥ 50 before Event deck runs out
- Draw 1 Event card per turn (timed pressure)
- Score tiers: <30 = Needs Revision, 30-49 = Minor Corrections, 50+ = Accepted!

---

## 6. BALANCE ADJUSTMENTS

### 6.1 Method Card Rebalancing
**Issue**: Some methods have extreme scores that limit playability.

**Adjustments**:
| Method | Current Reproducibility | Proposed | Current Sensibility | Proposed |
|--------|------------------------|----------|-------------------|----------|
| Autoethnography | 2 | 3 | 9 | 9 |
| Statistical Analysis | 9 | 8 | 2 | 3 |
| Performance Ethnography | 2 | 3 | 9 | 9 |

### 6.2 Event Card Rebalancing
**Issue**: Power level inconsistency

**Adjustments**:
- **Major Breakthrough**: Limit to once per game (shuffle back into deck if drawn again)
- **Catastrophic Hard Drive Failure**: Add "or discard 5 cards" alternative
- **Prestigious Fellowship**: Reduce max hand size to 8 (not 9)

### 6.3 Theory Card Point Adjustment
**Current**: Highly Specialized (+7), Standard (+5), Broad (+3)

**Issue**: +7 theories are too hard to use (only 1 alignment)

**Proposed**: +6 / +4 / +3 (slightly reduce gap)

---

## 7. EXPANSION PACK IDEAS

### 7.1 "STEM Edition" Expansion
- New cards for Science/Engineering research
- Add **Empirical Ontology**
- Add **Computational Methods**: Machine Learning, Simulation, etc.

### 7.2 "Practice-Based Research" Expansion
- More Methods from creative practice
- More Aesthetic & Embodied epistemologies
- New card type: **Artefact Cards**

### 7.3 "The Conference Circuit" Mini-Expansion (15 cards)
- Event cards focused on academic conferences
- Travel, networking, presentation mishaps

### 7.4 "Global Perspectives" Expansion
- Indigenous, Decolonial, and Non-Western methodologies
- New Ontology: **Relational Ontology**
- Methods from Global South research traditions

---

## 8. PLAYTESTING PRIORITIES

### Phase 1: Core Balance
- [ ] Test with current 41 methods
- [ ] Verify scoring feels fair
- [ ] Check game length (should be 30-45 min)

### Phase 2: Expanded Content
- [ ] Add 6 methods to reach 47
- [ ] Test Object-of-Study keyword system
- [ ] Balance Event cards

### Phase 3: New Mechanics
- [ ] Test Advisor cards
- [ ] Test Publication cards
- [ ] Test solo mode

---

## 9. IMPLEMENTATION ROADMAP

### Q1 2025: Foundation
- Fix card count discrepancy
- Complete synergy matrix
- Reorganize file structure
- Create reference documents

### Q2 2025: Content Expansion
- Add 20+ new Method cards
- Add 10 new Theory cards
- Balance Event cards
- Create web-based card database

### Q3 2025: New Features
- Design and test Advisor cards
- Design and test Publication cards
- Develop digital score calculator
- Create print-and-play PDF

### Q4 2025: Polish & Release
- Professional card design
- Comprehensive rulebook v2
- Launch website
- Release expansion packs

---

## 10. NEXT STEPS

1. **Validate current card data**: Audit CSV for errors and inconsistencies
2. **Create synergy matrix**: Spreadsheet showing all Method-Epistemology synergies
3. **Add missing Method cards**: Design 6 new methods to reach 47
4. **Playtest current version**: Gather feedback before major changes
5. **Reorganize files**: Implement new folder structure
6. **Document design decisions**: Why certain scores/alignments were chosen

---

## Questions for Discussion

1. **Target Audience**: Is this primarily for PhD students, or should it be accessible to undergrads too?
2. **Complexity Level**: Keep current complexity or simplify for wider appeal?
3. **Digital vs Physical**: Priority on print-and-play or web app version?
4. **Expansion Priority**: Which expansion (STEM, Practice-Based, Global) interests you most?
5. **Playtesting**: Do you have access to playtest groups?

---

*Last Updated: 2025-11-06*
