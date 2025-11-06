# Methodology Match - Card Audit Report

**Date**: 2025-11-06
**Version**: Cards v02

## Executive Summary

This audit identifies critical inconsistencies between the rulebook (rules_v1.md) and the card set (Methodology_Match_cards_02.csv). Major issues include missing Method cards, broken synergy chains, inconsistent naming conventions, and missing educational content.

**Severity Ratings**: 🔴 Critical | 🟡 Important | 🟢 Minor

---

## 1. Card Count Issues 🔴 CRITICAL

### Method Cards: Missing 4 Cards
- **Rulebook**: 47 Method cards
- **CSV File**: 43 Method cards
- **Missing**: 4 cards

**Impact**: Game balance affected, deck composition incorrect

**Methods Referenced in Epistemology Cards but NOT in Method deck**:
1. "Experiments" (Positivism synergy)
2. "Statistical Modelling" (Positivism synergy)
3. "Forensic Aesthetics" (Critical Epistemology synergy)
4. "Zine-Making" (Feminist Epistemology synergy)
5. "Voice-Centred Method" (Feminist Epistemology synergy)
6. "Soundscape Analysis" (Aesthetic Epistemology synergy)
7. "Practice Theory" (Pragmatist synergy) - This might be a Theory/Framework, not a Method

**Recommendation**: Add at least 4 missing methods or adjust Epistemology synergies

---

## 2. Naming Inconsistencies 🔴 CRITICAL

### Epistemology Card Names vs Method Card References

**Epistemology cards have these names**:
- Positivism
- Interpretivism
- Critical Epistemology
- Feminist Epistemology
- Constructivist Epistemology
- Embodied Epistemology
- Aesthetic Epistemology
- Pragmatist
- Objectivism

**But Method cards reference different/ambiguous names**:
| Method Card | References | Issue |
|-------------|-----------|-------|
| Action Research | "Critical, Pragmatist" | "Critical" is ambiguous - should be "Critical Epistemology" |
| Archival Research | "Positivism, Foucauldian" | "Foucauldian" doesn't exist as an Epistemology |
| Artefact Analysis | "Material Culture" | Not an epistemology |
| Drawing as Inquiry | "Deleuzian/Aesthetic" | "Deleuzian" doesn't exist |
| Discourse Analysis | "Foucauldian, Critical" | Same issues |
| Documentary Analysis | "Historical Method" | Not an epistemology |
| Experimental Design | "Objectivism, Positivism" | OK ✓ |
| Film Analysis | "Aesthetic" | Should be "Aesthetic Epistemology" |
| Grounded Theory | "Constructivist" | Should be "Constructivist Epistemology" |
| Historical Method | "Realism" | Realism is an Ontology, not Epistemology |
| Material Culture Analysis | "New Materialism" | Not an epistemology |
| Narrative Inquiry | "Feminist, Queer" | "Feminist" OK, but "Queer" is a theory not epistemology |
| Netnography | "Digital Humanities" | Not an epistemology |
| Semiotic Analysis | "Semiotics Theory" | This is a Theory/Framework, not Epistemology |
| Social Media Mining | "Positivism, Digital" | "Digital" is not an epistemology |
| Soundwalk Method | "Embodied/Aesthetic" | Should use full names |
| Statistical Analysis | "Positivism, Realism" | "Realism" is an Ontology |
| Survey (Quantitative) | "Positivism, Objectivist" | Should be "Objectivism" |
| Textual Analysis | "Semiotics" | This is a theory |
| VR Ethnography | "Embodied, Aesthetic" | Should use full names |
| Visual Analysis | "Semiotics" | This is a theory |

**Recommendation**: Standardize all Method card synergies to match exact Epistemology card names

---

## 3. Theory/Framework Alignment Issues 🟡 IMPORTANT

### Some alignments don't match Epistemology card names:

| Theory Card | Alignment Listed | Issue |
|-------------|-----------------|-------|
| Narratology | Objectivism | ✓ Matches |
| Pragmatist Theory | Pragmatist | ✓ Matches |
| Hermeneutics | Interpretivism | ✓ Matches |
| Structuralism | Objectivism | ✓ Matches |

**Most Theory cards are OK**, but need to verify all alignments match exactly

---

