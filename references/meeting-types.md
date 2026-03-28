# Meeting Types Reference

Detailed flow definitions for each meeting type. The main SKILL.md references this file for type-specific behavior.

---

## 1. progress-sync (进度同步)

**When to use**: Regular check-ins, start of work session, after a break, weekly sync.

**Moderator**: CEO

**Speaking order**: Engineer → Designer → Product → Marketing → CEO (builders first, strategist last)

**Flow**:
1. Each role reports: what they accomplished, what's in progress, what's blocked
2. Cross-role dependency check: "Does anyone need something from another role?"
3. Blocker resolution: prioritize and assign owners to unblock
4. CEO sets priorities for next period

**Required output**:
- Status summary per role (1-2 lines each)
- Blocker list with owners
- Top 3 priorities for next period

**Anti-patterns**:
- Turning into a decision meeting (park decisions, schedule separate meeting)
- Status reports longer than 3 sentences per role
- Discussing solutions to problems instead of just flagging them

---

## 2. decision (方案评审)

**When to use**: Choosing between approaches, evaluating a proposal, go/no-go decisions.

**Moderator**: CEO

**Speaking order**: Proposer first → Engineer (feasibility) → Product (user value) → Designer (UX impact) → Marketing (market impact) → CEO (decision)

**Flow**:
1. Proposer presents the options clearly (max 3 options)
2. Each role evaluates from their perspective with pros/cons
3. Open debate: roles challenge each other's assessments
4. CEO synthesizes and decides
5. Record: decision, rationale, trade-offs accepted, dissent

**Required output**:
- Options considered (with brief description)
- Decision and primary rationale
- Trade-offs explicitly accepted
- Dissenting opinions (if any)

**Anti-patterns**:
- Analysis paralysis (more than 3 options = narrow first)
- False consensus (if everyone agrees too easily, CEO should probe harder)
- Deciding without data ("I feel like..." is not an argument)
- Revisiting already-decided items without new information

---

## 3. milestone (里程碑复盘)

**When to use**: End of a phase, sprint review, before major pivot, quarterly review.

**Moderator**: Product (owns the roadmap)

**Speaking order**: Product (overview) → Engineer (technical status) → Designer (quality assessment) → Marketing (market readiness) → CEO (strategic adjustment)

**Flow**:
1. Product presents: planned vs actual, what shipped, what slipped
2. Engineer explains technical wins and remaining debt
3. Designer assesses quality and polish level
4. Marketing evaluates market timing and readiness
5. CEO adjusts priorities and timeline for next phase

**Required output**:
- Completed items checklist
- Slipped items with reasons
- Updated milestone/timeline table
- Adjusted priorities for next phase

**Anti-patterns**:
- Blame game (focus on what to do differently, not who failed)
- Ignoring slippage (if something slipped, acknowledge and adjust)
- Not updating the timeline (milestone review without timeline update is pointless)

---

## 4. problem-solving (问题排查 / War Room)

**When to use**: Bug investigation, incident response, performance issue, user complaint pattern.

**Moderator**: Engineer (owns the technical investigation)

**Speaking order**: Engineer (technical analysis) → Product (user impact) → Designer (UX implications) → Marketing (communication plan) → CEO (resource allocation)

**Flow**:
1. Engineer presents: symptoms, data, hypotheses for root cause
2. Product quantifies user impact and urgency
3. Designer identifies UX-level mitigations (even if temporary)
4. Marketing plans communication if user-facing
5. Team debates solutions: quick fix vs proper fix vs both
6. CEO allocates resources and sets timeline

**Required output**:
- Problem statement (1-2 sentences)
- Root cause (confirmed or top hypothesis)
- Chosen solution with timeline
- Communication plan (if user-facing)

**Anti-patterns**:
- Jumping to solutions before understanding the problem
- Fixing symptoms instead of root cause
- Not setting a deadline for the fix
- Forgetting to communicate to affected users

---

## 5. brainstorm (头脑风暴)

**When to use**: New feature ideation, naming, creative direction, exploring possibilities.

**Moderator**: Designer (owns creative process)

**Speaking order**: Free-form in diverge phase, structured in converge phase

**Flow**:
1. **Diverge** (no criticism allowed):
   - Each role generates 2-3 ideas from their perspective
   - Build on others' ideas ("yes, and...")
   - Wild ideas encouraged
2. **Converge**:
   - Group similar ideas
   - Each role votes for top 2 (with brief reasoning)
   - Identify the 2-3 strongest candidates
3. **Select**:
   - Brief debate on finalists
   - CEO makes final selection (or decides to prototype multiple)

**Required output**:
- Full idea list (even rejected ones, for future reference)
- Top 3 candidates with pros/cons
- Selected approach with rationale

**Anti-patterns**:
- Criticizing during diverge phase ("that won't work" kills creativity)
- Only generating safe/obvious ideas
- Not building on others' ideas
- Selecting by loudest voice instead of merit

---

## 6. kickoff (启动会)

**When to use**: Starting a new project, new phase, new initiative, onboarding to existing project.

**Moderator**: CEO (sets the vision)

**Speaking order**: CEO (vision) → Product (scope) → Engineer (technical approach) → Designer (design direction) → Marketing (go-to-market)

**Flow**:
1. CEO states: why this project, what success looks like, constraints
2. Product defines: MVP scope, user stories, what's in/out
3. Engineer proposes: technical approach, major risks, timeline estimate
4. Designer outlines: design direction, key screens/flows, style
5. Marketing plans: positioning, target audience, launch strategy
6. All roles confirm alignment or raise concerns
7. CEO finalizes scope and timeline

**Required output**:
- Project goal (1-2 sentences)
- MVP scope (in/out list)
- Technical approach summary
- Key milestones with dates
- Role assignments

**Anti-patterns**:
- Scope creep in the kickoff itself ("while we're at it...")
- No clear success criteria
- Unrealistic timeline without engineer buy-in
- Skipping the "what's OUT of scope" discussion
