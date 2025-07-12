# SPARK Framework - AI Development Module

## The AI Development Challenge

When humans and AI collaborate on development, two critical issues emerge:

1. **Double Work**: AI generates code → Human reviews → Human rewrites 50% → Waste
2. **Hidden Dependencies**: AI creates coupling between modules without human awareness

## SPARK-AI: Enhanced Framework for AI-Assisted Development

### Core Principle: "Specification Before Generation"

```
Traditional AI Dev:                    SPARK-AI Dev:
Human: "Build feature X"               Human: Writes spec first
AI: Generates 500 lines               AI: Reviews spec, asks questions  
Human: Realizes it's wrong            Human + AI: Align on approach
Human: Rewrites 300 lines             AI: Generates correct code
Result: 300 lines wasted              Result: 0 lines wasted
```

### The SPARK-AI Board (5 Columns)

```
┌────────────┬────────────┬──────────────┬────────────┬──────────┐
│   BACKLOG  │    SPEC    │ IN PROGRESS  │   REVIEW   │   DONE   │
│            │ [Human-Led]│ [AI-Assisted]│[Human-Led] │          │
├────────────┼────────────┼──────────────┼────────────┼──────────┤
│ Features   │ Define:    │ AI generates │ Human      │ Shipped  │
│ linked to  │ • Intent   │ based on     │ verifies:  │ to users │
│ OKRs       │ • Contract │ spec         │ • Correct  │          │
│            │ • Tests    │              │ • No hidden│          │
│            │ • Deps     │ Human guides │   deps     │          │
└────────────┴────────────┴──────────────┴────────────┴──────────┘
```

### New Work Item Format

```
┌─────────────────────────────────┐
│ TITLE: User Profile API         │
│ WHY: KR2 - Engagement +20%      │
│                                 │
│ SPEC: (Required before AI)      │
│ • Input: user_id: string        │
│ • Output: UserProfile object    │
│ • Deps: Only UserService        │
│ • Tests: List specific cases    │
│                                 │
│ CONSTRAINTS: (For AI)           │
│ • No new dependencies           │
│ • Use existing patterns         │
│ • Max 200 lines                │
└─────────────────────────────────┘
```

### Dependency Management Rules

1. **Explicit Dependency Declaration**
   ```
   Before AI generates anything:
   - List allowed dependencies
   - Specify forbidden dependencies
   - Define module boundaries
   ```

2. **Dependency Review Gate**
   ```
   AI Output → Dependency Scanner → Human Review
                     ↓
              [Auto-reject if new deps detected]
   ```

3. **The Import Freeze**
   ```
   # At top of spec
   ALLOWED_IMPORTS:
   - ./services/UserService
   - ./utils/validation
   - standard library only
   
   FORBIDDEN:
   - External packages
   - Other service modules
   - Database direct access
   ```

### Preventing Double Work

#### 1. The Specification Ritual (New)

**Before ANY AI generation:**
```
30-min Spec Session:
├─ 5 min: Write user story
├─ 10 min: Define interfaces/contracts  
├─ 10 min: List test scenarios
└─ 5 min: Declare dependencies
```

#### 2. Progressive Enhancement Pattern

Instead of "generate the whole feature":
```
Step 1: Human writes interface/types
Step 2: AI implements one method
Step 3: Human reviews, approves
Step 4: AI implements next method
...
Result: No large rewrites needed
```

#### 3. The AI Alignment Check

```
Human: Here's my spec [shows spec]
AI: I understand. To confirm:
     - Input types: ...
     - Output types: ...
     - Dependencies: ...
     - Constraints: ...
Human: Correct / [Adjustments]
AI: [Generates code]
```

### Modified SPARK Week for AI Development

**Monday Check-in (20 min)**
- Standard check-in
- Plus: "What needs specs this week?"

**Tuesday Spec Session (30 min)**
- Team writes specs together
- Clarify interfaces between modules
- Lock dependency boundaries

