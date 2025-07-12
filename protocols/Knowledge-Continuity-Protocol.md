# SPARK Knowledge Continuity Protocol

## When Key People Leave: Preserving Velocity Through Transitions

### The Bus Factor Problem

**Bus Factor**: Number of people who could get hit by a bus before the project dies.
**Startup Reality**: Bus factor is often 1-2 people for critical systems.

### Prevention: Daily Knowledge Distribution

#### Modified Work Item Format
```
┌─────────────────────────────────┐
│ TITLE: User Authentication API  │
│ WHY: KR2 - Security compliance  │
│ WHO: @alice (Lead: @bob backup) │
│                                 │
│ KNOWLEDGE LEVEL:                │
│ • Domain: Auth systems          │
│ • Technical: JWT, OAuth         │
│ • Business: GDPR compliance     │
│                                 │
│ BACKUP TRAINED: @bob (partial)  │
│ DOCS: /docs/auth-system.md      │
│ BUS FACTOR: 1 ⚠️               │
└─────────────────────────────────┘
```

#### Knowledge Distribution Rules
1. **No single-owner items** - Every work item has a backup person
2. **Pair programming encouraged** - Especially for complex items
3. **Documentation required** - Before moving to "Done"
4. **Knowledge audits** - Weekly check during retros

### Crisis Response: The 14-Day Handoff Protocol

#### Day 1-3: Emergency Triage (Departing Developer + Team)

**Hour 1: Immediate Assessment**
```
CRITICAL KNOWLEDGE AUDIT:
□ What's in their current WIP?
□ What only they understand?
□ What will break if they leave today?
□ Who can pick up each piece?
```

**Day 1-2: Knowledge Download**
```
KNOWLEDGE TRANSFER SESSIONS:
Day 1 AM: System architecture overview (2 hrs)
Day 1 PM: Current WIP walkthrough (2 hrs)
Day 2 AM: Critical system deep-dive (2 hrs)
Day 2 PM: Gotchas and debugging tips (2 hrs)
```

**Day 3: Work Redistribution**
- Reassign current WIP to backup developers
- Break large items into smaller, manageable pieces
- Update board with new ownership

#### Day 4-14: Structured Knowledge Transfer

**Modified SPARK Week During Handoff:**
- **Monday**: Handoff check-in (30 min) + normal check-in (15 min)
- **Wednesday**: Technical blockers focus (30 min) + normal blockers (15 min)
- **Friday**: Knowledge transfer retro (60 min) + normal retro (45 min)

**Daily Knowledge Sessions (60 min):**
- **Week 1**: Core systems walkthroughs
- **Week 2**: Edge cases, debugging, operational knowledge

#### The Handoff Board

```
┌─────────────┬─────────────┬──────────────┬────────────┬──────────┐
│  BACKLOG    │IN PROGRESS  │   REVIEW     │    DONE    │ HANDOFF  │
│             │   (Max: 1)  │              │            │ QUEUE    │
├─────────────┼─────────────┼──────────────┼────────────┼──────────┤
│ New Work    │ Current     │ Ready for    │ Shipped    │ Alice's  │
│ (Post-      │ Sprint      │ shipping     │ features   │ WIP      │
│ handoff)    │             │              │            │          │
│             │             │              │            │ □ Auth   │
│ Feature Y   │ Bug Fix #3  │ Feature Z    │ Feature A  │   API    │
│ @bob        │ @carol      │ @david       │ ✓ Done     │ @alice→  │
│ KR1: +15%   │ (alice's    │ @eric        │            │ @bob     │
│             │ knowledge)  │              │            │          │
│             │             │              │            │ □ Payment│
│             │             │              │            │   Flow   │
│             │             │              │            │ @alice→  │
│             │             │              │            │ @carol   │
└─────────────┴─────────────┴──────────────┴────────────┴──────────┘
```

### Knowledge Preservation Techniques

