# SPARK Customer Emergency Protocol

## When Customers Are Down: Balancing Fire-Fighting with Forward Progress

### The Customer Emergency Paradox

**The Problem**: Customer emergencies feel urgent but can destroy planned velocity
**The Solution**: Structured triage that balances retention with growth

### Emergency Classification System

#### Severity Levels

**CRITICAL (P0) - All hands**
- Customer business is stopped
- Revenue at immediate risk
- Security breach
- **Response**: < 1 hour
- **Resolution Target**: < 4 hours
- **Team Impact**: Stop all other work

**HIGH (P1) - Dedicated person**
- Customer significantly impacted
- Workaround exists but painful
- **Response**: < 4 hours
- **Resolution Target**: < 24 hours  
- **Team Impact**: 1 person dedicated

**MEDIUM (P2) - Normal flow**
- Customer inconvenienced
- Clear workaround available
- **Response**: < 24 hours
- **Resolution Target**: < 1 week
- **Team Impact**: Goes in normal backlog

**LOW (P3) - Planned work**
- Feature request disguised as "emergency"
- No current business impact
- **Response**: Acknowledge within 48 hours
- **Resolution Target**: Next quarter
- **Team Impact**: Normal planning process

### The Emergency Board Layout

```
┌─────────────┬─────────────┬──────────────┬────────────┬──────────┐
│  BACKLOG    │IN PROGRESS  │   REVIEW     │    DONE    │EMERGENCY │
│  (Planned)  │   (Max: 1)  │              │            │  QUEUE   │
├─────────────┼─────────────┼──────────────┼────────────┼──────────┤
│ Feature A   │ Feature B   │ Bug Fix #2   │ Feature Z  │ P0: DB   │
│ KR1: +10%   │ @alice      │ @bob         │ Shipped ✓  │ Down     │
│             │ Planned     │              │            │ @charlie │
│ Feature C   │             │              │            │ 2hr ETA  │
│ KR2: +5%    │             │              │            │          │
│             │             │              │            │ P1: API  │
│             │             │              │            │ Slow     │
│             │             │              │            │ @david   │
│             │             │              │            │ 1day ETA │
└─────────────┴─────────────┴──────────────┴────────────┴──────────┘
```

### Emergency Response Protocol

#### Stage 1: Triage (< 15 minutes)

**Emergency Triage Checklist:**
```
CUSTOMER IMPACT ASSESSMENT:
□ Which customer(s) affected?
□ Revenue impact ($ per hour down)?
□ Business process impact (critical/major/minor)?
□ Workaround available? (none/painful/easy)
□ External reputation risk? (high/medium/low)

TECHNICAL ASSESSMENT:
□ System affected (core/secondary/feature)?
□ Other customers affected? (yes/no/unknown)
□ Quick fix possible? (yes/no/needs investigation)
□ Rollback available? (yes/no/risky)

SEVERITY CLASSIFICATION: P0/P1/P2/P3
```

#### Stage 2: Response (Immediate)

**P0 Response (All Hands):**
```
IMMEDIATE ACTIONS (First 30 minutes):
□ War room activated (Slack channel/video call)
□ Customer communication sent (we're aware, investigating)
□ All WIP paused, team focuses on emergency
□ Incident commander assigned
□ Initial diagnosis started

COMMUNICATION TIMELINE:
0 min: Internal war room
15 min: Customer acknowledgment
30 min: Initial assessment to customer
60 min: Progress update to customer
Every hour: Progress updates until resolved
```

**P1 Response (Dedicated Person):**
```
IMMEDIATE ACTIONS (First 4 hours):
□ Senior person assigned full-time
□ Customer contacted with timeline
□ Work item created in Emergency Queue
□ Rest of team continues planned work
□ Regular updates to customer/stakeholders
```

#### Stage 3: Resolution & Learning

**Post-Emergency Retrospective:**
```
WITHIN 24 HOURS OF RESOLUTION:
□ Root cause analysis completed
□ Prevention plan created
□ Customer satisfaction confirmed
□ Team stress/impact assessment
□ Process improvement identified
```

### Interrupt Management Strategy

#### The 20% Emergency Buffer Rule
- Reserve 20% of team capacity for emergencies
- If no emergencies, use for technical debt
- Track actual emergency load monthly
- Adjust buffer based on data

#### Emergency Work vs Planned Work Balance
```
MONTHLY EMERGENCY TRACKING:
Emergency Work: 15% (target: < 20%)
Planned Work: 85% (target: > 80%)

If Emergency Work > 20%:
□ Improve system stability (more testing/monitoring)
□ Better customer onboarding (prevent misuse)
□ Stricter emergency classification
□ Consider dedicated support person
```