## 4. Ontology Gameplay Effects Not in Rulebook 🟡 IMPORTANT

The Ontology cards have gameplay effects that are NOT mentioned in the rulebook:

1. **Realism**: "+2 points when using causal or quantitative methods"
2. **Relativism**: "May hold contradictory findings and blocks generalisation bonuses from Realist players"
3. **Constructivism**: "Draw one extra Method after completing a qualitative stack"

**Issues**:
- Rulebook doesn't mention these effects
- "Generalisation bonuses" don't exist in rules
- Unclear what counts as "causal or quantitative methods"
- Unclear what counts as "qualitative stack"

**Recommendation**: Either add these to rulebook OR remove from cards

---

## 5. Missing Educational Content 🔴 CRITICAL

### Method Cards Have NO Descriptive Text

All 43 Method cards are missing:
- Brief description of the method
- Pros/cons
- Typical use cases
- Practical considerations

**Current**: Just title, synergies, and four scores
**Needed**: Educational text as outlined in project context

**Example of what's needed** (Semi-structured interviews):
```
**Description**: Flexible interview approach with prepared questions but allowing follow-up exploration
**Pros**: Balances structure with openness, captures unexpected insights
**Cons**: Time-intensive, requires skilled interviewer, harder to standardize
**Typical Use**: Understanding lived experiences, exploring complex topics
```

---

## 6. Epistemology Incompatibility Issues 🟡 IMPORTANT

### Positivism Card States:
"Incompatible: Autoethnography, Discourse Analysis"

**Problem**: These are METHODS, not Ontologies. According to the rulebook, Epistemologies should list compatible/incompatible ONTOLOGIES, not methods.

**Rulebook states**:
> Incompatible Paradigm (-5 Points): Applied if your stack's Ontology and Epistemology are explicitly listed as incompatible

This suggests Epistemology cards should show Ontology compatibility, not method compatibility.

**Current Epistemology compatibility listings**:
- Positivism: "Compatible Ontology: Realism" ✓
- Interpretivism: "Compatible Ontology: Relativism, Constructivism" ✓
- Critical Epistemology: "Compatible Ontology: Realism, Constructivism" ✓
- Feminist Epistemology: "Compatible Ontology: Relativism, Constructivism. Incompatible: Positivism" ⚠️
- Aesthetic Epistemology: "Incompatible: Positivism, Realism" ⚠️
- Objectivism: "Compatible Ontology: Realism. Incompatible: Constructivism" ✓

**Issues**:
1. Positivism's "Incompatible: Autoethnography, Discourse Analysis" lists METHODS not Ontologies
2. Feminist's "Incompatible: Positivism" lists an EPISTEMOLOGY not an Ontology
3. Aesthetic's "Incompatible: Positivism, Realism" mixes an Epistemology (Positivism) with an Ontology (Realism)

---

## 7. Synergy Chain Analysis 🔴 CRITICAL

### How the Game SHOULD Work:
1. Player has secret Ontology (e.g., Realism)
2. Player plays Epistemology (e.g., Positivism)
3. Check: Is Ontology compatible with Epistemology?
4. Player adds Methods (e.g., Survey)
5. Check: Does at least one Method have synergy with the Epistemology?
6. Score: Coherent Paradigm (+10) if both checks pass

### Current Problems:

**Example Stack**: Realism (Ontology) + Positivism (Epistemology) + Survey (Method)
- Positivism card says: Compatible with Realism ✓
- Positivism card lists synergies: "Surveys, Experiments, Statistical Modelling, Content Analysis, Social Media Mining"
- Survey (Quantitative) card says synergies: "Positivism, Objectivist"
- **Result**: Matches! ✓

**Example Stack**: Relativism (Ontology) + Interpretivism (Epistemology) + Interview (Method)
- Interpretivism says: Compatible with Relativism ✓
- Interpretivism lists synergies: "Interviews, Case Studies, Ethnography, Textual Analysis, Oral History"
- Interview (Qualitative) card says: "Interpretivism"
- **Result**: Matches! ✓