**Wednesday Blockers (15 min)**
- Include: "AI generated something unexpected"

**Thursday AI Review (30 min)**
- Review all AI-generated code as team
- Check for hidden dependencies
- Share patterns that worked

**Friday Retro (45 min)**
- Standard retro
- Plus: AI effectiveness metrics

### Metrics for AI Development

**Rework Rate**
```
AI Rework % = (Lines Changed After Generation / Total Lines Generated) × 100
Target: < 20%
```

**Dependency Creep**
```
Unwanted Dependencies = New deps introduced by AI per week
Target: 0
```

**Spec Coverage**
```
Spec Coverage = (Items with Spec / Total Items) × 100
Target: 100%
```

**AI Efficiency**
```
AI Success Rate = (AI code accepted as-is / Total AI generations) × 100
Target: > 80%
```

### Templates

#### Spec Template
```markdown
## Feature: [Name]
## KR Impact: [Which KR and expected impact]

### Interface
```typescript
// Input types
interface RequestDTO {
  // ...
}

// Output types  
interface ResponseDTO {
  // ...
}
```

### Dependencies
- ALLOWED: [explicit list]
- FORBIDDEN: [explicit list]

### Test Scenarios
1. Happy path: [description]
2. Error case: [description]
3. Edge case: [description]

### Constraints
- Max lines: [number]
- Performance: [requirements]
- Security: [considerations]
```

#### AI Prompt Template
```
Given this specification:
[paste spec]

Generate implementation following these rules:
1. Use ONLY the allowed dependencies
2. Follow existing patterns in [file]
3. Include error handling
4. Add unit tests
5. Keep under [X] lines

Do not:
- Add new dependencies
- Create new patterns
- Access database directly
- Add complex abstractions
```

### Dependency Visualization

```
BEFORE SPARK-AI:
┌─────────┐     ┌─────────┐     ┌─────────┐
│Service A│ ←-? │   AI    │ ?-→ │Service B│
└─────────┘     │Generated│     └─────────┘
      ↑         │  Code   │          ↑
      └---------│         │----------┘
                └─────────┘
        (Hidden dependencies everywhere)

WITH SPARK-AI:
┌─────────┐     ┌─────────┐     ┌─────────┐
│Service A│ ←-✓ │   AI    │ X   │Service B│
└─────────┘     │Generated│     └─────────┘
                │  Code   │
                └─────────┘
         (Explicit, controlled deps)
```

### Common Patterns

#### The "Interface First" Pattern
```
1. Human defines interface
2. Human writes tests against interface
3. AI implements interface
4. Tests pass = Done
```

#### The "Incremental Generation" Pattern
```
1. Generate smallest possible unit
2. Review and integrate
3. Generate next unit
4. Never generate > 100 lines at once
```

#### The "Dependency Injection" Pattern
```
// Spec includes:
"All dependencies must be injected via constructor"

// AI generates:
class Service {
  constructor(
    private userRepo: IUserRepo,  // Injected
    private logger: ILogger       // Injected
  ) {}
  // No direct imports or instantiations
}
```

### Rollout Plan

**Week 1**: Add SPEC column to board
**Week 2**: Implement spec templates
**Week 3**: Add dependency scanner
**Week 4**: Full SPARK-AI process

### Success Stories

**Before SPARK-AI:**
"We asked AI to build a payment system. It created 15 new dependencies, coupled to everything, and we rewrote 80% of it." - Startup CTO

**After SPARK-AI:**
"With specs, our AI rework dropped to 15%. No more surprise dependencies. We ship 3x faster." - Same CTO

## Summary

SPARK-AI solves the double-work problem through:
1. **Specification-first** development
2. **Progressive enhancement** vs big-bang generation
3. **Explicit dependency boundaries**
4. **Continuous alignment** between human intent and AI output

The result: AI becomes a true accelerator, not a source of technical debt.