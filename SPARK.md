# The SPARK Framework

## A Project Management Framework for High-Velocity Teams

**Version 1.0.0**

---

## What is SPARK?

SPARK (Swift Product Acceleration through Rapid Knowledge) is a lightweight project management framework designed for teams of 1-30 people who need to move fast while maintaining quality. It combines principles from Agile, Lean, and modern product thinking into a simple, teachable system.

### Core Philosophy
> "Sustainable speed beats temporary sprints. Flow beats batch. Outcomes beat outputs."

---

## The Five SPARK Principles

1. **Single-Piece Flow** - Work moves continuously, one item at a time per person
2. **Pull, Don't Push** - Team members pull work when ready
3. **Amplify Learning** - Every week, the team gets smarter
4. **Radically Minimize Waste** - Eliminate non-value-adding activities
5. **Keep It Simple** - The framework must be teachable in one hour

---

## The SPARK System

### 1. Objectives & Key Results (OKRs)

**What:** Quarterly goals that define success
**When:** Set every 3 months
**Who:** Leadership sets company OKRs, teams create aligned OKRs

**Examples:**
```
Early Stage Startup:
Objective: Achieve product-market fit
KR1: 50 customer interviews completed
KR2: 40% weekly active user rate
KR3: 3 customers willing to pay

Growth Stage Startup:
Objective: Scale revenue engine
KR1: $50k Monthly Recurring Revenue
KR2: 20% month-over-month growth
KR3: Customer acquisition cost < $100
```

### 2. The SPARK Board

A simple 4-column visual board:

```
┌─────────────┬──────────────┬──────────────┬─────────────┐
│   BACKLOG   │ IN PROGRESS  │    REVIEW    │    DONE     │
│             │   (Max: 1)   │              │             │
├─────────────┼──────────────┼──────────────┼─────────────┤
│ Feature A   │ Feature B    │ Feature C    │ Feature Z   │
│ KR1: +10%   │ @alice       │ @bob         │ Shipped ✓   │
│             │              │              │             │
│ Feature D   │              │              │ Feature Y   │
│ KR2: +5%    │              │              │ Shipped ✓   │
└─────────────┴──────────────┴──────────────┴─────────────┘
```

**Guidelines:**
- WIP limit of 1 per person (adjustable when justified)
- Items should link to a Key Result
- "Done" means shipped to real users

**Optional:** Teams may add columns (Ready), swimlanes, or visual indicators as needed.

#### Proposal Board

A companion board for team suggestions:

```
┌─────────────┬──────────────┬──────────────┐
│  PROPOSED   │    URGENT    │  REVIEWING   │
├─────────────┼──────────────┼──────────────┤
│ Bug fix #1  │ Server down  │ Feature idea │
│ @alice      │ @bob         │ @team        │
│ KR2 impact │ IMMEDIATE    │ Future OKR   │
└─────────────┴──────────────┴──────────────┘
```

**Flow:**
- Team members add proposals anytime
- Urgent items reviewed immediately by Product Owner
- Regular proposals reviewed during Friday planning
- Approved items move to main backlog

**Guidelines:**
- Include OKR impact in proposal
- Product Owner maintains final backlog control
- Proposals expire after 2 weeks if not addressed

### 3. Work Items

Each work item contains:
- **What:** Clear description of the deliverable
- **Why:** Which Key Result it impacts
- **How:** Acceptance criteria
- **Who:** Single owner (when pulled)

### 4. The SPARK Week

**Monday (15 min)**
- Check-in: Everyone posts their focus for the week
- Format: "This week I'm shipping X to achieve KR Y"

**Wednesday (15 min)**  
- Blockers check: Anyone stuck raises a flag
- Format: "I need help with X" or "All clear"

**Friday (45 min)**
- Retrospective: What did we learn?
- Metrics review: Are we hitting our KRs?
- Proposal review: What should we work on next week?
- Process tune: One thing to try next week

**Total:** < 2 hours/week of meetings

### 5. Roles

**Product Owner**
- Sets OKRs
- Maintains backlog
- Removes blockers

**Team Members**
- Pull work when ready
- Ship to production
- Share learnings
- Propose work items via proposal board

**No other roles required.**

---

## Metrics That Matter

### Flow Metrics
1. **Cycle Time**: How long from start to done?
2. **Throughput**: How many items per week?
3. **Flow Efficiency**: Active time ÷ Total time

### Outcome Metrics  
1. **OKR Progress**: Are we hitting our Key Results?
2. **Customer Impact**: NPS, usage, retention
3. **Team Health**: Sustainable pace, stress levels

---

## Transitioning to SPARK

### From Scrum
Week 1: Keep your sprint, add OKRs
Week 2: Drop sprint planning, pull from backlog
Week 3: Drop daily standup, use async check-ins
Week 4: You're now running SPARK!

### From Kanban
Day 1: Add OKRs to your board
Day 2: Apply WIP limit of 1 (adjustable when justified)
Day 3: Add Friday retrospectives
Done: You're running SPARK!

### From Waterfall
Month 1: Break project into 2-week deliverables
Month 2: Implement the SPARK board
Month 3: Add retrospectives and iterations
Month 4: Full SPARK implementation

---

## Common Patterns & Solutions

