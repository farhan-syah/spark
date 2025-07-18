# The SPARK Framework

## A Project Management Framework for High-Velocity Teams

**Version 1.0.0**

---

## What is SPARK?

SPARK (Swift Product Acceleration through Rapid Knowledge) is a lightweight project management framework for building high-performing teams. It addresses common failure modes seen in growing organizations—such as decreased velocity, conflicting priorities, and excessive process overhead—by providing a simple, teachable system.

By combining principles from Agile, Lean, and modern product thinking, SPARK delivers three key outcomes:

**Clarity & Focus:** It eliminates ambiguity by ensuring every team is focused on a single, measurable objective.

**Sustainable Speed:** It creates a system of continuous flow, preventing the burnout and waste associated with traditional batch-based processes.

**Scalable Autonomy:** It provides a clear model for organizational growth that preserves the speed and agility of a small team.

At its core, SPARK is a framework for achieving maximum impact with minimum ceremony, enabling teams to do their best work.

### Core Philosophy
> "Sustainable speed beats temporary bursts of work. Flow beats batch. Outcomes beat outputs."

---

## The Five SPARK Principles

1. **Single-Piece Flow** - Work moves continuously, one item at a time per person
2. **Pull, Don't Push** - Team members pull work when ready
3. **Amplify Learning** - Every week, the team gets smarter
4. **Radically Minimize Waste** - Eliminate non-value-adding activities
5. **Keep It Simple** - The framework must be teachable in one hour

---

## Principles Over Rules

> **🎯 SPARK is for people who seek continuous improvement and learning**

When rules conflict with principles, **principles win**. The goal is customer value, team learning, and sustainable flow - not perfect rule compliance.

### How Teams Grow with SPARK

**New Teams:**
- Start with the basic rules - they provide structure and safety
- Focus on building habits: pulling work, preserving context, linking to OKRs
- Learn through practice and weekly retrospectives

**Developing Teams:**
- Begin to understand the "why" behind each rule
- Start recognizing when rigid rule-following hurts the principles
- Experiment with adaptations during retrospectives

**Experienced Teams:**
- Adapt rules intelligently while always honoring principles
- Handle complex scenarios naturally (pair programming, emergencies, spikes)
- Teach newer team members the principles behind the practices

**The Beauty of SPARK:**
The framework grows with you. It teaches better practices through experience, not through complexity. Simple teams can absolutely use SPARK - the more you use it, the more you'll grow with it.

### Intelligent Adaptations You'll Learn

As teams mature with SPARK, they naturally learn to handle complex scenarios:

**Pair Programming:**
- Treat the pair as single owner (@alice-bob)
- One card counts for both people - they're 100% focused on one item
- Honors the spirit of WIP limit: prevents multitasking, encourages focus

**Emergency Work:**
- Use built-in escape hatch: temporarily break WIP limit for critical issues
- Make exceptions visible (e.g., "Emergency" swimlane)
- Return to normal flow once resolved

**Exploratory Spikes:**
- Frame in terms of risk reduction for OKRs
- "Done" = knowledge gained, decisions made, risks clarified
- Still links to Key Results by de-risking them

### Anti-Pattern Warning

❌ **Following rules so literally that you subvert the principles**

Examples:
- Sequential handoff disguised as "pair programming"
- Refusing urgent work because "WIP limit doesn't allow it"
- Rejecting valuable research because it's "not shippable"

Remember: SPARK is your teacher, not your judge. Learn from mistakes, adapt through retrospectives, and always serve the principles.

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

> **🎯 Sweet Spot: 5-10 people per pod for maximum flow and autonomy**

- **1-10 people**: Single workspace with one objective
- **10+ people**: Multiple workspaces (pod structure), each with focused objective
- **Cross-workspace coordination**: Pod leads sync weekly, but each workspace maintains independent focus

**Team Size Considerations**:
- **Solo developers (1 person)**: SPARK provides structure for personal productivity and learning
- **Small teams (2-4 people)**: Excellent for tight coordination and rapid iteration
- **Optimal teams (5-10 people)**: Best balance of diverse skills, efficient communication, and sustainable workload
- **Beyond 10 people**: Use pod structure to maintain SPARK's core benefits

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

### 2. Forecasting Without Estimation

In SPARK, we don't "estimate" tasks with story points. Instead, we use lightweight forecasting to answer business questions about timelines and scope, while relying on radical decomposition to ensure a predictable flow of daily work.