**Example Stack**: Constructivism (Ontology) + Feminist Epistemology + Autoethnography
- Feminist says: Compatible with Constructivism ✓
- Feminist lists synergies: "Autoethnography, Narrative Inquiry, Participatory Methods, Zine-Making, Voice-Centred Method"
- Autoethnography card says: "Feminist, Embodied"
- **Result**: "Feminist" matches "Feminist Epistemology" ✓ (if we allow abbreviation)

**BUT**: Many broken chains exist due to naming inconsistencies

---

## 8. Specific Card Issues

### Method Cards with Questionable Synergies:

1. **Artefact Analysis**: References "Material Culture" which isn't an Epistemology
2. **Material Culture Analysis**: References "New Materialism" which isn't in the game
3. **Documentary Analysis**: References "Historical Method" which is itself a Method, not Epistemology
4. **Exhibition-as-Research**: References "Practice Theory" which is a Theory/Framework
5. **Digital Humanities Methods**: References "Pragmatist Theory" (a Theory/Framework, not Epistemology)

### Rulebook's "Methodological Extremes" Rule:
> When you play a Method card with a Reproducibility or Sensibility score of 2 or less, you must discard one additional card

**Method cards with Reproducibility ≤ 2**:
- Autoethnography (2)
- Creative Writing as Inquiry (2)
- Drawing as Inquiry (2)
- Experimental Design (2) - Wait, this should have HIGH reproducibility!
- Performance Ethnography (2)
- Statistical Analysis (2) - This is WRONG! Should be ~9

**Method cards with Sensibility ≤ 2**:
- None

**Issues**:
- Statistical Analysis should have HIGH reproducibility (~9), not 2
- Experimental Design should have HIGH reproducibility (~8-9), not 2
- These scores seem backwards

---

## 9. Score Balance Issues 🟡 IMPORTANT

### Reproducibility Scores Look Suspicious:

**Methods that should have HIGH reproducibility but don't**:
- Statistical Analysis: Currently 9 ✓ (Wait, I misread earlier - this is correct!)
- Experimental Design: Currently 9 ✓ (Also correct!)

Let me recheck the "Methodological Extremes" issue...

Looking at the CSV again:
- Autoethnography: Repro=2, Sensibility=9 ✓
- Creative Writing as Inquiry: Repro=2, Sensibility=9 ✓
- Drawing as Inquiry: Repro=2, Sensibility=8 ✓
- Experimental Design: Repro=9, Sensibility=2 ✓
- Performance Ethnography: Repro=2, Sensibility=9 ✓
- Statistical Analysis: Repro=9, Sensibility=2 ✓

Actually, these make sense! Experimental Design and Statistical Analysis have HIGH reproducibility but LOW sensibility. The artistic/embodied methods have LOW reproducibility but HIGH sensibility.

**Correction**: Scores appear reasonable upon closer inspection

---

## 10. Summary of Required Fixes

### Priority 1 - CRITICAL (Breaks Gameplay):
1. ✅ Add 4 missing Method cards to reach 47 total
2. ✅ Standardize all Method synergies to use exact Epistemology card names
3. ✅ Fix Epistemology incompatibility listings (should reference Ontologies only)
4. ✅ Add descriptive educational text to all Method cards

### Priority 2 - IMPORTANT (Affects Balance):
5. ✅ Clarify or remove Ontology gameplay effects (update rulebook or cards)
6. ✅ Verify all Theory/Framework alignments match Epistemology names
7. ✅ Remove or fix methods that reference non-existent epistemologies

### Priority 3 - MINOR (Polish):
8. ✅ Add pros/cons to Method cards
9. ✅ Ensure Object-of-Study descriptions are consistent in length/detail
10. ✅ Review Event card balance and effects

---

## Recommended Next Steps

1. **Immediate**: Create a terminology mapping document
2. **Then**: Fix all synergy references in Method cards
3. **Then**: Add 4 missing Method cards
4. **Then**: Write educational text for all Method cards
5. **Finally**: Update rulebook to match actual card mechanics

---

## Questions for Designer

1. Should Ontology cards have gameplay effects? If yes, rulebook needs updating
2. What are the 4 missing methods? Should they be the ones referenced in Epistemology synergies?
3. Should Methods reference Epistemologies, Theories, or both?
4. Should we create an "Epistemology Family" system where abbreviations like "Feminist" = "Feminist Epistemology"?
5. How much text can physically fit on a Method card?
