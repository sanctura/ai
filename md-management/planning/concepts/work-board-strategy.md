# Work Board Strategy: Asana Implementation

**Purpose**: Create a shared workspace with each direct report to manage tasks, projects, and collaboration in a transparent, prioritized way.

**Date Created**: 2026-01-23

---

## Core Concept

Each direct report gets their own Asana project functioning as a "work board" - a shared space between you (MD) and them to:
- Track all work items in one visible location
- Distinguish between quick tasks and substantive work
- Prioritize collaboratively
- Create accountability without micromanagement
- Streamline 1:1 discussions

---

## Standard Section Structure

Every work board will have these sections:

### 1. Rapid Tasks
Quick items that take <30 minutes. These accumulate between meetings and get knocked out efficiently.
- Examples: "Send Elena the compliance checklist", "Review and approve PO", "Reply to vendor query"
- Rule: If it takes longer than expected, promote to a proper section

### 2. This Week
Active focus items for the current week. Limited to 3-5 items max to maintain focus.
- Pulled from Backlog during 1:1 or start of week
- Clear ownership and expected completion

### 3. In Progress
Larger work items actively being worked on. These span multiple days/weeks.
- Include subtasks for complex items
- Update status/comments as work progresses

### 4. Backlog
Prioritized queue of future work. Review during 1:1s to decide what moves to "This Week."
- Ordered by priority (top = highest)
- Add new items here by default

### 5. Waiting On
Items blocked pending input from someone else (including you).
- Tag who it's waiting on
- Review weekly to unblock

### 6. Done (This Month)
Completed items. Archive monthly for a sense of progress and to keep board clean.

---

## Approach by Staff Member

### Yaseen Harneker (CPO - Chief Project Officer)

**Nature of Work**: Strategic group-wide projects including capital equipment commissioning, radiation bunker development, chemotherapy licensing, regulatory delivery, and infrastructure initiatives

**The Challenge with CPO Work**:
CPO projects are large, multi-phase strategic initiatives that:
- Span months with many subtasks and milestones
- Have some subtasks active now, others that activate later
- Never fully "complete" until the entire project delivers

The standard "This Week" / "In Progress" model breaks down because:
- A 6-month project can't live in "This Week" forever
- "In Progress" becomes a dumping ground for everything active
- No distinction between "the whole project" and "what I'm actually working on right now"

**Solution: Project as Custom Field**

**Core Insight**: Projects don't sit on the board as tasks - they're a lens to filter by. Only granular, actionable milestones appear on the board. Tasks flow through simple workflow sections.

- **Project = Custom Field** (a filter/category)
- **Tasks = Granular milestones** (specific deliverables)
- **Sections = Workflow state** (where things are right now)

**Suggested Sections**:
| Section | Purpose |
|---------|---------|
| Spotlight | This week's focus - max 3-5 specific deliverables actively being driven |
| Backlog | Prioritized queue of upcoming work across all projects |
| Waiting On | Blocked on external parties (vendors, regulators, internal teams) |
| Done | Completed milestones (archive monthly) |

Simple 4-section workflow. Clean and focused.

**How It Works**:

*Board View Example*:
```
[Spotlight] ─────────────────────────────
  Submit permit application      [Radiation Bunker]
  Finalize vendor contract       [Capital Equipment]
  Complete licensing docs        [Chemo Licensing]

[Backlog] ───────────────────────────────
  Contractor RFP                 [Radiation Bunker]
  Inspection scheduling          [Chemo Licensing]
  Equipment spec review          [Capital Equipment]
  Foundation work planning       [Radiation Bunker]

[Waiting On] ────────────────────────────
  Permit approval                [Radiation Bunker]
  Regulatory response            [Chemo Licensing]

[Done] ──────────────────────────────────
  Architectural drawings         [Radiation Bunker]
  Initial budget approval        [Capital Equipment]
```

*Filtering by Project*:
To see all work for "Radiation Bunker":
- Filter custom field "Project" = Radiation Bunker
- Shows: Spotlight + Backlog + Waiting On + Done items for that project
- Full project roadmap visible through one filter

**Weekly Rhythm**:
1. **Start of week**: Review Backlog, pull 3-5 items into Spotlight
2. **During week**: Work Spotlight items, move to Done when complete
3. **Blocked items**: Move to Waiting On, tag who/what it's waiting on
4. **In 1:1**: Walk Spotlight (current focus), check Waiting On (unblock), review Backlog (prioritize next)

**1:1 Integration**: Use board as agenda - walk Spotlight first (what's the focus?), check Waiting On (what can we unblock?), review Backlog (what's coming next?). Filter by project when diving deep on specific initiatives.

**Key Fields to Track**:
| Field | Options | Purpose |
|-------|---------|---------|
| Project | Radiation Bunker / Chemo Licensing / Capital Equipment / [Others] | Which project this milestone belongs to |
| Target Date | Date | When this milestone should complete |
| Dependency | Vendor / Regulator / Internal / None | What's this blocked on (for Waiting On items) |

**Why This Works Better**:

| Problem | Solution |
|---------|----------|
| "Radiation Bunker" sits in one section forever | No parent project task - only granular milestones that complete and move to Done |
| "This Week" vs "In Progress" confusion | Single "Spotlight" section = this week's active focus. No ambiguity. |
| Future work clutters the view | Future milestones sit in Backlog until pulled to Spotlight |
| Can't see full project status | Filter by Project custom field to see all tasks across sections |

---

### Alida Wiese (Finance Manager)

**Nature of Work**: Cyclical financial operations, reporting, budgeting, CFO collaboration

