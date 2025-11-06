# Methodology Match: Implementation & Playtesting Plan

**Version**: 1.0
**Date**: 2025-11-06
**Purpose**: Plan for implementing and testing Methodology Match gameplay

---

## 1. Implementation Approaches

### Option A: Digital Prototype (Recommended First)
**Platform**: Tabletop Simulator or web-based (tabletop.io, PlayingCards.io)

**Advantages**:
- Fast iteration - update cards instantly
- Remote testing with distributed players
- Track game state automatically
- Easy to document and record sessions
- No printing costs during iteration

**Disadvantages**:
- Requires technical setup
- Less tactile than physical cards
- May have learning curve for platform

**Recommended**: Start here for rapid iteration

---

### Option B: Print-and-Play Prototype
**Format**: PDF cards printed on cardstock or paper + sleeves

**Advantages**:
- Physical tactile experience
- No technical barriers
- Easier to assess card text readability
- Real spatial layout testing
- Can playtest offline

**Disadvantages**:
- Slower iteration (reprint after changes)
- Printing costs
- Physical logistics

**Recommended**: Use after 2-3 digital playtests stabilize rules

---

### Option C: Hybrid Approach (Recommended)
1. **Phase 1** (Weeks 1-2): Digital playtesting for rules refinement
2. **Phase 2** (Weeks 3-4): Print-and-play for physical UX testing
3. **Phase 3** (Week 5+): Refined digital + physical testing

---

## 2. Implementation Requirements

### Digital Implementation Needs
- [ ] Card images for all 116 cards
- [ ] Rules reference sheet
- [ ] Player aid (scoring quick reference)
- [ ] Sample starting hands for testing
- [ ] Virtual table setup (deck, discard, play areas)

### Print-and-Play Needs
- [ ] Card templates (standard size: 63.5mm × 88mm / poker size)
- [ ] Printable PDF sheets (9 cards per page)
- [ ] Rules booklet (printable)
- [ ] Score tracking sheet
- [ ] Quick reference card

---

## 3. Playtesting Goals & Questions

### Core Mechanics Testing

**Turn Structure**:
- [ ] Is draw-play-discard flow intuitive?
- [ ] Do players understand when they can play each card type?
- [ ] Is the 7-card hand limit appropriate?
- [ ] Does the game move at good pace?

**Stack Building**:
- [ ] Can players understand what makes a valid stack?
- [ ] Is the Ontology-Epistemology-Theory-Method chain clear?
- [ ] Are stack requirements (1 Ontology, 1 Epistemology, 0-2 Theory, 1-3 Methods) balanced?
- [ ] Do players struggle to complete stacks (too restrictive)?
- [ ] Do stacks complete too easily (too permissive)?

**Compatibility/Synergy System**:
- [ ] Do players understand Ontology-Epistemology compatibility?
- [ ] Can they identify which Methods synergize with which Epistemologies?
- [ ] Is the Coherent vs Incompatible vs Mixed paradigm system clear?
- [ ] Are incompatibility penalties too harsh or too lenient?

---

### Balance Testing

**Point Distribution**:
- [ ] What's the typical score range? (target: 20-40 points per player)
- [ ] What's the gap between winner and loser? (target: 5-15 points)
- [ ] Which scoring mechanisms dominate? (Paradigm bonus, Theory bonus, Ontology effects)
- [ ] Are any cards overpowered or underpowered?

**Strategy Diversity**:
- [ ] Can players win with different Ontologies?
- [ ] Are Positivist and Interpretivist approaches equally viable?
- [ ] Do highly specialized Theories (7 points) provide enough value?
- [ ] Is there strategic variety or does optimal strategy emerge?

**Card Distribution**:
- [ ] Are there enough Methods for each Epistemology?
- [ ] Do players get stuck unable to complete stacks?
- [ ] Is deck size (116 cards) appropriate for 2-4 players?
- [ ] Should hand size vary by player count?