The process flows from the big picture down to the small details:

**1. The Themes Roadmap (12-18 Month View)**

This is your high-level strategic narrative. It communicates long-term direction to stakeholders.

- **What it is:** A list of broad business outcomes, not features (e.g., "Improve onboarding experience," "Increase platform reliability," "Expand into new markets")
- **How to forecast:** Use Quarters as the unit of measure. This is about general timing, not precise duration
- **Example:** "We plan to focus on the onboarding experience in Q2, and we are confident it will be our primary theme by Q3"

**2. Larger Initiatives on the Backlog (1-3 Month View)**

When a Theme is ready to be considered for the next quarter, it's broken down into larger initiatives.

- **What it is:** A significant piece of work that will deliver a Key Result (e.g., "Build the new user checklist," "Migrate the primary database")
- **How to forecast:** Use T-Shirt Sizes based on weeks of effort:
  - **S (Small):** ≈ 1-2 weeks
  - **M (Medium):** ≈ 3-6 weeks
  - **L (Large):** ≈ 7-12 weeks (a full quarter)
  - **XL (X-Large):** Too big! This initiative must be broken down further before it can be worked on

**3. The Forecast Conversation**

Use Confidence Ranges to set realistic expectations. This is the primary tool for answering "When will it be done?"

- **Example:** After sizing an initiative as a "Medium," the conversation with a stakeholder should sound like this: "This looks like a Medium-sized initiative, so we believe it will take around 3 to 6 weeks to complete. We'll know more once we start breaking it down."

**Key Principles for SPARK Forecasting:**
- **Decomposition Over Estimation:** For daily work, decompose tasks to be less than one week. This is the ultimate key to predictable flow
- **Communicate Uncertainty:** Always give ranges, not single dates. A forecast is an educated guess, not a promise
- **Track Throughput, Not Velocity:** Measure your team's historical throughput (number of work items completed per week) to inform your forecasts. If your team completes 3-5 items per week, a Large initiative will require breaking down into many smaller tasks
- **Forecast Outcomes, Not Outputs:** Frame your forecasts around delivering value (e.g., "The new onboarding flow should be live in 4-6 weeks"), not just finishing tasks

### 3. The SPARK Board

A simple 4-column visual board:

```
┌─────────────┬──────────────┬──────────────┬─────────────┐
│   BACKLOG   │ IN PROGRESS  │    REVIEW    │    DONE     │
│             │ (WIP Limit: 1 per person) │              │             │
├─────────────┼──────────────┼──────────────┼─────────────┤
│ Feature A   │ Feature B    │ Feature C    │ Feature Z   │
│ KR1: +10%   │ @alice       │ @bob         │ Shipped ✓   │
│             │              │              │             │
│ Feature D   │              │              │ Feature Y   │
│ KR2: +5%    │              │              │ Shipped ✓   │
└─────────────┴──────────────┴──────────────┴─────────────┘
```

**Guidelines:**
- **WIP limit of 1 per person** in "In Progress" column only
- Once task moves to "Review", person can immediately pull next task
- Items should link to a Key Result
- "Done" means the work item has delivered its intended value. For features, this means shipped to real users. For other work like spikes or technical debt, this means the learning is captured or the system is improved

**Why WIP Limit of 1:**
- **Accountability**: Clear answer to "who's working on this?"
- **Focus**: Prevents multitasking and context switching
- **Flow**: Exposes bottlenecks and forces the team to resolve them
- **Learning**: Requires breaking work down into small, valuable pieces

**Handling Real-World Complexity:**

SPARK's WIP limit is a discipline, not a dogmatic rule. Here's how mature teams handle common scenarios:

| Scenario | The SPARK Solution | Principle Applied |
|----------|-------------------|-------------------|
| **Pair Programming** | The **pair becomes the single owner** (`@alice-bob`). The card is their shared focus. | **Focus**: Two minds, one task. This is the ideal state of focus. |
| **Emergency Work** | **Use the escape hatch.** Pull the emergency item immediately and make the exception **visible** on the board. | **Outcome over Process**: The flow of customer value is more important than rigid rule compliance. |
| **External Blocker**<br/>(e.g., waiting for an API key from another team) | The task is **truly blocked**. Move it back to the Backlog with rich context explaining the blocker. Pull new work. | **Minimize Waste**: Prevents idle time. The context ensures work can be resumed by anyone once unblocked. |
| **Task Requires Multiple Skills**<br/>(e.g., frontend/backend work) | **Keep the flow going.** The primary owner pulls the other person in. This can be done via:<br/>1. **Swarming:** Bob helps Alice finish her part so the card can keep moving.<br/>2. **Pairing:** Alice and Bob pair up to complete the task together under a single owner (`@alice-bob`). | **Flow**: Avoids the waste of handoffs and queues. The goal is to get the item to "Done," not just to finish your part. |

