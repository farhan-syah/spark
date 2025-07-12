# SPARK Feature Focus Protocol

## Escaping the Feature Factory: Strategic Focus Over Feature Volume

### The Feature Factory Problem

**Symptoms:**
- 30+ items in backlog, all "critical"
- Sales promising features that don't exist
- Nothing ships completely
- Team always behind, stakeholders always frustrated

**Root Cause:** No mechanism for saying no

### The Feature Evaluation Framework

#### The SPARK Feature Filter

Every feature request must pass through:

```
FEATURE REQUEST: [Name]
REQUESTER: [Sales/Customer/Internal]
BUSINESS CASE: [Why this matters]

SPARK FILTER:
□ OKR Alignment: Which KR does this serve? [Specific KR]
□ Customer Count: How many customers want this? [Number]
□ Revenue Impact: What's the $ impact? [Specific amount]
□ Effort Estimate: How big is this? [S/M/L/XL]
□ Strategic Value: Build once, sell many? [Yes/No]

DECISION: ACCEPT / REJECT / DEFER
```

#### The Three Buckets Strategy

**CORE (60% of capacity)**
- Features that serve multiple customers
- Directly tied to growth OKRs
- Can be sold to new prospects
- Example: Better search, mobile app, API

**CUSTOM (20% of capacity)**
- One-off features for big customers
- High revenue impact (>$50k ARR)
- Can be delivered without derailing core
- Example: Custom integrations, specific workflows

**EXPERIMENTS (20% of capacity)**
- New feature validation
- Small bets on future direction
- Quick to build, test, and learn
- Example: New UI concepts, beta features

### Sales-Engineering Alignment System

#### The Deal Feature Checklist

**Before Sales Can Promise Features:**
```
DEAL FEATURE EVALUATION:
□ Feature exists in roadmap? → Promise with timeline
□ Feature doesn't exist but fits CORE? → Add to backlog, give estimate
□ Feature is CUSTOM and deal >$50k? → Engineering consultation required
□ Feature is CUSTOM and deal <$50k? → Suggest workaround/alternative
□ Feature conflicts with strategy? → Sales cannot promise
```

#### Weekly Sales-Engineering Sync (30 min)

**Every Wednesday:**
- Review deals in pipeline requiring custom features
- Engineering provides capacity reality check
- Sales gets roadmap updates
- Align on what can/cannot be promised

**Agenda:**
```
1. Deal Pipeline Review (15 min)
   - Features requested in active deals
   - Engineering effort estimates
   - Capacity availability

2. Roadmap Updates (10 min)
   - What's shipping this week/month
   - What sales can start promising

3. Feature Request Triage (5 min)
   - New requests since last sync
   - Quick accept/reject/defer decisions
```

### The Feature Focus Board

```
┌─────────────┬─────────────┬──────────────┬────────────┬──────────┐
│  BACKLOG    │IN PROGRESS  │   REVIEW     │    DONE    │ PARKING  │
│             │   (Max: 1)  │              │            │   LOT    │
├─────────────┼─────────────┼──────────────┼────────────┼──────────┤
│ CORE:       │ Search V2   │ Mobile App   │ API v2     │ Custom   │
│ Search V2   │ @alice      │ @bob         │ ✓ Shipped  │ Features │
│ KR1: +20%   │ Week 2/3    │              │            │ (Future) │
│ Multi-cust  │             │              │            │          │
│             │             │              │            │ Widget X │
│ CUSTOM:     │             │              │            │ (BigCorp)│
│ BigCorp Intg│             │              │            │ $100k    │
│ $100k deal  │             │              │            │ Q2 2024  │
│ KR2: +$100k │             │              │            │          │
│             │             │              │            │ Feature Y│
│ EXPERIMENT: │             │              │            │ (Maybe)  │
│ AI Summary  │             │              │            │ $5k deal │
│ KR1: +5%    │             │              │            │ REJECT   │
│ Quick test  │             │              │            │          │
└─────────────┴─────────────┴──────────────┴────────────┴──────────┘
```

### Stakeholder Expectation Management

#### The "No, But..." Framework

**Instead of:** "We can't build that"
**Say:** "We can't build that this quarter, but here's what we can do..."

**Template Responses:**

**For Low-Value Requests:**
```
"This feature would serve 1 customer and take 3 weeks. Instead, 
we could build [similar feature] that serves 10 customers in 
the same time. Would that work?"
```

**For High-Effort Requests:**
```
"This would take 2 months and delay 3 core features that 
benefit all customers. We could build a simpler version 
in 2 weeks that gives you 80% of the value. Interested?"
```

**For Off-Strategy Requests:**
```
"This takes us away from our core strength in [area]. 
There's a great tool called [X] that does this well. 
Can we integrate with them instead?"
```

