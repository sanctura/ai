# The President's List

A structured process for managing questions, decisions, and requests that require CEO input.

## The Problem

Dr James Laporta is both CEO and Lead Medical Director. His current system requires people to keep asking him questions repeatedly until they get an answer — he sits reassured knowing nothing will slip through because people will always follow up.

The reality for everyone else:
- Staff must chase James indefinitely for answers, creating frustration and inefficiency
- James is overwhelmed by a constant stream of unstructured questions from multiple people and channels
- There's no visibility into what's been asked, what's pending, or what's been answered
- Priority items sit alongside trivial requests with no way to triage
- The same question may be asked by multiple people without anyone knowing

## The Solution: President's List

A single, maintained register of all outstanding questions and requests for the CEO — organized by location, categorized, and prioritized by the team before being sent to James.

### How It Works

1. **Staff log questions** — Instead of messaging James directly, staff add their question to the President's List with their name, the category, and any context needed
2. **Team prioritizes** — Each location's team agrees on what matters most, ranking items so James sees priority first
3. **Daily digest sent** — The outstanding list is sent to James daily via WhatsApp and email — one consolidated view instead of scattered messages
4. **James responds at his pace** — He can answer in priority order, cherry-pick what he can address quickly, or flag items that need a meeting
5. **Answers linked back** — When James responds, the answer is recorded against the question and the item is closed
6. **List is maintained** — Answered items are archived, stale items are reviewed, and the list stays current

### Two Lists, One Process

| List | Owner | Coverage |
|------|-------|----------|
| **UK President's List** | Amanda Ross | London clinic staff questions |
| **Cape Town President's List** | Kyle Bennett | Cape Town clinic staff questions |

The list owner is responsible for:
- Collecting and logging new questions from their team
- Facilitating priority discussions with staff
- Sending the daily digest to James
- Recording James's answers and updating the list
- Escalating truly urgent items through the normal channel (direct call/message)

### Question Categories

| Category | Covers | Examples |
|----------|--------|----------|
| **Clinical** | Patient-related matters | Treatment protocols, patient care decisions, medical equipment, clinical procedures, medication queries |
| **Operational** | Office, admin, people, and everything else | Facility decisions, supplier approvals, hiring, process changes, IT, systems, spend approvals, strategy |

### Priority Levels

| Priority | Meaning | Expected Response |
|----------|---------|-------------------|
| **Urgent** | Blocking patient care or revenue — needs answer today | Same day |
| **High** | Blocking a project or person — needs answer this week | Within 2-3 days |
| **Medium** | Important but not blocking — needs answer soon | Within 1 week |
| **Low** | Nice to know / future planning | When convenient |

> **Note**: Truly urgent clinical/patient care matters should still go directly to James — the President's List is not a replacement for emergency escalation.

### List Format

Each entry on the list should capture:

| Field | Description |
|-------|-------------|
| **#** | Sequential number for easy reference |
| **Date Added** | When the question was logged |
| **Asked By** | Who needs the answer |
| **Category** | Clinical / Operational |
| **Priority** | Urgent / High / Medium / Low |
| **Question** | The actual question, written clearly with enough context for James to answer |
| **Status** | Open / Answered / Escalated / Withdrawn |
| **Answer** | James's response (when provided) |
| **Date Answered** | When the response was received |

### Daily Digest Format

The daily WhatsApp/email to James should follow this structure:

```
President's List — [UK / Cape Town] — [Date]

URGENT (need answer today):
  #12 — [Question summary] (Asked by: [Name], [Date])

HIGH PRIORITY:
  #8 — [Question summary] (Asked by: [Name], [Date])
  #11 — [Question summary] (Asked by: [Name], [Date])

MEDIUM:
  #3 — [Question summary] (Asked by: [Name], [Date])
  #5 — [Question summary] (Asked by: [Name], [Date])

LOW:
  #1 — [Question summary] (Asked by: [Name], [Date])

Total outstanding: [X] questions ([Y] new today)
```

### Where to Maintain the List

Each clinic gets its own **Asana board** — consistent with the existing work board strategy for direct reports.

| Board | Owner | Asana Project Name (suggested) |
|-------|-------|-------------------------------|
| **UK President's List** | Amanda Ross | `President's List — UK` |
| **Cape Town President's List** | Kyle Bennett | `President's List — Cape Town` |

**Board Structure:**

Sections (columns in board view):
1. **New** — Freshly logged questions, not yet prioritized
2. **Prioritized** — Team has agreed on priority, awaiting James's response
3. **Answered** — James has responded, answer recorded on the task
4. **Escalated** — Needs a meeting or deeper discussion

**Custom Fields:**
- **Category**: Clinical / Operational (dropdown)
- **Priority**: Urgent / High / Medium / Low (dropdown)
- **Asked By**: Text field (staff member's name)

Each question is an Asana task. The task description contains the full question and context. When James answers, the answer is added as a comment or in a dedicated "Answer" field, and the task moves to Answered.

The daily digest is generated from the **New** and **Prioritized** sections and sent to James via WhatsApp and email.

## Rollout Plan

### Phase 1: Setup (Week 1)
- [ ] Create Asana project: `President's List — UK` (owner: Amanda)
- [ ] Create Asana project: `President's List — Cape Town` (owner: Kyle)
- [ ] Configure sections (New, Prioritized, Answered, Escalated) and custom fields (Category, Priority, Asked By)
- [ ] Brief Amanda and Kyle on their role as list owners

### Phase 2: Communicate (Week 1-2)
- [ ] Explain the process to James — frame as: "We're making your life easier by consolidating everything into one daily digest you can work through"
- [ ] Brief all staff at both locations — questions go to list owner, not directly to James (unless truly urgent/clinical)
- [ ] Set up daily digest schedule (suggest: sent by 9am each morning)

### Phase 3: Operate (Week 2+)
- [ ] List owners collect questions daily
- [ ] Staff discuss priorities (can be quick — start of day or team chat)
- [ ] Daily digest sent to James
- [ ] Answers recorded same day when received
- [ ] Weekly review: stale items flagged, patterns noted

### Phase 4: Review (Week 4)
- [ ] Assess: Is James responding? Are items getting resolved faster?
- [ ] Adjust frequency if needed (daily may be too much — could move to 2-3x/week)
- [ ] Identify categories where James could delegate decision authority
- [ ] Consider: Can some categories be answered by Grant (MD) instead?

## Benefits

**For James:**
- One consolidated view instead of constant interruptions
- Can batch-process answers efficiently
- Priority items surfaced — no risk of missing what matters
- Still gets everything asked — just structured

**For Staff:**
- No more chasing — the system chases for them
- Visibility into where their question sits in the queue
- Peer-prioritization means genuinely urgent items rise to the top
- Clear answers recorded and accessible

**For Grant (MD):**
- Visibility into what the business needs from the CEO
- Can identify items Grant can answer directly (reducing James's load)
- Pattern recognition — recurring question categories may signal delegation opportunities or process gaps
- Evidence base for conversations about decision-making speed

## Long-Term Opportunity

Over time, the President's List becomes a dataset that reveals:
- Which categories generate the most questions (delegation opportunity)
- Average response times by category (bottleneck identification)
- Which questions could be pre-answered with SOPs or policies
- Whether certain staff need more authority to make decisions independently

This can inform a gradual shift from "ask James everything" to "James decides on X, Grant decides on Y, managers decide on Z" — a proper decision-rights framework.

---

*Concept created: 2026-02-18*
*Status: Draft — needs review and CEO buy-in before rollout*
