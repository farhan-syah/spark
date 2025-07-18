# The SPARK Framework

## A Project Management Framework for High-Velocity Teams

**Version 1.0.0**

---

## What is SPARK?

SPARK (Swift Product Acceleration through Rapid Knowledge) is a lightweight project management framework designed for teams of 1-10 people who need to move fast while maintaining quality. For larger organizations, SPARK uses a pod structure where each pod operates as an independent 5-10 person team. It combines principles from Agile, Lean, and modern product thinking into a simple, teachable system.

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

## Workspace Architecture Principle

> **🎯 CORE RULE: One Workspace = One Board = One Objective**
> 
> This is SPARK's fundamental scaling principle. Each workspace contains exactly one board focused on a single Objective (OKR). To scale, add new workspaces (pods), never expand existing ones.

Each SPARK workspace contains exactly one board focused on a single Objective (OKR). This prevents the organizational chaos common when one workspace accumulates multiple boards with unclear ownership and conflicting priorities.

### Why This Matters

**Prevents "Board Proliferation":**
- No confusion about which board to use
- Clear ownership of each objective
- Simple mental model for team members

**Enables Multi-Team Organizations:**
- Growth Team Workspace → OKR: Acquire 1000 new customers
- Retention Team Workspace → OKR: Achieve 95% user retention  
- Platform Team Workspace → OKR: 99.9% system uptime

**Supports Cross-Team Participation:**
- Users can join multiple workspaces as needed
- Each workspace maintains its own focused objective
- Clear context switching between different team goals

### Implementation Examples

**✅ Good Organization:**
- **Company**: TechCorp (multiple workspaces)
  - **Growth Workspace**: One board, OKR: Customer acquisition
  - **Product Workspace**: One board, OKR: User engagement
  - **Platform Workspace**: One board, OKR: System reliability

**❌ Avoid This:**
- **Company**: TechCorp (single workspace)
  - Multiple boards: Growth Board, Product Board, Platform Board
  - Competing priorities and unclear focus

### Scaling Guidance

- **1-10 people**: Single workspace with one objective
- **10+ people**: Multiple workspaces (pod structure), each with focused objective
- **Cross-workspace coordination**: Pod leads sync weekly, but each workspace maintains independent focus

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
- WIP limit of 1 per person in "In Progress" column only
- Once task moves to "Review", person can immediately pull next task
- Items should link to a Key Result
- "Done" means shipped to real users

**Task Flow and Ownership:**
- Single owner while in "In Progress"
- Owner can unassign themselves at any time
- Tasks rejected from Review return to Backlog with enhanced context
- Any team member can pull any Backlog task (with accumulated context)
- Context enables smooth handoffs between team members

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

**Common Team Patterns:**
- Some teams limit active proposals per person (e.g., 3 max)
- Some teams add cool-down periods for resubmitted proposals
- Some teams do weekly proposal cleanup during retro
- Some teams run periodic "proposal quality reviews" if volume becomes unmanageable
- Some teams distinguish between "quick wins" and "exploration" proposals
- Adapt based on your team's proposal volume and culture

### 3. Work Items

Each work item contains:
- **What:** Clear description of the deliverable
- **Why:** Which Key Result it impacts
- **How:** Acceptance criteria
- **Who:** Single owner (when pulled)

**Optional Context (for AI-assisted development):**
- **Context:** Technical patterns, business constraints, team decisions
- **Relationships:** Dependencies, blockers, related work
- **Guidance:** Implementation approaches, safety considerations

**Context Examples:**
- **Technical:** "Uses React hooks", "Breaking change", "Requires DB migration"  
- **Business:** "Affects premium users", "Legal compliance required"
- **Team:** "Follow auth patterns", "Pair with Alice on security review"

**Context Guidelines:**
- Keep context concise - aim for 1-3 bullet points
- Focus on information that prevents the next person from making mistakes
- Avoid essays - use keywords and short phrases
- Ask: "What would someone pulling this work need to know?"

*For analog teams: These can be represented with colored dots, corner icons, or mini-cards rather than full text.*

*Note: Context fields are completely optional and don't affect core SPARK functionality.*

### SPARK's Core Power: Context Preservation

When tasks cycle through In Progress → Review → Backlog (due to rejection), they accumulate:
- Technical context from previous attempts
- Business insights from review feedback  
- Implementation approaches that were tried
- Blockers encountered and resolved

This means ANY team member can pick up ANY task and understand:
- What's been tried before
- Why previous approaches didn't work
- What the current status and next steps are
- Technical and business constraints discovered

**Result**: No work is ever "lost" and knowledge compounds across iterations.

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

**Optional AI-Enhanced Learning:**
- Pattern analysis: What patterns emerge from completed work?
- Context insights: How can better context prevent future issues?
- Relationship mapping: Which work items commonly connect?

*Note: AI enhancements are optional and don't change retro duration or core process.*

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

## Recognition and Rewards