**Methodological Extremes Rule**:
- [ ] Does the extra discard cost (Reproducibility/Sensibility ≤ 2) create interesting choices?
- [ ] Is this penalty too harsh or too lenient?
- [ ] Do players avoid extreme methods or embrace them strategically?

---

### Usability Testing

**Card Clarity**:
- [ ] Is text readable at card size?
- [ ] Are Method descriptions too long/short?
- [ ] Do players understand what each card does?
- [ ] Are synergies clearly marked?
- [ ] Can players quickly identify card types?

**Rules Clarity**:
- [ ] Which rules cause confusion?
- [ ] What questions do players ask repeatedly?
- [ ] Where do rules need examples?
- [ ] Are edge cases covered?

**Learning Curve**:
- [ ] How long does rules explanation take? (target: 10-15 minutes)
- [ ] How many turns before players feel comfortable? (target: 2-3 rounds)
- [ ] What's the biggest learning barrier?

---

### Educational Value Testing

**Methodological Learning**:
- [ ] Do players learn about research methods?
- [ ] Do they understand epistemological differences?
- [ ] Can they explain why certain combinations are coherent/incompatible?
- [ ] Do card descriptions provide useful information?

**Engagement**:
- [ ] Do players enjoy the educational aspect?
- [ ] Is the game "too academic" or "not academic enough"?
- [ ] Do humanities PhD students find it relevant?
- [ ] Does it spark methodological discussions?

---

## 4. Testing Protocol

### Test Session Structure

**Pre-Session** (5 minutes):
- Explain rules using rulebook
- Show example stacks
- Answer clarifying questions

**Play Session** (30-60 minutes):
- 2-4 players complete a full game
- Observer takes notes (or video record)
- Players think aloud when possible

**Post-Session Debrief** (15 minutes):
- Structured feedback questions
- Open discussion
- What was fun? What was frustrating?
- Suggested changes

---

### Observation Checklist

During gameplay, observe:
- [ ] Moments of confusion (write down exact situation)
- [ ] Rules disputes or clarification requests
- [ ] Player engagement level (are they enjoying it?)
- [ ] Decision-making time (are turns quick or slow?)
- [ ] Use of different strategies
- [ ] Which cards are played frequently vs rarely
- [ ] Whether players read Method card descriptions
- [ ] Emotional responses (frustration, satisfaction, excitement)

---

### Data Collection

**Quantitative Data**:
- Game duration
- Final scores (all players)
- Number of turns to complete first stack
- Number of turns to complete second stack
- Score breakdown (Paradigm, Theory, Ontology, Supplemental, Final Awards)
- Card distribution: which Ontologies/Epistemologies/Methods were played
- How many Methods with Methodological Extremes penalty were played

**Qualitative Data**:
- Player feedback quotes
- Observed confusion points
- Suggested rule changes
- Favorite/least favorite aspects
- Educational insights gained

---

## 5. Testing Phases

### Phase 1: Developer Testing (Solo & 2-player)
**Goal**: Validate basic mechanics work

**Tests**:
1. **Solo "dummy" game**: Play all hands yourself to verify rules logic
2. **2-player test**: Play with colleague who understands design intent
3. **Focus**: Rules consistency, basic flow, obvious exploits

**Success Criteria**:
- Game completes without breaking
- Rules are internally consistent
- No obviously overpowered strategies

**Duration**: 2-3 sessions

---

### Phase 2: Blind Playtesting (3-4 players)
**Goal**: Test rules clarity with fresh eyes

**Tests**:
1. Give rulebook to players who haven't seen the game
2. Minimal designer intervention (only answer direct questions)
3. Observe where confusion occurs

**Success Criteria**:
- Players can complete a game with minimal help
- Rules disputes are rare
- Players enjoy the experience

**Duration**: 3-5 sessions with different groups

---

### Phase 3: Balance Testing (Multiple sessions, varied players)
**Goal**: Refine scoring and card balance

**Tests**:
1. Track all game data (scores, cards played, strategies)
2. Identify dominant strategies or cards
3. Test specific balance changes