### Customer Communication Framework

#### Emergency Communication Templates

**P0 Acknowledgment (< 15 min):**
```
Subject: [URGENT] We're investigating your reported issue

Hi [Customer],

We've received your report about [issue] and have immediately 
escalated this to our engineering team. We understand this is 
impacting your business operations.

Current status: Investigation in progress
Next update: Within 1 hour
Assigned engineer: [Name]

We'll keep you updated every hour until resolved.

[Your Name]
Emergency Response Team
```

**P1 Response (< 4 hours):**
```
Subject: Update on reported issue - [Brief description]

Hi [Customer],

Thank you for reporting [issue]. We've classified this as high 
priority and assigned [Engineer] to work on it full-time.

Initial assessment: [Brief technical summary]
Estimated resolution: [Timeframe]
Workaround available: [If any]

We'll update you every 4 hours until resolved.
```

#### Post-Resolution Follow-up
```
Subject: Resolution confirmed + Prevention plan

Hi [Customer],

The issue has been resolved. Here's what happened and how 
we're preventing it in the future:

Root cause: [Simple explanation]
Fix applied: [What we did]
Prevention: [What we're building to prevent recurrence]

We're sorry for the disruption and appreciate your patience.
Please confirm everything is working normally.
```

### OKR Integration During Emergencies

#### Emergency Impact on OKRs

**Customer Retention vs Growth Trade-off:**
```
CURRENT OKRS:
O1: Delight existing customers
├─ KR1: Customer satisfaction > 95%
├─ KR2: Support resolution time < 4 hours
└─ KR3: Zero critical bugs per month

O2: Accelerate new customer acquisition  
├─ KR1: 50 new signups per month
├─ KR2: 3 new features shipped
└─ KR3: Conversion rate > 15%

EMERGENCY DECISION MATRIX:
Emergency threatens KR2 (support time) → Drop work on O2/KR2 (new features)
Customer at risk → All hands protect O1/KR1 (satisfaction)
```

#### Emergency OKR Adjustments
- **P0 Emergencies**: Temporarily suspend growth OKRs
- **P1 Emergencies**: Reduce growth OKR targets by 20%
- **P2/P3**: Handle within normal flow, no OKR impact

### Preventing Emergency Spiral

#### Early Warning System
```
CUSTOMER HEALTH DASHBOARD:
Red Flags (Predict P0/P1 emergencies):
□ Support ticket volume increased 50%+
□ Same customer 3+ tickets this week
□ Error rates trending up for 48+ hours
□ Customer satisfaction scores dropping

Green Flags (System health):
□ Error rates stable or declining
□ Support tickets decreasing
□ Customer satisfaction scores improving
□ Proactive monitoring alerts working
```

#### System Reliability Investment
- **Target**: < 10% of capacity on emergencies
- **Strategy**: Invest saved emergency time in stability
- **Metrics**: Mean time to recovery, error rates, monitoring coverage

### Success Metrics

#### Emergency Response Quality:
- **Response Time**: Meeting SLA targets
- **Resolution Time**: Trending down over time
- **Customer Satisfaction**: Post-emergency scores
- **Repeat Issues**: < 10% of emergencies are repeats

#### Team Health During Emergencies:
- **Stress Level**: 1-10 rating during/after emergencies
- **Planned Work Impact**: % of planned features delayed
- **Burnout Prevention**: Sustainable emergency response pace

### Integration with Standard SPARK

#### Prevention (Daily Practice):
- Monitor customer health metrics during check-ins
- Include "early warning signals" in Friday retros
- Build stability features based on emergency patterns
- Customer feedback loop in weekly planning

#### Response (During Emergency):
- Emergency Queue column on board
- Modified check-ins include emergency status
- Escalation path through Product Owner
- Clear communication responsibilities

#### Recovery (Post-Emergency):
- Emergency retrospective replaces standard retro
- Adjustment of upcoming OKRs if needed
- Investment in prevention based on root cause
- Customer relationship repair if necessary

### The Emergency Mindset Shift

**Old Thinking**: "All customer issues are emergencies"
**SPARK Thinking**: "Customer success is the goal, not customer demands"

**Old Thinking**: "Drop everything for any customer complaint"  
**SPARK Thinking**: "Triage objectively, respond proportionally"

**Old Thinking**: "We're bad at planning because emergencies happen"
**SPARK Thinking**: "We're getting better at building reliable systems"