### Pattern: Too Many Blockers
**Solution:** Product Owner dedicates 50% time to unblocking

### Pattern: Work Items Too Big
**Solution:** If it takes > 1 week, break it down

### Pattern: Losing Sight of OKRs
**Solution:** Every work item must tag a KR

### Pattern: Review Bottleneck
**Solution:** Implement "Review SLA" - max 24 hours

### Pattern: Knowledge Silos
**Solution:** Friday retros include mini tech talks

---

## Scaling Beyond 10 People

When teams grow beyond 10 people, use a pod structure:

**Pod Organization:**
```
Pod Alpha (5 people):
• OKR: Customer acquisition
• Focus: Growth features
• Lead: Alice

Pod Beta (5 people):  
• OKR: Customer retention
• Focus: Core platform
• Lead: Bob

Cross-Pod Coordination:
• Weekly pod lead sync (30 min)
• Monthly all-hands retro (90 min)
• Shared technical standards
• Inter-pod dependency management
```

---

## Handling Disruptions

SPARK is designed to handle common startup disruptions through structured responses:

### Emergency Response
When critical customer issues arise:
1. Move emergency work to board immediately
2. Someone pulls the emergency item (breaking WIP limit temporarily)
3. Communicate impact to stakeholders
4. Resume normal flow once resolved

### Direction Changes
When strategy pivots:
1. Call emergency retro to reassess OKRs
2. Archive irrelevant backlog items
3. Create new OKRs aligned with new direction
4. Team pulls work from updated backlog

### Knowledge Loss
When key team members leave:
1. Document what they're working on
2. Pair departing person with successor
3. Break down their work into smaller pieces
4. Distribute knowledge across team

### External Dependencies
When third-party services break:
1. Assign someone to vendor relationship
2. Track dependency health weekly
3. Build fallback plans for critical dependencies
4. Consider building internal alternatives for unreliable vendors

---

## FAQ

**Q: What about dependencies?**
A: Use a simple escalation pattern:
- **Level 1 (Team)**: Direct conversation between team members
- **Level 2 (Visible)**: Create a dependency card on boards to track cross-team work  
- **Level 3 (Escalated)**: Product Owner/leader actively manages external blockers with daily updates

Make dependencies visible early and have clear ownership for resolution.

**Q: How do we estimate?**
A: You don't. Break work small enough (1 week maximum) that estimation is unnecessary. This decomposition skill requires practice but is essential for SPARK success.

**Q: What about roadmaps?**
A: OKRs are your roadmap. Trust emergence for specific features.

**Q: Can we keep using release cycles?**
A: Yes. SPARK's small work breakdown makes this easy - work flows continuously but releases are batched. Teams ship when features are ready within the cycle.

**Q: Can this scale?**
A: Yes. Works for 1-10 people as-is. Pod structure handles 10-50 people.

**Q: What tools do we need?**
A: Any board works - Trello, Notion, Linear, sticky notes, whiteboard.

**Q: What skills does our team need?**
A: Work decomposition (breaking tasks into <1 week pieces) and an effective Product Owner who can prioritize, remove blockers, and communicate strategy. These skills develop with practice.

**Q: How do we handle multiple priorities?**
A: OKRs force prioritization. If everything is urgent, nothing is urgent.

**Q: What about technical debt?**
A: Track it like features. Dedicate capacity to debt reduction during retros.

---

## Get Started

### Today
1. Read this guide with your team
2. Identify which transition approach fits your current process
3. Set up a simple 4-column board

### Tomorrow  
1. Define current quarter OKRs with your team
2. Move existing work into SPARK backlog format
3. Apply WIP limit of 1 per person (adjustable when justified)

### This Week
1. Start Monday/Wednesday/Friday ceremonies
2. Begin pulling work instead of assigning it
3. Measure baseline cycle time and throughput

### First Month
1. Tune the process based on what you learn
2. Address common patterns as they emerge
3. Consider pod structure if team >10 people
4. Document what works for your specific context

---

## Advanced Considerations

### For AI-Assisted Development
- Write specifications before AI generates code
- Declare allowed/forbidden dependencies explicitly
- Review AI output for unexpected coupling
- Use progressive enhancement vs. big-bang generation

### For Remote Teams
- Use async communication for check-ins
- Record retro decisions for those who can't attend
- Share board access with entire team
- Over-communicate context and decisions

### For Regulated Industries
- Add compliance review step to board
- Track regulatory requirements like features
- Include compliance criteria in "Done" definition
- Plan buffer time for regulatory approval

### For Customer-Facing Teams
- Include customer impact in work item descriptions
- Track customer satisfaction metrics weekly
- Plan customer communication for major changes
- Reserve capacity for urgent customer issues

---

## Contributing

SPARK Framework is open source and community-driven. We welcome:
- Experience reports from teams using SPARK
- Improvements to the framework based on real usage
- Templates and examples for different contexts
- Documentation improvements

---

## License

SPARK Framework is released under MIT License. Use it, modify it, teach it. Help make work better for everyone.

Created by the startup community, for the startup community.

---

*Remember: The goal isn't to follow SPARK perfectly. The goal is to ship value to customers sustainably while building resilient, high-performing teams. SPARK is a means to that end, not the end itself.*