**The Key Takeaway:** The WIP limit is a tool to force a crucial conversation: **"What is the fastest way to get *this specific item* to Done?"** Sometimes the answer is to focus alone, sometimes it's to pair up, and sometimes it's to pause and swarm a blocker. SPARK's context preservation ensures that no matter the path, knowledge and accountability are never lost.

**Task Flow and Ownership:**
- Single owner while in "In Progress"
- Owner can unassign themselves at any time
- Tasks rejected from Review return to Backlog with enhanced context
- Any team member can pull any Backlog task (with accumulated context)
- Context enables smooth handoffs between team members

**Optional:** Teams may add columns (Ready), swimlanes, or visual indicators as needed.

#### Proposal Board

To protect the main backlog's focus, all new ideas and non-urgent bugs first enter the Proposal Board. This is a companion board for team suggestions:

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

### 4. Work Items

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

### 5. The SPARK Week

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

### 6. Roles & Responsibilities

SPARK has one core role, the Product Owner, but thrives when responsibilities are distributed across the team.

**Product Owner**
- Sets the strategic direction with OKRs and the Themes Roadmap
- Maintains the final say on backlog prioritization and scope
- Focuses on removing business and external blockers

**Team Members (Shared Responsibilities)**
- Pull work when ready, ship to production, and share learnings
- Own internal blocker resolution: Team members unblock each other on technical issues first
- Manage proposals: The team collectively reviews proposals during the Friday retro

**Optional: Tech Lead**

To further empower the team, one member may act as a "first among equals" to guide technical strategy. This is not a formal manager role. Their responsibilities include:
- Guiding technical decisions and architecture
- Mentoring other team members
- Serving as the final point of escalation for internal technical blockers

**Anti-Pattern Warning:** A Product Owner trying to handle all blockers and technical decisions will become the primary constraint. Successful SPARK teams distribute responsibility.

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

| ✅ Success Patterns | ❌ Anti-Patterns |
|-------------------|------------------|
| **Keep pods under 10 people** - Maintains focus and fast decision-making | **Workspace >10 people** - Dilutes focus, slows decisions |
| **One workspace = one objective** - Creates clear focus and eliminates context overlap | **Multiple objectives per workspace** - Creates confusion, context overlap |
| **Scale by adding new pods** - Maintains autonomy and avoids coordination overhead | **Scaling by adding people** - Causes friction, meeting overhead |
| **Maintain pod autonomy** - Preserves fast-flow benefits and ownership | **Centralized bottlenecks** - Defeats fast-flow benefits |
| **One workspace = one board** - Ensures clear ownership and priorities | **Multiple boards per workspace** - Unclear ownership, competing priorities |
| **Distributed blocker resolution** - Whole team owns unblocking, PO focuses on external blockers | **PO handles all blockers** - Creates superhuman PO bottleneck |
| **Break work down to <1 week** - Ensures predictable flow and easy estimation | **Work items too big** - Creates unpredictable delivery and estimation problems |
| **Every work item links to KR** - Maintains outcome focus and strategic alignment | **Work disconnected from OKRs** - Leads to feature factory mentality |
| **Review SLA of 24 hours max** - Prevents review bottlenecks and maintains flow | **Slow or inconsistent reviews** - Creates flow disruption and context loss |
| **Share knowledge regularly** - Friday retros include mini tech talks and learning | **Knowledge silos** - Information hoarding prevents team growth and creates bus factor risks |

---

## Scaling Beyond 10 People

When teams grow beyond 10 people, use a pod structure with **separate workspaces**:

> **🚀 Each pod operates like a mini-startup**: Fully autonomous, self-organizing, and accountable for its objective. Pod leads are facilitators, not bottlenecks.

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

### When to Split Your Pod

**Clear Signals for Creating New Pods:**
- ✅ Team exceeds 10 people
- ✅ Multiple objectives competing for attention on same board
- ✅ Board feels cluttered or confusing
- ✅ Discussions slow down or people feel out of the loop
- ✅ Meetings are taking too long or feel unfocused
- ✅ Team members don't understand all work items on the board

