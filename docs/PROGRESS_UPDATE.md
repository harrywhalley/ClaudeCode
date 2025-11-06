# Methodology Match: Progress Update

**Date**: 2025-11-06
**Status**: Options C & D Complete ✅

---

## ✅ COMPLETED: Option C - Fix Ontology Issues

### New Ontology Cards (3 → 5)

**Added 2 New Ontologies**:

1. **Critical Realism**
   - Combines realist ontology with interpretive epistemology
   - Bridges quantitative and qualitative approaches
   - Gameplay Effect: +3 points if stack includes Methods with both Reproducibility 6+ AND Sensibility 6+
   - Compatible with: All epistemologies except Aesthetic

2. **Relational Ontology**
   - Reality exists in relationships, not isolated entities
   - Central to Indigenous philosophies and ecological thinking
   - Gameplay Effect: +3 points if stack includes Participatory Methods, Action Research, or Ethnography
   - Compatible with: Constructivism, Relativism, Feminist, Critical, Embodied, Pragmatist

### Revised All Existing Ontology Cards

**Realism**:
- Clearer philosophical description
- Gameplay Effect: +2 points if stack includes a Method with Reproducibility 8+
- Objective and easy to verify

**Relativism**:
- Updated description for clarity
- Gameplay Effect: +2 points if stack includes Methods from different paradigms (one with Reproducibility 7+, one with Sensibility 7+)
- Rewards methodological diversity

**Constructivism**:
- Enhanced description
- Gameplay Effect: When completing a stack with 2+ Methods with Sensibility 7+, draw 1 card (then discard to 7)
- Rewards qualitative depth

### Game Impact

- **Player Count**: Now supports 2-5 players (was locked to 3)
- **Ontology Draft**: New mechanic where players draft Ontologies face-up for strategic choice
- **2-3 Player Variant**: Secret draft from 2 random Ontologies for more variety
- **Total Cards**: 118 (was 116)

### Rules Integration

- Updated docs/rules_v1.md Section 2: Game Components
- Updated docs/rules_v1.md Section 4: Game Setup (Ontology Draft)
- Updated docs/rules_v1.md Section 7.2: Added Ontology Bonus subsection
- All Epistemology cards updated with new Ontology compatibilities

---

## ✅ COMPLETED: Option D - Fix All Synergies

### Fixed Name Mismatches

**Before** → **After**:
- "Surveys" → "Survey (Quantitative)"
- "Experiments" → "Experimental Design"
- "Statistical Modelling" → "Statistical Analysis"
- "Interviews" → "Interview (Qualitative)"
- "Case Studies" → "Case Study"

### Removed Non-Existent Cards