**Board Focus**:
- Recurring tasks are central - monthly close, payroll, reporting cycles
- Clear deadlines matter more here than other roles
- Coordination with fractional CFO needs visibility

**Suggested Sections**:
| Section | Purpose |
|---------|---------|
| Rapid Tasks | Quick approvals, queries, small requests |
| This Week | Current week priorities |
| Monthly Cycle | Recurring monthly tasks (close, reports, payroll) |
| Projects | Larger initiatives (budget, system changes) |
| CFO Coordination | Items involving fractional CFO |
| Waiting On | Blocked items |
| Done | Completed work |

**1:1 Integration**: Start with Monthly Cycle status, then walk projects and blockers.

**Key Fields to Track**:
- Due date (critical for finance)
- Recurring (yes/no)
- Reporting period affected

---

### Kyle Bennett (Practice Manager)

**Nature of Work**: Day-to-day practice operations, reception management, facilities, patient experience

**Board Focus**:
- Higher volume of "Rapid Tasks" - operational role has many quick items
- Facilities and equipment tracking important
- Team management items (3 direct reports)

**Suggested Sections**:
| Section | Purpose |
|---------|---------|
| Rapid Tasks | Quick operational items, approvals |
| This Week | Current week priorities |
| Reception & Front Desk | Patient experience, scheduling, team items |
| Facilities | Maintenance, equipment, environment |
| Staff Management | Team-related items for his 3 reports |
| Waiting On | Blocked items |
| Done | Completed work |

**1:1 Integration**: Quick scan of Rapid Tasks, deeper dive on any facility or staff issues.

**Key Fields to Track**:
- Urgency (Today / This Week / Can Wait)
- Category (Reception / Facilities / Staff)
- Cost implication (if any)

---

### Dr Elena Hilton (Medical Officer - Cape Town)

**Nature of Work**: Clinical oversight, nursing team management (7 staff), Cape Town operations, medical protocols

**Board Focus**:
- Clinical/compliance items need clear tracking
- Team management for 7 nursing staff
- Less frequent 1:1s (bi-weekly) so board needs to capture more between meetings

**Suggested Sections**:
| Section | Purpose |
|---------|---------|
| Rapid Tasks | Quick clinical queries, approvals |
| This Week | Current week priorities |
| Clinical Operations | Patient care, protocols, quality |
| Nursing Team | Team management for 7 staff |
| Compliance & Training | Regulatory, certifications, training |
| Waiting On | Blocked items |
| Done | Completed work |

**1:1 Integration**: Critical to review board before bi-weekly 1:1 given less frequent touchpoints. Use board to capture items between meetings.

**Key Fields to Track**:
- Clinical impact (High / Medium / Low)
- Staff member involved (for team items)
- Compliance deadline (if applicable)

---

### Dr Ismaeel Ebrahim (Medical Officer - London)

**Nature of Work**: Clinical oversight, nursing team management (4 staff), London operations, UK medical protocols

**Board Focus**:
- Similar structure to Elena but London-specific
- UK regulatory/compliance considerations
- Timezone awareness (11am+ SAST meetings)
- Smaller team (4 vs 7)

**Suggested Sections**:
| Section | Purpose |
|---------|---------|
| Rapid Tasks | Quick clinical queries, approvals |
| This Week | Current week priorities |
| Clinical Operations | Patient care, protocols, quality |
| Nursing Team | Team management for 4 staff |
| UK Compliance | UK-specific regulatory, CQC, training |
| Waiting On | Blocked items |
| Done | Completed work |

**1:1 Integration**: Same as Elena - bi-weekly requires good board hygiene. Async updates even more important due to timezone.

**Key Fields to Track**:
- Clinical impact (High / Medium / Low)
- Staff member involved
- UK compliance deadline

---

## Operating Principles

### Adding Tasks
- **Either party can add tasks** - this is collaborative, not top-down
- Default new items to **Backlog** unless urgent
- Use task comments for context/discussion rather than separate messages
- Tag each other when input needed

### During 1:1s
1. Quick scan of **Rapid Tasks** - knock out or delegate immediately
2. Review **This Week** - are we on track?
3. Check **Waiting On** - can we unblock anything?
4. Pull from **Backlog** to **This Week** as capacity allows
5. Add new items that came up in discussion

### Between 1:1s
- Update task status when things change
- Add comments rather than separate Slack/email threads
- Move completed items to Done
- Add new items as they arise

### Monthly Hygiene
- Archive "Done" items older than 1 month
- Review Backlog for stale items (delete or deprioritize)
- Assess if section structure still serves the work

---

## Success Metrics

After 30 days, assess:
- [ ] Both parties regularly adding/updating tasks
- [ ] Board is reviewed in every 1:1
- [ ] Fewer "I forgot about that" moments
- [ ] Reduced status-check messages between meetings
- [ ] Clear view of what each person is working on

After 90 days, assess:
- [ ] Patterns visible (recurring blockers, capacity issues)
- [ ] Improved alignment on priorities
- [ ] Historical record of accomplishments for reviews

---

## Rollout Sequence

**Week 1**: Yaseen + Alida (Mon 1:1s - start of week)
- Introduce concept, create boards together
- Seed with current known work items

**Week 2**: Kyle + Elena/Ismaeel (depending on cycle week)
- Apply learnings from Week 1
- Refine section structure if needed

**Week 3**: Remaining Medical Officer
- Full coverage of all direct reports

**Week 4**: Review and refine
- What's working? What needs adjustment?
- Finalize section structure as standard template

---

*Last Updated: 2026-01-23*