**How to Split:**
1. **Identify the new objective** - What distinct outcome needs focus?
2. **Create new workspace** - Set up separate board and OKR
3. **Move relevant work** - Transfer related items to new board
4. **Assign pod lead** - Designate someone to facilitate the new pod
5. **Establish coordination** - Set up regular sync with other pods

### Visual: Healthy vs Unhealthy Scaling

**❌ Unhealthy: Growing Single Pod**
```
┌─────────────────────────────────────────────┐
│ Marketing Workspace (15 people!)           │
│ OKR: Growth + Retention + Platform         │
│ ┌─────────────────────────────────────────┐ │
│ │ Cluttered Board                         │ │
│ │ Growth tasks │ Platform │ Retention    │ │
│ │ SEO feature  │ API bugs │ Onboarding   │ │
│ │ Ad campaign  │ Database │ Email flows  │ │
│ │ @12 people working on different goals   │ │
│ └─────────────────────────────────────────┘ │
└─────────────────────────────────────────────┘
```

**✅ Healthy: Independent Pods**
```
┌─────────────────────────┐  ┌─────────────────────────┐
│ Growth Pod (6 people)   │  │ Retention Pod (5 people)│
│ OKR: Customer Acquisition│  │ OKR: User Retention     │
│ ┌─────────────────────┐ │  │ ┌─────────────────────┐ │
│ │ Focused Board       │ │  │ │ Focused Board       │ │
│ │ SEO feature         │ │  │ │ Onboarding flow     │ │
│ │ Ad campaign         │ │  │ │ Email sequences     │ │
│ │ Landing pages       │ │  │ │ User analytics      │ │
│ └─────────────────────┘ │  │ └─────────────────────┘ │
└─────────────────────────┘  └─────────────────────────┘
           │                            │
           └──── Weekly Sync ────────────┘
```

### Managing Cross-Pod Dependencies

While pod autonomy is ideal, dependencies between pods are inevitable as organizations scale. The key is to manage them without destroying the focus and flow that makes SPARK effective.

The SPARK approach is to treat dependencies as formal agreements between autonomous teams, not as informal requests. Manage them transparently and resolve conflicts quickly.

#### 1. Dependency Negotiation (During Quarterly Planning)

Dependencies must be identified and negotiated *before* the quarter begins. There are two primary patterns:

**Dependency Contracts (For clear deliverables):**
When Pod A needs a specific deliverable from Pod B, they create a simple contract during OKR planning. It should define:
- **What:** The specific deliverable
- **When:** The target delivery timeline
- **Why:** Which of Pod A's KRs it unblocks
- **Success Criteria:** How both pods will know it's truly "done"

**Shared Key Results (For deep collaboration):**
For the most critical, interdependent work, the pods should create a Shared KR. This makes both pods jointly accountable for the same business outcome.
- *Growth Pod KR:* `Acquire 1000 new users via the new onboarding flow`
- *Platform Pod KR:* `Enable Growth Pod to acquire 1000 new users by delivering the new onboarding flow infrastructure`

#### 2. Operational Workflow (During the Quarter)

Use a **Dependency Card** on the requesting pod's board to track the agreement.

- **Owned By:** The requesting pod (the team that *needs* the work)
- **Status Flow:** `Requested` → `In Progress` → `Delivered` → `Verified`
- **Updates:** The providing pod is responsible for communicating status changes. The requesting pod is responsible for verifying the final delivery against the success criteria.

**Example Dependency Card:**