**Success Criteria**:
- Score variance is reasonable
- Multiple strategies are viable
- No cards are ignored/broken

**Duration**: 5-10 sessions

---

### Phase 4: Educational Testing (PhD students)
**Goal**: Validate educational value with target audience

**Tests**:
1. Playtest with actual humanities/arts/design PhD students
2. Pre/post questionnaire on methodological understanding
3. Discussion on learning value

**Success Criteria**:
- Students report learning about methods
- Game sparks methodological discussions
- Students would recommend to peers

**Duration**: 3-5 sessions with different cohorts

---

## 6. Feedback Collection Tools

### Feedback Form Template

**Player Information**:
- Name (optional)
- Research discipline
- Familiarity with research methods (1-5 scale)
- Gaming experience (1-5 scale)

**Gameplay Experience** (1-5 scale):
- How easy were the rules to learn?
- How clear were the card descriptions?
- How engaging was the gameplay?
- How balanced did the game feel?
- How much did you learn about research methods?

**Open Questions**:
1. What was the most confusing part of the game?
2. What was the most enjoyable part?
3. What was the most frustrating part?
4. Which cards or mechanics need clarification?
5. What would you change?
6. Would you play this again?
7. Would you recommend it to other researchers?

**Educational Value**:
1. Did you learn anything new about research methods?
2. Did the game change how you think about methodological coherence?
3. Which Method cards were most interesting/surprising?

---

### Change Tracking System

**Issue Log Format**:
| Issue # | Date | Category | Description | Severity | Proposed Fix | Status |
|---------|------|----------|-------------|----------|--------------|--------|
| 001 | 2025-11-06 | Rules | Players confused about when to score | High | Add example in rulebook | Open |
| 002 | 2025-11-06 | Balance | Realism Ontology too weak | Medium | Increase bonus to +3 | Open |

**Categories**:
- Rules clarity
- Card text
- Balance
- Strategy
- Educational value
- Physical design
- Other

**Severity**:
- Critical (breaks game)
- High (major confusion/frustration)
- Medium (noticeable issue)
- Low (minor polish)

---

## 7. Iteration Process

### After Each Playtest Session:

1. **Immediate Debrief** (same day):
   - Review notes
   - Log all issues
   - Prioritize by severity

2. **Analysis** (1-2 days):
   - Identify patterns across multiple sessions
   - Propose specific changes
   - Consider knock-on effects

3. **Changes** (before next test):
   - Update rulebook
   - Modify card CSV
   - Document what changed and why
   - Create new version number

4. **Communication**:
   - Share changes with playtesters
   - Explain rationale
   - Request specific focus areas for next test

### Version Control:
- Use git branches for major changes
- Tag stable versions (v1.0, v1.1, etc.)
- Keep changelog of all rule/card modifications
- Archive all playtest versions

---

## 8. Specific Testing Scenarios

### Scenario 1: Minimum Viable Game
**Setup**: 2 players, simplified rules
**Goal**: Verify core loop works
**Focus**: Draw-play-discard, stack building, scoring

### Scenario 2: Full Game (3-4 players)
**Setup**: Complete rules, all cards
**Goal**: Test full experience
**Focus**: Game length, balance, interaction

### Scenario 3: Edge Cases
**Setup**: Deliberately create edge case situations
**Test Cases**:
- What if draw pile runs out before anyone completes second stack?
- What if all players have incompatible Ontology-Epistemology?
- What if player can't legally play any card?
- What if Event card creates impossible situation?

### Scenario 4: Strategy Testing
**Setup**: Experienced players, multiple games
**Goal**: Identify optimal strategies
**Focus**: Does diversity of winning strategies exist?

### Scenario 5: Educational Testing
**Setup**: Pre-teach some methods, see if game reinforces
**Goal**: Measure learning outcomes
**Focus**: Knowledge retention, conceptual understanding

---

## 9. Success Metrics