#### The Roadmap Communication Strategy

**Monthly Stakeholder Update:**
```
FEATURE ROADMAP UPDATE - MARCH

SHIPPING THIS MONTH:
✓ Search improvements (multi-customer request)
✓ Mobile app beta (growth OKR)

COMING NEXT MONTH:
→ API v2 (enables integrations)
→ Custom BigCorp workflow ($100k deal)

IN PIPELINE (Q2):
→ Advanced analytics
→ Team collaboration features

NOT HAPPENING (and why):
✗ Custom reporting for SmallCorp (1 customer, 6 weeks effort)
✗ Integration with LegacyTool (conflicts with API strategy)
✗ Advanced AI features (need core platform first)

Questions? Hit reply or join Friday's roadmap session.
```

### The Feature Debt Problem

#### Preventing Half-Built Features

**Definition of Done for Features:**
```
FEATURE COMPLETE CHECKLIST:
□ Core functionality works
□ Edge cases handled
□ Error states designed
□ Help documentation written
□ Customer success team trained
□ Usage metrics instrumented
□ Can be sold to new customers

Not done until ALL boxes checked.
```

#### Feature Completion Tracking

```
CURRENT FEATURE STATUS:
Search V2: 90% complete (needs help docs)
Mobile App: 60% complete (testing phase)
BigCorp Integration: 30% complete (just started)

COMPLETION VELOCITY:
Last month: 2 features shipped complete
This month: 1 feature shipped, 2 in progress
Trend: Focus improving ✓
```

### Saying No Gracefully

#### The Customer Response Framework

**When Customer Requests One-Off Feature:**
```
"Thank you for the feedback! This feature would benefit you 
specifically, but we're focused on features that help all 
our customers. Here are three alternatives:

1. [Workaround using existing features]
2. [Similar feature that serves many customers, timeline]
3. [Integration with tool that does this well]

Our roadmap focuses on [current quarter OKRs]. Would any 
of these alternatives work for your use case?"
```

**When Sales Pushes Back:**
```
"I understand this could close the deal. Let's look at the 
numbers:

Building this custom feature:
- Takes 4 weeks
- Serves 1 customer  
- Delays 2 core features
- Doesn't help us land other prospects

Building the core feature instead:
- Takes 4 weeks
- Serves 20+ customers
- Advances our growth OKR
- Helps close 3 other deals

Can we position the core feature to this prospect instead?"
```

### Metrics That Matter

#### Feature Factory Health Indicators

**Good Signs:**
- **Feature Completion Rate**: >90% of started features ship complete
- **Multi-Customer Impact**: >80% of features serve multiple customers
- **Sales-Engineering Alignment**: <5 promises made that can't be delivered
- **Roadmap Predictability**: Stakeholders can rely on timeline estimates

**Warning Signs:**
- **WIP Explosion**: >2x as many features in progress as team size
- **Custom Feature Creep**: >30% of capacity on one-off features  
- **Stakeholder Frustration**: Regular complaints about delayed features
- **Quality Debt**: Features shipping incomplete, requiring rework

#### The Focus Score

```
MONTHLY FOCUS SCORE:
Core Features: 6 (target: 60% capacity)
Custom Features: 2 (target: 20% capacity)  
Experiments: 2 (target: 20% capacity)

FOCUS SCORE: 8.5/10 ✓ (Well balanced)

Action: Continue current approach
```

### Emergency Feature Override

#### When to Break the Rules

**Criteria for Emergency Custom Feature:**
- Customer threatening to leave (>$100k ARR)
- Competitive threat (losing deals to this missing feature)
- Regulatory requirement (must-have for compliance)
- Strategic partnership requirement

**Emergency Protocol:**
1. CEO/CPO approval required
2. Explicit OKR adjustment
3. Clear timeline for technical debt paydown
4. Communication to all stakeholders about priority shift

### Integration with Standard SPARK

#### Daily Practice:
- Feature requests tagged with bucket (Core/Custom/Experiment)
- OKR alignment required for backlog entry
- Sales-engineering sync every Wednesday
- Feature completion tracking in Friday retros

#### Weekly Planning:
- Capacity allocation review (60/20/20 split)
- New feature request triage
- Stakeholder expectation updates
- Focus score calculation

#### Monthly Strategy:
- Roadmap communication to stakeholders
- Feature factory health assessment
- Sales-engineering process improvement
- Custom feature ROI analysis

### The Feature Focus Mindset

**Old Thinking**: "Say yes to everything, figure it out later"
**SPARK Thinking**: "Say no to everything except what serves our strategy"

**Old Thinking**: "More features = more value"
**SPARK Thinking**: "Complete features that many customers use = more value"

**Old Thinking**: "Sales knows what customers want"
**SPARK Thinking**: "Engineering and sales together decide what's possible and valuable"