# Asana Work Board Setup Guide

**Purpose**: Step-by-step instructions for creating and configuring work boards for each direct report.

**Reference**: See `work-board-strategy.md` for the strategic rationale and per-person approach.

---

## Prerequisites

- [ ] Asana Business or Enterprise account (for custom fields)
- [ ] Each direct report has an Asana account
- [ ] You have project creation permissions

---

## Phase 1: Create Projects (One Per Person)

### Step 1: Create the First Project

1. Click **+ Create** → **Project**
2. Choose **Blank project**
3. **Name**: `[Name] - Work Board` (e.g., "Yaseen - Work Board")
4. **Privacy**: Private to specific people (just you + that person)
5. **Default view**: Board (not List)
6. Click **Create project**

### Step 2: Add Team Member

1. Click **Share** (top right)
2. Add the direct report's email
3. Set permission to **Can edit** (they need to add/update tasks)
4. Send invite

### Step 3: Repeat for All 5 Reports

Create these projects:
- [ ] Yaseen - Work Board
- [ ] Alida - Work Board
- [ ] Kyle - Work Board
- [ ] Elena - Work Board
- [ ] Ismaeel - Work Board

---

## Phase 2: Configure Sections

For each project, set up the section structure. In Board view, sections appear as columns.

### Standard Sections (All Boards)

Click **+ Add section** to create each:

1. **Rapid Tasks** (leftmost - first thing you see)
2. **This Week**
3. **In Progress**
4. **Backlog**
5. **Waiting On**
6. **Done**

### Customized Sections by Person

After the standard sections, add role-specific sections:

**Yaseen (COO)**:
- Strategic Initiatives
- Process Improvements
- Cross-Location Items

**Alida (Finance)**:
- Monthly Cycle
- CFO Coordination

**Kyle (Practice Manager)**:
- Reception & Front Desk
- Facilities
- Staff Management

**Elena (Medical Officer - Cape Town)**:
- Clinical Operations
- Nursing Team
- Compliance & Training

**Ismaeel (Medical Officer - London)**:
- Clinical Operations
- Nursing Team
- UK Compliance

---

## Phase 3: Set Up Custom Fields

Custom fields help you filter, sort, and report. Create these at the project level.

### For All Projects

1. Click the dropdown next to project name → **Customize** → **+ Add custom field**

**Priority** (Dropdown):
- P1 - Urgent
- P2 - Important
- P3 - Normal

**Status** (Dropdown):
- Not Started
- In Progress
- Blocked
- Complete

### Role-Specific Fields

**Yaseen**:
- Location (Dropdown): Cape Town / London / Both

**Alida**:
- Recurring (Yes/No)
- Reporting Period (Text)

**Kyle**:
- Urgency (Dropdown): Today / This Week / Can Wait
- Category (Dropdown): Reception / Facilities / Staff

**Elena & Ismaeel**:
- Clinical Impact (Dropdown): High / Medium / Low
- Staff Member (Text or Dropdown if you list their team)

---

## Phase 4: Board View Configuration

### Set Default View

1. Open project in Board view
2. Click **Save layout as default**

### Configure Card Details

1. Click **Customize** → **Fields**
2. Enable these to show on cards:
   - Due date
   - Priority
   - Assignee

### Color Coding (Optional)

1. In Board view, click **Color** dropdown
2. Color by Priority:
   - P1 = Red
   - P2 = Yellow
   - P3 = Blue/Gray

---

## Phase 5: Seed Initial Tasks

Before your next 1:1 with each person, add known work items.

### Preparation Checklist

For each person, gather:
- [ ] Outstanding items from recent 1:1s
- [ ] Known projects they own
- [ ] Pending requests/tasks from email/Slack
- [ ] Quarterly goals (if defined)

### During First 1:1

Walk through the board together:
1. Explain the concept (shared workspace, not surveillance)
2. Show the sections and what goes where
3. Add items together - both of you contribute
4. Prioritize the Backlog
5. Pull 3-5 items to "This Week"
6. Agree on how you'll both use it going forward

---

## Phase 6: Establish Workflows

### Adding New Tasks

**Default behavior**: Add to Backlog unless urgent

**Urgent items**: Add directly to "This Week" and tag the person

**Rapid Tasks**: Small items go here with clear description

### Task Details Best Practices

When creating a task, include:
- Clear action-oriented title ("Review Q4 budget proposal" not "Budget stuff")
- Due date if applicable
- Subtasks for multi-step items
- Relevant attachments or links
- @mention if input needed

### Comments vs. New Tasks

- **Use comments** for: updates, questions, discussion on existing work
- **Create new task** for: distinct new work items, even if related

### Weekly Rhythms

**Before Monday 1:1s** (Kyle, Alida, Yaseen):
- Review their board
- Note items to discuss
- Check Waiting On for things you can unblock

**Before Wednesday 1:1s** (Elena/Ismaeel bi-weekly):
- Same prep
- Check for async updates since last meeting

**End of Week**:
- Move completed items to Done
- Quick scan of all boards for stale items

---

## Phase 7: Rollout Schedule

### Week 1

| Day | Action |
|-----|--------|
| Mon | Create Yaseen + Alida boards before 1:1s |
| Mon | Introduce boards in their 1:1s, seed initial tasks |
| Tue | Refine based on feedback |

### Week 2

| Day | Action |
|-----|--------|
| Mon | Create Kyle board before 1:1 |
| Mon | Introduce in Kyle's 1:1 |
| Wed | Create Elena or Ismaeel board (depending on cycle week) |
| Wed | Introduce in Medical Officer 1:1 |

### Week 3

| Day | Action |
|-----|--------|
| Wed | Create remaining Medical Officer board |
| Wed | Introduce in their 1:1 |
| Thu | All boards live - review overall approach |

### Week 4

| Day | Action |
|-----|--------|
| All | Full operation - refine workflows |
| Fri | Document what's working, what needs adjustment |

---

## Quick Reference: Section Mapping

| Work Type | Section |
|-----------|---------|
| Takes <30 min | Rapid Tasks |
| Must do this week | This Week |
| Actively working on | In Progress |
| Future work, prioritized | Backlog |
| Blocked on someone | Waiting On |
| Finished | Done |

---

## Troubleshooting

### "Board feels like micromanagement"
- Emphasize it's collaborative - they add items too
- Focus discussions on blockers, not status checks
- Give them ownership of their board updates

### "Too many sections"
- Consolidate if sections stay empty
- Start with standard 6, add custom only as needed

### "Items getting stale"
- Monthly cleanup ritual
- Delete or archive items older than 90 days with no activity

### "Duplication with other tools"
- This becomes the single source of truth for your working relationship
- Link to other tools (docs, Slack threads) from task comments
- Gradually migrate away from other tracking

---

## Templates for First Tasks

Seed each board with a few starter tasks during setup:

**All Boards**:
```
Task: Review and refine board sections
Section: This Week
Note: Decide if current sections serve our work well
```

```
Task: Identify 5 current priorities
Section: Backlog
Note: Brain dump current work, then prioritize
```

**Yaseen**:
```
Task: Document cross-location coordination needs
Section: Strategic Initiatives
```

**Alida**:
```
Task: Map monthly financial cycle tasks
Section: Monthly Cycle
```

**Kyle**:
```
Task: List outstanding facilities items
Section: Facilities
```

**Elena/Ismaeel**:
```
Task: Review nursing team performance/concerns
Section: Nursing Team
```

---

*Last Updated: 2026-01-23*