### Minimum Viable Product Success:
- [ ] Game completes without breaking
- [ ] Players understand how to win
- [ ] No critical rules issues
- [ ] At least 3/5 enjoyment rating

### Beta Version Success:
- [ ] Game completes in 45-60 minutes
- [ ] Scores range 20-40 points
- [ ] Score gap 5-15 points
- [ ] 4/5 enjoyment rating
- [ ] Rules clarity 4/5
- [ ] Players report learning about methods

### Release Candidate Success:
- [ ] 10+ successful playtests
- [ ] No critical or high-severity issues remaining
- [ ] 4.5/5 enjoyment rating
- [ ] PhD students enthusiastically recommend
- [ ] Clear documentation for self-publishing

---

## 10. Implementation Timeline

### Week 1-2: Digital Prototype
- [ ] Create simple card images (text-based, minimal design)
- [ ] Set up digital platform (Tabletop Simulator or web)
- [ ] Conduct 2-3 developer tests
- [ ] Log initial issues

### Week 3-4: Blind Playtesting
- [ ] Recruit 3-5 playtest groups (2-4 players each)
- [ ] Conduct blind playtests
- [ ] Collect feedback
- [ ] Make first round of changes

### Week 5-6: Balance Iteration
- [ ] Test with updated rules/cards
- [ ] Track quantitative data
- [ ] Identify balance issues
- [ ] Refine scoring systems

### Week 7-8: Physical Prototype
- [ ] Create print-and-play version
- [ ] Test physical card UX
- [ ] Refine card text for readability
- [ ] Test card design templates

### Week 9-10: Educational Validation
- [ ] Playtest with PhD students
- [ ] Assess learning outcomes
- [ ] Final refinements
- [ ] Prepare for publication

---

## 11. Tools & Resources Needed

### Digital Implementation:
- [ ] Spreadsheet for card data export
- [ ] Card image generator (Python script or template)
- [ ] Tabletop Simulator workshop or PlayingCards.io account
- [ ] Screen recording software (for remote playtests)

### Physical Prototyping:
- [ ] Card template (InDesign/Figma/Canva)
- [ ] Printer access
- [ ] Cardstock or card sleeves
- [ ] Scissors/paper cutter

### Data Collection:
- [ ] Feedback form (Google Forms/Typeform)
- [ ] Spreadsheet for tracking game data
- [ ] Issue tracking system (GitHub issues or Trello)
- [ ] Note-taking template

### Communication:
- [ ] Playtester recruitment email template
- [ ] Consent form (if recording sessions)
- [ ] Thank you message template

---

## 12. Known Risks & Mitigation

### Risk 1: Game too complex for casual play
**Mitigation**: Create "simplified" variant, test with non-academics

### Risk 2: Game too long
**Mitigation**: Add timer, reduce stack requirements, or reduce hand size

### Risk 3: Too few players available
**Mitigation**: Develop solo mode, recruit via university networks

### Risk 4: Balance issues hard to identify
**Mitigation**: Systematic data collection, mathematical modeling of scoring

### Risk 5: Educational value unclear
**Mitigation**: Pre/post knowledge assessment, focus groups

### Risk 6: Changes create new issues
**Mitigation**: Version control, thorough documentation, regression testing

---

## 13. Post-Testing Deliverables

After playtesting phase, produce:
1. **Finalized Rulebook** (with examples and edge cases)
2. **Finalized Card CSV** (with any balance changes)
3. **Playtest Report** (summary of findings and changes)
4. **Print-and-Play PDF** (ready for distribution)
5. **Manufacturing Specifications** (if pursuing publication)
6. **Educator's Guide** (how to use in teaching)

---

## Next Steps

1. Choose implementation approach (Digital/Physical/Hybrid)
2. Create first playable prototype
3. Recruit playtesters
4. Conduct first session
5. Begin iteration loop

**Recommended First Action**: Create digital prototype using PlayingCards.io (free, quick setup, shareable link for remote testing)