**Feminist Epistemology**:
- ❌ Removed "Zine-Making" (doesn't exist)
- ❌ Removed "Voice-Centred Method" (doesn't exist)
- ✅ Added "Creative Writing as Inquiry"
- ✅ Added "Memory-Work Method"

**Critical Epistemology**:
- ❌ Removed "Forensic Aesthetics" (doesn't exist)
- ✅ Added "Critical Discourse Analysis"
- ✅ Added "Ethnography"

**Embodied Epistemology**:
- ❌ Removed "Affect Theory" (it's a Theory, not a Method)
- ✅ Added "Phenomenology"
- ✅ Added "Sensory Ethnography"

**Aesthetic Epistemology**:
- ❌ Removed "Soundscape Analysis" (doesn't exist)
- ❌ Removed "Affect Theory" (it's a Theory, not a Method)
- ✅ Added "Drawing as Inquiry"
- ✅ Added "Performance Ethnography"
- ✅ Added "Sensory Ethnography"

**Pragmatist Epistemology**:
- ❌ Removed "Actor-Network Theory" (it's a Theory)
- ❌ Removed "Practice Theory" (it's a Theory)
- ✅ Added "Digital Humanities Methods"
- ✅ Added "Speculative Design"
- ✅ Added "Cultural Probes"

**Constructivist Epistemology**:
- ❌ Removed "Actor-Network Theory" (it's a Theory)
- ❌ Removed "Symbolic Interactionism" (it's a Theory)
- ❌ Removed "Reader-Response" (it's a Theory)
- ✅ Added "Ethnography"
- ✅ Added "Interview (Qualitative)"
- ✅ Added "Focus Groups"

**Objectivism Epistemology**:
- ❌ Removed "Structuralism" (it's a Theory)
- ❌ Removed "Semiotics Theory" (it's a Theory)
- ❌ Removed "Marxist Theory" (it's a Theory)
- ✅ Added "Statistical Analysis"
- ✅ Added "Content Analysis"
- ✅ Added "Semiotic Analysis"

### Created Synergy Matrix

**New File**: `cards/synergy_matrix.csv`

- Visual matrix showing all 47 Methods × 9 Epistemologies
- Uses ✓ marks for easy reference
- Helpful for:
  - Players checking synergies during gameplay
  - Game designers balancing card distribution
  - Understanding epistemological alignment patterns

---

## 📊 Summary of Changes

| Component | Before | After | Status |
|-----------|--------|-------|--------|
| **Ontology Cards** | 3 | 5 | ✅ Fixed |
| **Player Count** | 3 only | 2-5 | ✅ Fixed |
| **Ontology Setup** | Random deal | Draft (strategic) | ✅ Fixed |
| **Ontology Effects** | Not in rules | Integrated | ✅ Fixed |
| **Synergy Names** | Mismatched | Exact matches | ✅ Fixed |
| **Non-existent Methods** | Listed | Removed | ✅ Fixed |
| **Theory/Method Confusion** | Mixed | Separated | ✅ Fixed |
| **Synergy Matrix** | None | Created | ✅ Created |

---

## 🎯 NEXT: Option A - Fix Scoring Clarity

### What Needs to Be Done

The cards currently don't show scoring information, requiring constant rulebook reference. This needs to be fixed by adding scoring text to all card types.

**Affected Card Types**:
1. **Method Cards** (47 cards) - Need scoring info for:
   - Ethical Risk (if ≥7: -1 point)
   - Reproducibility (contributes to Objectivity Award)
   - Sensibility (contributes to Insight Award)
   - Novelty (if avg ≥7: +3 Cutting-Edge Bonus)
   - Methodological Extremes (if Reproducibility or Sensibility ≤2: discard extra card)

2. **Theory Cards** (22 cards) - Need scoring info for:
   - Alignment-based points (+7, +5, or +3)
   - "If aligned: +X points, if not aligned: 0 points"

3. **Epistemology Cards** (9 cards) - Need scoring info for:
   - Paradigm Chain scoring (+10, -5, or +3)
   - Clear explanation of compatibility requirements

4. **Ontology Cards** (5 cards) - Already done! ✅
   - Gameplay Effects already clarified

5. **Object-of-Study Cards** (20 cards) - Need:
   - Keywords for objective matching
   - Scoring explanation (+2 if keyword matches)

6. **Event Cards** (15 cards) - Mostly OK, minor clarifications

### Approach

Create scoring reference text that can be added to each card's "Scoring Information" column. Examples already created in `cards/card_template_improved_examples.csv`.

---

## 🎯 REMAINING: Option B - Add Educational Content

### What Needs to Be Done

Add descriptions to all cards so players understand what methods and theories are.

**Method Cards** (47 cards):
- All descriptions already written in `docs/GAME_REVIEW_COMPREHENSIVE.md` Section 8
- Just need to be integrated into the cards CSV

**Theory Cards** (22 cards):
- Need 1-2 sentence descriptions
- Explain what each theoretical framework is

**Epistemology & Ontology Cards**:
- Descriptions already improved ✅

---

## 📁 Files Modified

| File | Changes |
|------|---------|
| `cards/cards_master.csv` | +2 Ontology cards, revised all Ontology descriptions, fixed all 9 Epistemology synergy lists |
| `cards/synergy_matrix.csv` | NEW - Visual reference matrix |
| `docs/rules_v1.md` | Updated card counts, added Ontology draft, integrated Ontology bonuses |

---

## 🔢 Card Count Status

| Card Type | Count | Status |
|-----------|-------|--------|
| Ontology | 5 | ✅ Complete |
| Epistemology | 9 | ✅ Complete |
| Theory/Framework | 22 | ⚠️ Need descriptions |
| Method | 47 | ⚠️ Need descriptions + scoring |
| Object-of-Study | 20 | ⚠️ Need keywords |
| Event | 15 | ✅ Mostly complete |
| **TOTAL** | **118** | |

---

## 📈 Progress Tracker

### Option C: Fix Ontology Issues ✅ COMPLETE
- [x] Design 2 new Ontology cards
- [x] Clarify all Ontology Gameplay Effects
- [x] Update rules for 2-5 player support
- [x] Add Ontology draft mechanic
- [x] Integrate Ontology bonuses into scoring rules

### Option D: Fix All Synergies ✅ COMPLETE
- [x] Standardize all Method-Epistemology name matches
- [x] Remove all non-existent cards from synergy lists
- [x] Add missing Methods to synergy lists
- [x] Separate Methods from Theories in synergy lists
- [x] Create comprehensive synergy matrix

### Option A: Fix Scoring Clarity ⏳ PENDING
- [ ] Add scoring text to all Method cards (47)
- [ ] Add scoring text to all Theory cards (22)
- [ ] Add scoring text to all Epistemology cards (9)
- [ ] Add keywords to Object-of-Study cards (20)
- [ ] Create player reference cards

### Option B: Add Educational Content ⏳ PENDING
- [ ] Integrate 47 Method descriptions (already written)
- [ ] Write 22 Theory descriptions
- [ ] Create comprehensive glossary

---

## 🚀 Next Steps

1. **Continue with Option A** - Add scoring information to all cards
2. **Then Option B** - Integrate all descriptions
3. **Create player reference cards** - Quick-reference for scoring
4. **Playtest** - Test with real players to validate changes

---

## 💾 Git Status

**Branch**: `claude/review-game-structure-011CUrjBqkircErovvuF14GW`

**Recent Commits**:
- `2b7673c` - Fix Ontology and Synergy issues (Options C & D complete)
- `2cff2d7` - Add comprehensive game review and card improvement templates
- `51cfd0b` - Reorganize project structure and complete card deck

**All changes pushed** ✅

---

*Last Updated: 2025-11-06*
