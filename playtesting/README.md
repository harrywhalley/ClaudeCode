# Methodology Match: Playtesting Folder

This folder contains all the tools, templates, and documentation needed to playtest and iterate on Methodology Match.

---

## 📁 What's in This Folder

### Core Planning Documents

**📄 implementation_plan.md** - Comprehensive guide to implementing and testing the game
- Implementation approaches (digital, physical, hybrid)
- Testing goals and questions
- Playtesting phases and timeline
- Success metrics
- Everything you need to plan playtesting

**📄 quick_start_guide.md** - Get started playtesting TODAY
- Fastest paths to first playtest
- Step-by-step setup instructions
- Minimum viable playtest approach
- First session checklist

---

### Data Collection Tools

**📄 playtest_feedback_form.md** - Structured feedback from players
- Gameplay experience ratings
- Educational value assessment
- Open-ended questions
- Use one per player per session

**📄 session_log_template.md** - Detailed session documentation
- Game data (scores, cards used, timing)
- Observations during play
- Confusion and frustration points
- Follow-up actions
- Use one per playtest session

**📄 issue_tracker_template.md** - Track all bugs, balance issues, and improvements
- Categorized issue logging
- Severity ratings
- Proposed fixes
- Status tracking
- Central hub for all problems found

---

### Version Control

**📄 CHANGELOG.md** - Document all changes between versions
- Version history
- What changed and why
- Migration notes
- Links to issues resolved

---

## 🚀 How to Use This Folder

### If You're Starting Your First Playtest

1. **Read**: `quick_start_guide.md`
2. **Choose**: Digital, physical, or solo approach
3. **Prepare**: Cards and rulebook
4. **Print**: `playtest_feedback_form.md` and `session_log_template.md`
5. **Play**: Run your first session!
6. **Document**: Fill in session log and collect feedback
7. **Track**: Log issues in `issue_tracker_template.md`

### If You're Planning a Testing Campaign

1. **Read**: `implementation_plan.md` in full
2. **Decide**: Which testing phases to pursue
3. **Schedule**: Multiple sessions with different groups
4. **Prepare**: All templates and tools
5. **Execute**: Follow the structured testing protocol
6. **Iterate**: Make changes and test again

### If You're Making Changes to the Game

1. **Review**: Issues in issue tracker
2. **Decide**: What to change
3. **Update**: Rules and/or cards in main folder
4. **Document**: Changes in `CHANGELOG.md`
5. **Version**: Increment version number
6. **Test**: Validate changes with new playtest

---

## 📊 Workflow Overview

```
┌─────────────────┐
│   Playtest      │
│   Session       │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Collect Data   │
│  - Session Log  │
│  - Feedback     │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Log Issues     │
│  - Issue        │
│    Tracker      │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Analyze &      │
│  Decide Changes │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Update Game    │
│  - Rules        │
│  - Cards        │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Document in    │
│  CHANGELOG      │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Playtest       │
│  Again          │
└─────────────────┘
```

---

## 🎯 Key Files for Different Roles

### If You're the Designer/Developer
**Primary files**:
- `implementation_plan.md` - Your strategic guide
- `issue_tracker_template.md` - Your bug database
- `CHANGELOG.md` - Your version history

### If You're Running Playtests
**Primary files**:
- `quick_start_guide.md` - Setup instructions
- `session_log_template.md` - Document each session
- `playtest_feedback_form.md` - Collect player input

### If You're a Playtester
**Primary files**:
- `playtest_feedback_form.md` - Share your experience
- Rules folder (in parent directory) - Game rules

---

## 📋 Checklist: Complete Playtest Session

Before session:
- [ ] Choose which version to test (check CHANGELOG)
- [ ] Prepare cards (digital or physical)
- [ ] Print session log template
- [ ] Print feedback forms (one per player)
- [ ] Review what you're testing this session
- [ ] Recruit 2-4 players

During session:
- [ ] Record start time
- [ ] Explain rules
- [ ] Observe and take notes
- [ ] Track game data (scores, cards, timing)
- [ ] Note all confusion points
- [ ] Don't over-intervene

