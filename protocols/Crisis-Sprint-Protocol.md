# SPARK Crisis Sprint Protocol

## When Everything Must Ship: High-Stakes Deadline Management

### The Crisis Sprint Framework

#### Day 1: Stakeholder Alignment Summit (4 hours)

**Morning (2 hours) - Reality Check:**
1. **Current State Assessment** (30 min)
   - What's actually working today?
   - What's broken but fixable?
   - What's impossible in timeframe?

2. **Demo Success Definition** (60 min)
   - What specific investor objections must be overcome?
   - What 3 moments in demo must be flawless?
   - What can be "smoke and mirrors" vs real?

3. **Resource Audit** (30 min)
   - Available development hours
   - Current velocity data
   - External dependencies

**Afternoon (2 hours) - Crisis OKRs:**
4. **Crisis OKR Creation** (90 min)
   ```
   CRISIS OBJECTIVE: Secure Series A funding
   
   KR1: Demo converts 2+ investors to term sheet
   KR2: Zero critical bugs during demo
   KR3: Core value prop is undeniable in 10 minutes
   ```

5. **Feature Triage** (30 min)
   - **MUST HAVE**: Demo fails without this
   - **SHOULD HAVE**: Makes demo stronger
   - **COULD HAVE**: Nice but not essential
   - **WON'T HAVE**: Explicitly cut for now

#### Crisis Board Layout

```
┌─────────────┬─────────────┬──────────────┬────────────┬──────────┐
│   CRISIS    │ IN PROGRESS │    REVIEW    │    DONE    │   CUT    │
│   BACKLOG   │   (Max: 1)  │   (24hr SLA) │            │ (Future) │
├─────────────┼─────────────┼──────────────┼────────────┼──────────┤
│ MUST: Core  │ Bug Fix #1  │ Smoke Test   │ Login Fix  │ Feature D│
│ Feature Fix │ @alice      │ @pending     │ ✓ Demo     │ (Post-   │
│ Demo Impact │ 3 days est  │              │ Ready      │ funding) │
│             │             │              │            │          │
│ SHOULD: UI  │             │              │ Data Viz   │ Feature E│
│ Polish      │             │              │ ✓ Demo     │ (Nice to │
│ Demo Impact │             │              │ Ready      │ have)    │
└─────────────┴─────────────┴──────────────┴────────────┴──────────┘
```

### Crisis-Specific Rules

#### Modified SPARK Principles:
1. **Demo-Driven Development**: Everything serves the demo narrative
2. **Technical Debt is OK**: If it works for demo, ship it
3. **Parallel Demo Track**: One person owns demo flow while team ships features
4. **Daily Demo Runs**: Test full demo daily, fix what breaks

#### Crisis Week Schedule:
**Monday**: Crisis check-in + demo run (30 min)
**Wednesday**: Blocker escalation + demo run (30 min)  
**Friday**: Demo rehearsal + quick retro (60 min)
**Daily**: End-of-day demo smoke test (15 min)

### Stakeholder Management

#### The Crisis Council
**Who**: CEO, Head of Product, Lead Engineer, Demo Owner
**When**: Daily 15-min alignment calls
**Purpose**: 
- Resolve conflicts immediately
- Make cut/keep decisions
- Adjust timeline reality

#### Decision Matrix
| Decision Type | Owner | Consultation |
|--------------|-------|--------------|
| Feature cuts | CEO | Engineering estimate |
| Technical shortcuts | Lead Engineer | Demo impact |
| Demo narrative | Demo Owner | Customer feedback |
| Resource allocation | Head of Product | Team capacity |

### Quality Levels

#### Demo Quality vs Production Quality
```
PRODUCTION QUALITY:
- Error handling for all edge cases
- Performance at scale
- Security hardened
- Full test coverage
- Documentation complete

DEMO QUALITY:
- Happy path works flawlessly
- Handles expected demo data
- Looks polished on surface
- Core value prop is clear
- Recovery plan for demo failures
```

#### The Demo Quality Checklist
- [ ] Works with demo dataset
- [ ] Visually impressive
- [ ] Tells clear story
- [ ] 3 fallback plans if it breaks
- [ ] Can be reset quickly between demos

### Risk Management

#### Demo Failure Protocol
1. **Plan A**: Everything works perfectly
2. **Plan B**: Minor glitch, smooth recovery
3. **Plan C**: Major failure, pivot to different feature
4. **Plan D**: Complete failure, focus on vision/team story

#### Technical Debt Tracking
```
DEMO DEBT LOG:
- Feature X: Hardcoded for demo data only
- API Y: No error handling, fails on edge cases  
- UI Z: Only tested in Chrome, demo browser
- Database: Sample data only, doesn't scale

POST-DEMO CLEANUP PLAN:
Week 1: Address hardcoding
Week 2: Add error handling
Week 3: Cross-browser testing
Week 4: Production data migration
```

### Success Metrics

#### Leading Indicators (Weekly):
- Demo run success rate
- Feature completion %
- Bug count trend
- Team stress level (1-10)

#### Lagging Indicators (Post-demo):
- Investor interest level
- Term sheet conversion
- Technical debt created
- Team burnout level

### Crisis Anti-Patterns & Solutions

| Anti-Pattern | Why It Fails | SPARK Solution |
|-------------|--------------|----------------|
| "Everything is critical" | Nothing gets done well | MUST/SHOULD/COULD triage |
| "More people = faster" | Brooks' Law applies | Keep team size constant |
| "Work weekends" | Burnout + more bugs | Sustainable pace + scope cut |
| "Perfect demo script" | Real questions throw you off | Practice 10+ variations |
| "Hide technical debt" | It compounds fast | Track it explicitly |

### Integration with Standard SPARK

**When Crisis Mode Activates:**
- High-stakes deadline < 8 weeks away
- Success criteria are existential (funding, major customer, etc.)
- Normal velocity won't meet requirements

**When Crisis Mode Ends:**
- Deadline passes (success or failure)
- Return to normal OKRs
- Technical debt cleanup becomes priority
- Team recovery/retrospective

**Crisis Mode Limits:**
- Maximum 8 weeks duration
- Maximum 2x per year
- Requires explicit team consent
- Must include recovery period

### The Crisis Retrospective

**Immediate (Day after demo):**
- What went right?
- What went wrong?
- Emotional check-in with team

**1 Week Later:**
- Technical debt assessment
- Process improvements
- Recovery timeline

**1 Month Later:**
- Did we make the right trade-offs?
- How can we avoid crisis mode next time?
- What early warning signals did we miss?