**Flow-Based Recognition:**
- Items successfully pulled and completed per week
- Quality: tasks shipped without rework cycles
- Learning: context and insights contributed during task work
- Collaboration: helping others understand task context

**Recognition Metrics:**
- **Throughput**: Consistent task completion velocity
- **Quality**: Low rejection/rework rates
- **Knowledge**: Rich context documentation
- **Teamwork**: Cross-task collaboration and knowledge sharing

**Recognition Patterns:**
- Weekly acknowledgments during Friday retrospectives
- Peer recognition for context quality and knowledge sharing
- Celebration of customer impact when KRs advance

*Focus: Sustainable contribution patterns that improve team flow and knowledge.*

---

## Transitioning to SPARK

### From Scrum
Week 1: Keep your sprint, add OKRs
Week 2: Drop sprint planning, pull from backlog
Week 3: Drop daily standup, use async check-ins
Week 4: You're now running SPARK!

### From Kanban
Day 1: Add OKRs to your board
Day 2: Apply WIP limit of 1 in "In Progress" column
Day 3: Add Friday retrospectives
Done: You're running SPARK!

### From Waterfall
Month 1: Break project into 2-week deliverables
Month 2: Implement the SPARK board
Month 3: Add retrospectives and iterations
Month 4: Full SPARK implementation

---

## Common Patterns & Solutions

### Anti-Patterns to Avoid

| Anti-Pattern | Why It Hurts | Solution |
|-------------|-------------|----------|
| **Workspace >10 people** | Dilutes focus, slows decisions | Split into multiple workspaces |
| **Multiple objectives per workspace** | Creates confusion, context overlap | One workspace = one objective |
| **Scaling by adding people** | Causes friction, meeting overhead | Add new pods, not more people |
| **Centralized bottlenecks** | Defeats fast-flow benefits | Maintain pod autonomy |
| **Multiple boards per workspace** | Unclear ownership, competing priorities | One workspace = one board |

### Solutions to Common Patterns

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

When teams grow beyond 10 people, use a pod structure with **separate workspaces**:

**Pod Organization (Multiple Workspaces):**
```
Growth Workspace (Pod Alpha - 5 people):
• OKR: Customer acquisition
• Focus: Growth features
• Lead: Alice
• One board focused on acquisition

Retention Workspace (Pod Beta - 5 people):  
• OKR: Customer retention
• Focus: Core platform
• Lead: Bob
• One board focused on retention

Cross-Workspace Coordination:
• Weekly pod lead sync (30 min)
• Monthly all-hands retro (90 min)
• Shared technical standards
• Inter-workspace dependency management
```

**Key Principle**: Each pod = separate workspace with its own board and OKR. This maintains the "One Workspace = One Board = One Objective" architecture while enabling organizational scaling.

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
A: Any board works - digital kanban tools, sticky notes, whiteboard.

**Q: What skills does our team need?**
A: Work decomposition (breaking tasks into <1 week pieces) and an effective Product Owner who can prioritize, remove blockers, and communicate strategy. These skills develop with practice.

**Q: How do we handle multiple priorities?**
A: OKRs force prioritization. If everything is urgent, nothing is urgent.

**Q: What about technical debt?**
A: Track it like features. Dedicate capacity to debt reduction during retros.

**Q: Should we use the AI enhancements?**
A: Only if they add value to your team. The context fields help human developers as much as AI agents - use them if better documentation and relationship tracking would reduce your rework. Consider starting with Level 0 (pure SPARK) and experimenting gradually. Many successful teams ignore AI features entirely and focus on core SPARK principles. Choose what fits your team's needs and comfort level.

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

**Process Guidelines:**
- Write specifications before AI generates code
- Declare allowed/forbidden dependencies explicitly
- Review AI output for unexpected coupling
- Use progressive enhancement vs. big-bang generation

**Context Enhancement (Optional):**
- Add technical context to work items (tech stack, patterns, constraints)
- Document team decisions and architectural patterns
- Track relationships between work items
- Include business context and user impact
- Preserve implementation guidance for future reference

**Progressive Adoption:**
- **Level 0**: Use core SPARK without AI enhancements
- **Level 1**: Add context fields to selected work items
- **Level 2**: Include AI insights in Friday retrospectives
- **Level 3**: Full context capture and AI integration

**Implementation Examples:**
- **Analog teams**: Colored dots, simple icons, or corner abbreviations
- **Digital teams**: Custom fields, tags, or structured descriptions
- **Hybrid teams**: Mix of physical and digital context tracking
- Choose what works for your team's tools and culture

**AI Tool Considerations:**
- Consider training AI tools on your team's specific context
- Teams using AI often find local fine-tuning or team-specific prompts work better than generic tools
- Be aware that generic AI may not understand your domain, constraints, or team patterns
- Teams often find human validation of AI suggestions valuable
- Some teams disable AI features entirely - this is perfectly fine

*Context fields are completely optional - teams can ignore all AI enhancements while maintaining full SPARK functionality.*

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