After session:
- [ ] Complete session log
- [ ] Collect all feedback forms
- [ ] Log issues in issue tracker
- [ ] Thank players
- [ ] Review notes same day (while fresh)

After analysis:
- [ ] Identify patterns across sessions
- [ ] Prioritize issues
- [ ] Propose changes
- [ ] Update cards/rules
- [ ] Document in CHANGELOG
- [ ] Version bump
- [ ] Schedule next test

---

## 🔢 Version Tracking

Current version: **v1.0** (Initial complete version)

See `CHANGELOG.md` for:
- Version history
- What changed between versions
- Why changes were made
- How to migrate from older versions

---

## 💡 Tips for Effective Playtesting

### Do:
✅ Test early and often
✅ Document everything (even small observations)
✅ Test with target audience (PhD students)
✅ Ask open-ended questions
✅ Observe silently during play
✅ Change one thing at a time
✅ Re-test after changes
✅ Thank your playtesters!

### Don't:
❌ Test too late (after everything is "perfect")
❌ Rely on memory (write it down!)
❌ Only test with friends who'll be "nice"
❌ Lead players to answers
❌ Intervene constantly during play
❌ Change everything at once
❌ Assume fixes work without testing

---

## 📈 Success Metrics

Track these across playtests:

**Quantitative**:
- Game duration (target: 45-60 min)
- Score ranges (target: 20-40 points)
- Score gaps (target: 5-15 points)
- Rules questions per session (target: decreasing)
- Enjoyment rating (target: 4+/5)

**Qualitative**:
- Player engagement (high/medium/low)
- Strategic depth (rich/adequate/shallow)
- Educational value (high/medium/low)
- Recommendation likelihood (would/might/wouldn't)

**Goals**:
- Session-over-session improvement
- Converge toward stability (fewer changes needed)
- Consistently positive feedback
- Clear educational outcomes

---

## 🗂️ File Organization Tips

### Keep It Organized:

```
playtesting/
├── README.md (this file)
├── implementation_plan.md
├── quick_start_guide.md
├── playtest_feedback_form.md
├── session_log_template.md
├── issue_tracker_template.md
├── CHANGELOG.md
│
├── sessions/ (create this)
│   ├── session_001.md
│   ├── session_002.md
│   └── ...
│
├── feedback/ (create this)
│   ├── session_001_player1.md
│   ├── session_001_player2.md
│   └── ...
│
└── versions/ (create this)
    ├── v1.0/
    ├── v1.1/
    └── ...
```

### Naming Conventions:
- Session logs: `session_XXX.md`
- Feedback forms: `session_XXX_playerY.md`
- Issue IDs: `#XXX` (three digits)
- Versions: `vX.Y` or `vX.Y.Z`

---

## ❓ FAQ

**Q: How many playtests do I need?**
A: Minimum 10 sessions. Stop when no new issues emerge and feedback is consistently excellent.

**Q: Should I test digitally or physically first?**
A: Start digital for faster iteration, then switch to physical to test UX.

**Q: What if I can't get 4 players?**
A: 2-3 players works fine for early testing. Test 4-player later.

**Q: How do I know when the game is "done"?**
A: When 3+ sessions in a row produce no critical/high issues and players enthusiastically recommend.

**Q: What if playtesting reveals major problems?**
A: That's the point! Better to find and fix now than after printing 1000 copies.

**Q: How much should I change between tests?**
A: Start with top 3 issues. Don't change everything at once or you won't know what worked.

---

## 🎲 Ready to Playtest?

1. Start with `quick_start_guide.md`
2. Run your first session this week
3. Document what you learn
4. Iterate and improve
5. Make an amazing game!

**Good luck!** 🚀

---

## 📝 Quick Links

- **Main game folder**: `../` (parent directory)
- **Rulebook**: `../rules_v1.md`
- **Cards**: `../Methodology_Match_cards_02.csv`
- **Project context**: `../.claude/methodology-match-project.md`
- **Card audit**: `../card_audit_report.md`

---

*Last updated: 2025-11-06*
*Current version: v1.0*