#### 1. The Learning Log
**Departing developer maintains daily log:**
```
DAY 8 KNOWLEDGE TRANSFER LOG:
Taught @bob about:
- OAuth token refresh logic in auth.service.ts:245
- Why we retry 3 times (API rate limits)
- Debug command: npm run debug:auth

@bob understands: 80%
Still needs: Error handling edge cases
Next session: Payment integration patterns
```

#### 2. Video Documentation
- Record screen while explaining complex systems
- Create "day in the life" videos showing common tasks
- Capture debugging sessions for common issues

#### 3. Code Archaeology
**Systematic code review sessions:**
- Walk through git history for critical files
- Explain design decisions and trade-offs
- Document "why" not just "what"

#### 4. Shadow Programming
- Departing developer works normally
- Backup developer shadows and asks questions
- Gradually reverse roles over time

### Long-term Bus Factor Mitigation

#### Knowledge Distribution Metrics
```
TEAM KNOWLEDGE HEALTH:
Bus Factor by System:
• Authentication: 2 people ✓
• Payment Processing: 1 person ⚠️ 
• Data Pipeline: 3 people ✓
• Frontend: 2 people ✓

Action: Cross-train @david on payments
```

#### Continuous Knowledge Sharing

**Weekly Practices:**
- **Mini Tech Talks** (15 min during Friday retro)
  - Each person teaches one thing they learned
  - Rotate who explains complex systems

- **Code Review Culture**
  - Reviews focus on knowledge transfer, not just bugs
  - Require explanatory comments for complex logic

- **Pair Programming Rotation**
  - Mandatory pairing for bus factor 1 items
  - Rotate pairs to spread knowledge

#### Documentation Standards

**Required Documentation:**
- **System Overview**: High-level architecture
- **Runbooks**: How to debug common issues  
- **Decision Log**: Why we chose X over Y
- **Setup Guide**: New developer onboarding

**Documentation Quality Gate:**
- Can a new team member understand it?
- Does it include the "why" not just "what"?
- Is it maintained as code changes?

### Emergency Protocols

#### If Key Person Leaves Immediately (No handoff time)

**Hour 1: Damage Assessment**
```
IMMEDIATE ACTIONS:
□ Lock their accounts (security)
□ Export their work (git history, documents)
□ Identify critical systems they owned
□ Find backup contacts (vendors, customers)
```

**Day 1: Emergency Response Team**
- Assign emergency owners to critical systems
- Focus on keeping lights on, not new features
- Document what we discover as we go

**Week 1: Recovery Plan**
- Hire emergency contractor/consultant
- Intensive reverse engineering of critical systems
- Reduce scope to essential features only

### Success Metrics

#### Handoff Quality Indicators:
- **Knowledge Transfer Score**: Backup person rates understanding 1-10
- **Velocity Recovery**: Team back to 80% velocity within 2 weeks
- **System Stability**: No increase in critical bugs post-departure
- **Documentation Coverage**: All critical systems documented

#### Bus Factor Health:
- **Target**: No system with bus factor < 2
- **Measurement**: Weekly knowledge audit
- **Action**: Immediate cross-training for bus factor 1 items

### Integration with Standard SPARK

#### Prevention (Always Active):
- Modified work item format includes bus factor
- Weekly knowledge distribution check during retros
- Pair programming for complex items
- Documentation requirements for "Done"

#### Response (When Someone Leaves):
- Activate 14-day handoff protocol
- Modified board with handoff queue
- Extended retros focus on knowledge transfer
- Temporary scope reduction to focus on continuity

#### Recovery (Post-Departure):
- Return to normal SPARK operations
- Increased focus on knowledge distribution
- Higher documentation standards
- Regular bus factor audits

### The Knowledge Continuity Mindset

**Traditional Thinking**: "Alice knows that system, so Alice owns it"
**SPARK Thinking**: "Alice built that system, now Alice teaches it"

The goal isn't to make everyone redundant—it's to make everyone valuable and the team resilient.