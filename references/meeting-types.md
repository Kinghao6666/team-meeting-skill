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

---

## 7. retrospective (回顾会)

**When to use**: End of a sprint/phase, after a major release, after an incident, or periodically to reflect on process.

**Moderator**: Product (owns process improvement)

**Speaking order**: Free-form in reflection phases, structured in commitment phase

**Flow**:
1. **What went well**: Each role shares 1-2 things that worked — celebrate wins
2. **What went wrong**: Each role shares 1-2 pain points — no blame, focus on process
3. **Root causes**: Team discusses WHY things went wrong, not just WHAT
4. **Improvement actions**: Propose concrete changes (not "try harder")
5. **Commitments**: Each role commits to ONE specific improvement for next cycle

**Required output**:
- Wins list (what to keep doing)
- Pain points list (what to stop/change)
- Root cause analysis for top 2-3 pain points
- Improvement commitments with owners

**Anti-patterns**:
- Blame game ("you broke it" instead of "the process allowed this to happen")
- Vague improvements ("communicate better" — HOW?)
- Too many commitments (pick 2-3, not 10)
- Skipping the celebration of wins (morale matters)

---

## 8. go-no-go (发布决策)

**When to use**: Before a major release, launch, or irreversible deployment.

**Moderator**: CEO (owns the final call)

**Speaking order**: Engineer (technical readiness) → Product (feature completeness) → Designer (quality/polish) → Marketing (market readiness) → CEO (final decision)

**Flow**:
1. Each role declares **GO** or **NO-GO** with specific reasoning
2. NO-GO items are listed as blockers with severity (critical/major/minor)
3. Team debates: can blockers be mitigated without delaying?
4. CEO makes final call: GO, NO-GO, or CONDITIONAL GO (go with known issues)
5. If CONDITIONAL GO: list accepted risks explicitly

**Required output**:
- Per-role GO/NO-GO status with reasoning
- Blocker list with severity
- Final decision: GO / NO-GO / CONDITIONAL GO
- If GO: launch date and rollback plan
- If NO-GO: what must be fixed and revised target date

**Anti-patterns**:
- Rubber-stamping (everyone says GO without real assessment)
- Perfectionism (NO-GO for minor polish issues)
- No rollback plan (what if launch goes wrong?)
- Ignoring marketing/market readiness (technically ready ≠ market ready)

---

## 9. sprint-planning (迭代规划)

**When to use**: Start of a work week/sprint, planning the next iteration of work.

**Moderator**: Product (owns the backlog)

**Speaking order**: Product (priorities) → Engineer (capacity + estimates) → Designer (design needs) → Marketing (upcoming deadlines) → CEO (final scope)

**Flow**:
1. **Review last sprint**: Check commitments vs actuals — what shipped, what slipped, why
2. **Present candidates**: Product lists top priority items from backlog
3. **Estimate effort**: Engineer estimates each item (hours or T-shirt sizes)
4. **Capacity check**: Total estimates vs available time — cut if overloaded
5. **Commit**: Team agrees on the sprint scope — this is a promise, not a wish list
6. **Assign owners**: Each item gets a clear owner

**Required output**:
- Last sprint review (shipped/slipped/why)
- This sprint committed items with estimates and owners
- Stretch goals (nice-to-have if time permits, clearly marked)
- Total capacity vs committed load

**Anti-patterns**:
- Overcommitting (planning 50 hours of work for a 40-hour week)
- No estimates ("we'll just see how far we get")
- Carrying over slipped items without asking why they slipped
- Not leaving buffer for unexpected work (bugs, urgent requests)

---

## 10. design-review (方案评审)

**When to use**: Evaluating a technical architecture, visual design, or product proposal before implementation.

**Moderator**: Engineer (for technical reviews) or Designer (for visual reviews)

**Speaking order**: Presenter first → each role reviews from their perspective → open discussion → verdict

**Flow**:
1. **Present**: Proposer explains the design/architecture (goals, approach, trade-offs)
2. **Per-role review**: Each role evaluates from their domain:
   - Engineer: feasibility, performance, maintainability, tech debt
   - Product: user value, requirement coverage, edge cases
   - Designer: consistency, usability, visual quality
   - Marketing: market fit, messaging implications
   - CEO: strategic alignment, resource justification
3. **Risk identification**: What could go wrong? What's the worst case?
4. **Change requests**: Specific modifications required before approval
5. **Verdict**: APPROVED / APPROVED WITH CHANGES / REJECTED (with reasons)

**Required output**:
- Design summary (what was reviewed)
- Per-role feedback
- Risk list
- Change requests (if any)
- Verdict with conditions

**Anti-patterns**:
- Reviewing without understanding the goals first
- Bikeshedding (debating minor details while ignoring major risks)
- No clear verdict (ending with "looks good I guess")
- Approving without identifying any risks (nothing is risk-free)

---

## 11. demo (成果演示)

**When to use**: Showing completed work to the team, end-of-sprint showcase, or validating that implementation matches expectations.

**Moderator**: Product (owns acceptance criteria)

**Speaking order**: Presenter demos → Product (acceptance check) → Designer (quality check) → Engineer (technical notes) → Marketing (positioning notes) → CEO (strategic fit)

**Flow**:
1. **Demo**: Walk through the completed work — show it running, not just describe it
2. **Acceptance check**: Product verifies against original requirements — what's met, what's missing
3. **Quality check**: Designer evaluates polish, consistency, UX issues
4. **Technical notes**: Engineer flags any technical concerns discovered during demo
5. **Feedback round**: Each role gives 1-2 specific feedback items
6. **Gap list**: Compile all missing/broken/unpolished items
7. **Next steps**: Prioritize gaps — fix now vs fix later vs won't fix

**Required output**:
- What was demoed (feature list)
- Acceptance status per feature (pass/fail/partial)
- Feedback list per role
- Gap/issue list with priority
- Next steps

**Anti-patterns**:
- Demoing slides instead of working software
- "It works on my machine" without showing real scenarios
- Only showing happy path (test edge cases too)
- No acceptance criteria defined beforehand (can't evaluate without standards)