| Field | Value |
|-------|-------|
| **Title** | User Analytics API for Growth Dashboard |
| **Owner** | Growth Pod (`@alice`) |
| **Provider** | Platform Pod (`@bob`'s task `PLAT-123`) |
| **Status** | `In Progress` |
| **Contract** | API endpoints for user signup flow, delivery by Week 3 |
| **Success** | Growth Pod can track conversion funnel in the dashboard |

**Best Practice:** The Provider field should ideally link to the specific person and the task ID on the other pod's board for maximum clarity.

#### 3. Escalation Protocol

When pod leads can't resolve a dependency conflict:

**Level 1: Direct Negotiation (2 business days max)**
Pod leads negotiate, focusing on the question: "Which path delivers more immediate customer value relative to our OKRs?"

**Level 2: Dependency Arbiter (1 business day max)**
Escalate to a pre-designated shared manager or "dependency arbiter." They review the OKR impact and make a binding priority call.

**Level 3: Business Impact Assessment (Rarely needed)**
For mission-critical conflicts, leadership reviews the overall business impact, which may require adjusting a pod's quarterly OKRs.

**Key Principle:** A fast decision is better than a perfect one. A blocked dependency hurts everyone.

#### 4. Common Patterns

| ✅ Success Patterns | ❌ Anti-Patterns to Avoid |
|-------------------|-------------------------|
| First, try to split work to **eliminate** dependencies | Creating dependencies when a different work split would avoid it |
| Negotiate dependencies **upfront** during OKR planning | Ignoring dependencies until they become a crisis |
| Use **lightweight contracts** and visible Dependency Cards | Creating heavy administrative overhead or duplicate work tracking |
| **Resolve conflicts quickly** through the escalation protocol | Letting a centralized person or committee manage all dependencies |

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


**Q: How do we estimate?**
A: SPARK replaces detailed estimation with two distinct practices: radical decomposition for daily work and lightweight forecasting for strategic planning.

**For Individual Tasks:** The rule is decomposition, not estimation. Every task pulled from the backlog should be small enough to be completed in less than one week. At this level, detailed estimates are unnecessary waste.

**For Larger Initiatives:** To aid in business planning for bigger pieces of work, use lightweight forecasts to communicate the general scale and uncertainty:
- **T-Shirt Sizes:** For a rough sense of magnitude (e.g., S ≈ 1-2 weeks, M ≈ 3-6 weeks, L ≈ A full quarter)
- **Confidence Ranges:** For more defined initiatives (e.g., "We believe this will take 4-6 weeks to complete")

**Crucially, a forecast is a communication tool to aid in planning, not a delivery promise.** Its purpose is to provide business context without the wasteful ceremony of story-pointing. The most essential skill for predictable delivery in SPARK remains the team's ability to decompose work effectively.

**Q: What about roadmaps?**
A: SPARK replaces a traditional feature-based roadmap with a more flexible two-part system:

**The Themes Roadmap (The "What"):** This is your high-level, strategic narrative for the next 6-18 months. It communicates direction to stakeholders by focusing on the customer problems or business opportunities we will tackle.
- **Example Theme:** "Reduce new user time-to-value"

**Quarterly OKRs (The "How"):** This is your tactical execution plan for the next 3 months. OKRs define how we will measure our success in tackling a theme for that quarter.
- **Example OKR for the Theme above:** Objective: Create a frictionless onboarding experience. Key Result: Increase Week 1 user activation rate from 20% to 40%

**Q: Can we keep using release cycles?**
A: Yes. SPARK's small work breakdown makes this easy - work flows continuously but releases are batched. Teams ship when features are ready within the cycle.

**Q: Can this scale?**
A: Yes. Scaling is a core design principle of SPARK, not an afterthought. It scales by replicating small, high-performance teams ("pods"), not by creating complex layers of management.

**1-10 People:** A single pod operates with maximum simplicity.
**10-50+ People:** The organization scales by adding new, autonomous pods, each with its own focused objective. The "Workspace Architecture" and "Managing Cross-Pod Dependencies" sections detail exactly how this works.

The framework is intentionally designed to prevent the communication overhead and loss of focus that typically slow down growing teams.

**Q: What tools do we need?**
A: Any board works - digital kanban tools, sticky notes, whiteboard.

**Q: What skills does our team need?**
A: Work decomposition (breaking tasks into <1 week pieces) and a team culture of shared ownership, guided by a Product Owner who focuses on strategy and empowers the team to manage its own flow. These skills develop with practice.

**Q: How do we handle multiple priorities?**
A: OKRs force prioritization. If everything is urgent, nothing is urgent.

**Q: What about technical debt?**
A: Track it like features. Dedicate capacity to debt reduction during retros.

**Q: Should we use the AI enhancements?**
A: Only if they add value to your team. The context fields help human developers as much as AI agents - use them if better documentation and relationship tracking would reduce your rework. Consider starting with Level 0 (pure SPARK) and experimenting gradually. Many successful teams ignore AI features entirely and focus on core SPARK principles. Choose what fits your team's needs and comfort level.

---

## How SPARK Differs from Other Frameworks

| Framework | Work Flow | Planning | Roles | Scaling | Focus |
|-----------|-----------|----------|-------|---------|--------|
| **SPARK** | Continuous pull | OKRs (quarterly) | Minimal (PO + Team) | Independent pods | Outcomes + Learning |
| **Scrum** | Sprint batches | Story points + sprints | Multiple (SM, PO, Team) | Coordination layers | Process compliance |
| **Kanban** | Continuous flow | No planning | Minimal | Board replication | Workflow visualization |
| **Waterfall** | Sequential phases | Upfront planning | Defined roles | Functional departments | Phase completion |
| **SAFe** | Program increments | Multi-level planning | Extensive hierarchy | Coordination frameworks | Enterprise alignment |

**SPARK's Unique Approach:**
- **Radical autonomy**: Each pod is fully self-contained
- **Outcome obsession**: Every work item must advance a Key Result  
- **Knowledge compounds**: Context preservation across all work
- **Scale by splitting**: Add pods, never add complexity

---

## Is SPARK Working for You?

Use this diagnostic checklist to assess your SPARK implementation:

### ✅ Health Check: Signs SPARK is Working

**Flow Indicators:**
- [ ] Work moves smoothly from Backlog → In Progress → Review → Done
- [ ] Team members pull work when ready (not when assigned)
- [ ] Cycle time is predictable and improving
- [ ] "Done" means shipped to real users

**Team Indicators:**
- [ ] Everyone understands all work on the board
- [ ] Meetings are short and focused (<15 min for check-ins)
- [ ] People feel autonomous and empowered
- [ ] Learning happens every week and is captured

**Outcome Indicators:**
- [ ] OKRs are driving daily decisions
- [ ] Every work item clearly links to a Key Result
- [ ] Team is hitting quarterly objectives
- [ ] Customer impact is visible and measurable

### 🚨 Red Flags: Signs You Need to Adjust

**Flow Problems:**
- [ ] Work gets stuck in Review for days
- [ ] People are multitasking or working on multiple items
- [ ] Board feels cluttered or confusing
- [ ] "Done" items aren't reaching customers

**Team Problems:**
- [ ] Meetings are long or feel unproductive
- [ ] People feel overloaded or stressed
- [ ] Team members don't understand others' work
- [ ] Decisions are slow or unclear

**Outcome Problems:**
- [ ] OKRs feel disconnected from daily work
- [ ] Work items don't clearly link to objectives
- [ ] Team is missing quarterly targets
- [ ] Customer impact is unclear

### 💡 Quick Fixes
- **Too many red flags?** Consider splitting your pod or refocusing on core SPARK principles
- **Flow issues?** Review WIP limits and "Done" definition
- **Team issues?** Ensure everyone understands the board and can pull work
- **Outcome issues?** Reconnect work items to OKRs and customer impact

---

## Troubleshooting Common Issues

### "People are multitasking and ignoring WIP limits"
**Root cause**: Work items are too large or unclear
**Solution**: Break work into smaller pieces (<1 week each), clarify acceptance criteria

### "Board is cluttered and confusing"
**Root cause**: Multiple objectives on one board, or work items lack clear ownership
**Solution**: Split pod if multiple objectives, ensure every item has clear "what/why/who"

### "Meetings are taking too long"
**Root cause**: Too many people, or discussions are about details not decisions
**Solution**: Keep meetings to core team only, use async for updates, focus on blockers

### "Work gets stuck in Review"
**Root cause**: Unclear "Done" definition or reviewer unavailability
**Solution**: Define clear acceptance criteria, implement 24-hour Review SLA

### "Team feels disconnected from OKRs"
**Root cause**: Work items don't clearly link to Key Results
**Solution**: Every backlog item must tag a KR, remove items that don't advance objectives

### "People don't understand others' work"
**Root cause**: Complex or siloed work items
**Solution**: Break work into smaller pieces, add context documentation, pair more often

### "Nothing feels 'Done'"
**Root cause**: "Done" doesn't mean shipped to users
**Solution**: Redefine "Done" as "in production and measured", track customer impact

---

## Get Started

### Today
1. Read this guide with your team
2. Identify which transition approach fits your current process
3. Set up a simple 4-column board

### Tomorrow  
1. Define current quarter OKRs with your team
2. Move existing work into SPARK backlog format
3. Apply WIP limit of 1 per person (refer to the 'Principles Over Rules' section for handling exceptions like pairing)

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