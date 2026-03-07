# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Maintenance Commands
- **"Reflect"**: When I use the word "Reflect" or "Update Docs", perform the following actions:
  1. Scan the `@business`, `@people`, `@planning` (including initiative folders), `@projects`, `@resources` and `@tracking` directories to identify new folders or templates.
  2. Compare what you find with the current descriptions in this file (`CLAUDE.md`).
  3. Update this file to include the new structures and suggest workflows based on the templates found.

## Repository Purpose

This is a **persistent management assistant system** for a Managing Director/Chief Technology Officer. The repository maintains business context, organizational data, strategic alignment, and operational tracking to support executive decision-making, planning, and execution.

**Critical**: This is NOT a software development repository. It's a structured knowledge base of markdown files tracking business operations, people management, and strategic planning.

## Core Architecture

The system is organized into six functional areas:

### 1. Business Context (`/business/`)
Foundational strategic information that informs all decision-making:
- `overview.md` - Company mission, vision, strategic priorities, targets, market context, and operational constraints
- `organization.md` - Org chart, reporting structure, dual MD/CTO role breakdown, and decision-making framework
- `ceo-directives.md` - CEO feedback, strategic guidance, action items, and alignment tracking

**These files provide essential context for all recommendations and must be reviewed before providing guidance.**

### 2. People Management (`/people/`)
Team oversight, performance tracking, and stakeholder management:
- `team-roster.md` - All direct reports (4), extended team, 1:1 schedule, and team health indicators
- `hiring.md` - Open positions (Founders Associate), recruiting pipeline, and future hiring needs
- `google-drive-structure.md` - Reference for MD Google Drive folder structure with sharing permissions
- `direct-report-expectations.md` - General expectations for all direct reports: Attitude, Communication, Accountability, Continuous Improvement, Strategic Alignment

**Inbox** (`/people/_inbox/`):
Drop zone for raw information about people. Files are named `YYYY-MM-DD-description.md` and processed into the correct location when user says "process inbox". See `_inbox/README.md` for full workflow.

**Direct Reports** (`/people/direct-reports/`):
Each direct report has their own folder with a consistent structure:
- `_TEMPLATE/` - Template folder to copy when adding a new direct report (`profile.md` + `performance.md` + `info-base.md`)
- `amanda-ross/` - Amanda Ross (London)
- `kyle-bennett/` - Kyle Bennett (Practice Manager)
- `yaseen-harneker/` - Yaseen Harneker (CPO)
- `ismaeel-ebrahim/` - Dr Ismaeel Ebrahim (Medical Officer, Cape Town)
- `ronald-mashonga/` - Ronald Mashonga

Each person's folder contains:
| File/Folder | Purpose |
|---|---|
| `profile.md` | Role, responsibilities, team managed, retention, development, goals |
| `performance.md` | Running log of date-stamped observations with category tags |
| `info-base.md` | Structured information base — compiled database of performance status, feedback register, task tracking, concerns/patterns, decisions, and context. Auto-maintained by inbox-processor agent. |
| `documents/` | Contracts, policies, legal/HR documents |
| `flash-reports/` | Weekly flash reports (`YYYY-MM-DD.md`, Friday date) |
| `one-on-ones/` | 1:1 meeting notes (`YYYY-MM-DD.md`, meeting date) |
| `updates/` | Generated summaries, review docs, job specs, role profiles, quarterly reports (`YYYY-MM-DD-description.md`) |

**Extended Team** (`/people/extended-team/`):
Employees the MD interacts with who don't report directly to them (skip-level reports, key employees in other teams):
- `_TEMPLATE/` - Template folder with `profile.md` + `info-base.md`
- `lexee-duval/` - Lexee Duval (Receptionist, London, reports to Amanda)
- Each person's folder contains: `profile.md`, `info-base.md`, `meetings/`, `updates/`

**Stakeholders** (`/people/stakeholders/`):
External stakeholders and senior leaders the MD works with (CEO, CFO, CMO, board members, external partners):
- `_TEMPLATE/` - Template folder with lighter `profile.md`
- Each stakeholder folder contains: `profile.md`, `meetings/`, `updates/`

**Ex-Employees** (`/people/ex-employees/`):
Former employees whose records are retained for reference:
- `alida-wiese/` - Alida Wiese (former Finance Manager)
- `elena-hilton/` - Dr Elena Hilton (former Medical Officer, Cape Town)

**When discussing people topics, always reference the specific person's folder. For direct reports, read `info-base.md` (structured current-state database) for quick context, `profile.md` (static role context), and `performance.md` (chronological source of truth). For extended team members, read `info-base.md` and `profile.md`.**

### 3. Project Tracking (`/projects/`)
Initiative management and execution status:
- `active.md` - Current projects with owners, status (🟢🟡🔴), health, milestones, blockers, and resources
- `pipeline.md` - Committed (next quarter), under evaluation, backlog, and declined/deferred projects
- `archive/` - Completed projects (moved from active)

**Cross-reference projects with strategic priorities in `business/overview.md` to ensure alignment.**

### 3a. Resources (`/resources/`)
Reference materials and organizational artifacts:
- `Org Chart - Proposed Org Chart 2025-12-15.jpg` - Visual organizational structure showing CEO, MD, direct reports, and all 28 staff members with locations (Cape Town, London, Global)

**Use this to understand reporting structure and team composition visually.**

### 4. Planning (`/planning/`)
Initiative-based planning system. Each initiative gets its own folder with an `info-base.md` tracker, supporting documents, ideas, and updates.

**Root Files:**
- `current-week.md` - Active weekly plan (copied from `weekly-planning/weekly-template.md` each Monday)
- `EXAMPLE-current-week.md` - Filled example showing how to write priorities, track meetings, and complete reviews
- `archive/` - Historical weekly plans (moved every Monday)

**Templates & Inbox:**
- `_TEMPLATE/` - Copy to create a new initiative folder (`info-base.md` + `supporting/` + `ideas/` + `updates/`)
- `_inbox/` - Drop zone for raw planning information, processed by planning-processor agent
  - `README.md` - Inbox workflow instructions
  - `_processed/` - Archived processed files

**Initiative Folders** (each contains `info-base.md` + `supporting/` + `ideas/` + `updates/`):

| Folder | Description | Key Files |
|--------|-------------|-----------|
| `meeting-structure/` | Meeting rhythm, calendar, 4-week cycle | `meeting-structure.md`, `MEETING-SCHEDULE-SUMMARY.md`, `meeting-setup-checklist.md`, `meeting-template.md` |
| `weekly-planning/` | Weekly planning system & templates | `weekly-template.md`, `WEEKLY-USAGE-GUIDE.md` |
| `work-boards/` | Asana work board system for direct reports | `work-board-strategy.md`, `asana-setup-guide.md`, `asana-workboard-reference.md` |
| `flash-reports/` | Weekly flash report system | `flash-report-template.md`, `updates/flash-report-rollout-email.md` |
| `decisions/` | Decision tracking & log | `decisions.md` |
| `presidents-list/` | CEO question management system | `presidents-list.md` |
| `nursing-roster/` | Nursing roster proposal | *(new initiative)* |
| `lead-management/` | Lead management & conversion | *(new initiative)* |
| `incentive-program/` | Employee incentive trial (March) | *(new initiative)* |

**Each initiative's `info-base.md` has 8 sections**: Status & Health, Purpose & Success Criteria, Key Decisions, Timeline & Milestones, Stakeholders & Adoption, Open Items & Actions, Feedback & Ideas, Patterns & Lessons Learned.

**When discussing planning initiatives, read the initiative's `info-base.md` for quick current-state context.**

**Weekly planning must align with CEO directives and strategic priorities. Meeting structure follows 4-week cycle with alternating bi-weekly patterns.**

### 5. Risk & Opportunity Tracking (`/tracking/`)
Ongoing monitoring and strategic evaluation:
- `risks.md` - Active risks by category (Financial/Operational/Strategic/Technical/People) with impact, likelihood, mitigation plans, and leading indicators
- `opportunities.md` - Active opportunities with potential value, effort required, strategic fit, and decision timelines
- `metrics.md` - Executive dashboard with financial, growth, product/technology, team, and operational efficiency KPIs

**MD Progress Tracking** (`/tracking/md-progress/`):
Personal progress tracking for the Managing Director role transition:
- `README.md` - System overview and weekly workflow
- `progress-tracker.md` - Cumulative timeline, wins log, and growth areas
- `weekly-logs/` - Weekly progress entries named `log-YYYY-MM-DD.md` (Monday date)
- `communications/` - CEO and board update drafts named `update-YYYY-MM-DD.md`

**Always consider risks and opportunities when making recommendations.**

### 6. Metrics & KPIs (`/tracking/metrics.md`)
Executive dashboard structure:
- Financial Health (Revenue, Burn Rate, Cash Runway, Gross Margin)
- Growth Metrics (New Customers, Retention, Churn, NPS)
- Product/Technology (Uptime, Performance, Release Frequency, Tech Debt)
- Team/People (Headcount, Attrition, Time to Hire, Engagement)
- Operational Efficiency (CAC, LTV/CAC, Sales Cycle, Support Volume)

## Operational Workflow

### Update Cadence
**Daily**: Review/update `current-week.md`, mark priority progress (🔴🟡🟢), update project status, capture decisions after meetings
**Weekly**:
- **Monday**: Copy `weekly-template.md` → `current-week.md`, set top 3 priorities, prep meeting agendas
- **Friday**: Complete week-end review section in `current-week.md`, archive to `planning/archive/week-YYYY-MM-DD.md`, create MD progress log in `tracking/md-progress/weekly-logs/`, review flash reports from direct reports (due 4pm)
**Bi-Weekly**: Update `direct-reports/[name]/performance.md` before Medical Officer 1:1s (Ismaeel W2,4)
**Monthly**: Update metrics, refresh all profile and performance files before scheduled 1:1s, review risks/opportunities
**Quarterly**: Update strategic sections in `business/overview.md`, conduct formal performance reviews, adjust org structure if needed
**Ad Hoc**: CEO feedback → `ceo-directives.md`, project changes → `active.md`, new risks → `risks.md`, decisions → `planning/decisions/decisions.md`, post-1:1 → `direct-reports/[name]/performance.md` and `one-on-ones/`, raw people notes → `people/_inbox/`, raw planning notes → `planning/_inbox/`

### Meeting Rhythm (4-Week Cycle)
**Every Week**: Kyle (Mon), Yaseen (Tue), Amanda (Wed)
**Week 1 & 3**: Project Meeting (Thu), Ricardo if 1st/3rd Thu
**Week 2 & 4**: Ismaeel (Wed), Exco (Thu), CEO James (Thu), CFO if 2nd Thu, CMO if 4th Thu
**Monthly**: CFO (2nd Thu), CMO (4th Thu)
**Bi-Monthly**: Ricardo (1st & 3rd Thu)

### Key Workflows

**Weekly Planning (Every Monday, 10-15 minutes)**
1. Copy `planning/weekly-planning/weekly-template.md` to `planning/current-week.md`
2. Fill in week dates and cycle week number (1, 2, 3, or 4) - determines which meetings occur
3. Read `business/ceo-directives.md` for current CEO priorities
4. Review `projects/active.md` for project health and blockers
5. Check `tracking/risks.md` for emerging issues
6. Review `people/team-roster.md` for scheduled 1:1s this week
7. Set top 3 priorities aligned to strategy with concrete success criteria
8. Prep meeting agendas for the week (direct reports send theirs 24h before)
9. Plan deep work blocks with specific focus areas

**Refer to `planning/weekly-planning/WEEKLY-USAGE-GUIDE.md` for complete workflow and `planning/EXAMPLE-current-week.md` for reference.**

**Meeting Structure Understanding**
1. Refer to `planning/meeting-structure/MEETING-SCHEDULE-SUMMARY.md` for quick weekly schedule reference
2. Understand 4-week cycle: Week 1 (light), Week 2 (heavy with CEO), Week 3 (light), Week 4 (heavy with CEO)
3. Monday = MD Day (6h deep work), Tuesday = CTO Day (7h deep work)
4. Wednesday = Medical Officers (bi-weekly alternating) + Innovation time (9-11am, no calendar)
5. Thursday = Project/Exco (alternating) + CEO (bi-weekly on Exco weeks) + Strategic partners (rotating)
6. Friday = Review & flex (no external meetings)
7. UK-based staff (Amanda, Ismaeel) meet at 11am+ SAST for timezone compatibility

**Decision Support**
1. Read relevant context files (`business/overview.md`, `ceo-directives.md`, `organization.md`)
2. Review related projects, risks, and metrics
3. Check `planning/decisions/decisions.md` for precedent decisions
4. Provide recommendation with clear rationale referencing business context
5. Document decision in `planning/decisions/decisions.md` once made

**People Management**
1. Read `people/team-roster.md` for team overview
2. Read `people/direct-reports/[name]/info-base.md` for structured current-state database (quick scan of status, concerns, feedback, tasks)
3. Read `people/direct-reports/[name]/profile.md` for role context, development, and goals
4. Read `people/direct-reports/[name]/performance.md` for full chronological observation history
5. Review recent 1:1 notes in `people/direct-reports/[name]/one-on-ones/`
6. Check latest flash reports in `people/direct-reports/[name]/flash-reports/`
7. Provide guidance considering team health, organizational constraints, and strategic priorities

**Process Inbox** (Route raw people information — uses `inbox-processor` sub-agent)
Use the `inbox-processor` agent (`.claude/agents/inbox-processor.md`) which handles the full workflow:
1. Scan `people/_inbox/` for unprocessed files (skip README.md and `_processed/`)
2. Classify content by person and type (observation, achievement, concern, feedback, meeting notes, flash report, task, decision, etc.)
3. Route content to correct destinations:
   - Performance observations/feedback → append to `people/direct-reports/[name]/performance.md` with appropriate tags
   - Meeting notes → create file in `one-on-ones/` or `stakeholders/[name]/meetings/`
   - Flash report content → create file in `flash-reports/`
   - Documents/contracts → note in profile or place in `documents/`
   - Tasks/decisions/context → update `info-base.md` directly
   - New person → create folder from appropriate `_TEMPLATE/`
4. Update each person's `info-base.md` with compiled/structured data from processed content
5. Move processed files to `people/_inbox/_processed/` with routing comment
6. Output structured summary to user (files processed, destinations, urgent flags, questions)

**Process Planning Inbox** (Route raw planning information — uses `planning-processor` sub-agent)
Use the `planning-processor` agent (`.claude/agents/planning-processor.md`) which handles two modes:
1. **Inbox scan**: Scan `planning/_inbox/` for unprocessed files, identify which initiative each relates to, route content to correct initiative folder (info-base updates, supporting docs, ideas, updates), move processed files to `_inbox/_processed/`, output summary
2. **Conversational**: User tells the agent what happened, agent identifies the initiative, classifies content, updates the correct `info-base.md` sections, and confirms
- New initiatives → create folder from `planning/_TEMPLATE/`
- Status/blocker changes → info-base Section 1
- Decisions → info-base Section 3
- Timeline changes → info-base Section 4
- Action items → info-base Section 6
- Feedback/ideas → info-base Section 7
- Formal communications → `updates/YYYY-MM-DD-description.md`
- Reference material → `supporting/`

**Project Oversight**
1. Read all `projects/active.md` to assess portfolio health
2. Cross-reference with `business/overview.md` strategic priorities
3. Check resource allocation against `people/team-roster.md`
4. Flag projects with 🔴 status or misalignment with strategy
5. Surface cross-project dependencies and resource conflicts

**Risk Management**
1. Review `tracking/risks.md` for all active risks
2. Check leading indicators mentioned in risk entries
3. Review related metrics in `tracking/metrics.md`
4. Flag risks with increasing likelihood or impact
5. Assess mitigation plan progress

**Work Board Management** (Asana-based direct report tracking)
1. Refer to `planning/work-boards/work-board-strategy.md` for overall approach and per-person section structure
2. Use `planning/work-boards/asana-setup-guide.md` for setup and configuration instructions
3. Each direct report has their own work board with role-specific sections
4. Yaseen (CPO) uses "Project as Custom Field" model: 4 sections (Spotlight, Backlog, Waiting On, Done) with Project dropdown for filtering
5. Other reports use domain-specific sections (e.g., Alida: Monthly Cycle, CFO Coordination; Kyle: Facilities, Reception)
6. Review work boards before 1:1s to identify blockers and priorities

**MD Progress Tracking** (Personal role transition tracking)
1. Each Friday, create weekly log in `tracking/md-progress/weekly-logs/log-YYYY-MM-DD.md` (Monday date)
2. List MD progress items as brief bullets
3. List CTO progress items if relevant
4. Update `tracking/md-progress/progress-tracker.md` with key wins
5. When needed, draft CEO updates in `tracking/md-progress/communications/`
6. Keep entries concise and factual - not over-elaborated

**Flash Reports** (Weekly direct report updates)
1. Direct reports submit flash reports every Friday by 4pm (local time)
2. Format: accomplishments, challenges/blockers, next week's focus, asks
3. Review over weekend before Monday 1:1s (Kyle, Alida)
4. Reference specific items in 1:1s to reinforce value
5. Look for patterns across reports (common blockers, resource conflicts)
6. Respond immediately if urgent blockers flagged
7. Template and guidance in `planning/flash-reports/flash-report-template.md`

## Assistant Behavior Guidelines

### Context-First Approach
**Always read relevant context files before providing recommendations.** This is a knowledge base, not a code repository. The user expects you to:
- Understand their full business situation
- Reference specific data from the files
- Maintain strategic alignment across all guidance
- Surface patterns and insights from historical data (use git history)

### Executive-Level Communication
- Provide clear, pragmatic, actionable guidance
- Focus on strategic impact and trade-offs
- Surface risks and opportunities proactively
- Be direct about misalignments or concerns
- Reference specific file locations when citing data (e.g., "based on `business/overview.md`")

### Data Integrity
- Keep information current and accurate
- Archive historical data (weekly plans → `planning/archive/`, completed projects → `projects/archive/`)
- Use git commits to track evolution
- Maintain consistency across related files (e.g., project owner must exist in `team-roster.md`)

### Proactive Support
When user asks about:
- **Planning**: Read CEO directives, active projects, risks, team roster → suggest weekly priorities
- **Decisions**: Read business context, related projects/risks → provide recommendation with rationale
- **People**: Read team roster, direct-reports profiles and performance logs → prepare for 1:1s, identify issues
- **Projects**: Read active projects and strategic priorities → assess health, flag misalignment
- **Strategy**: Read business overview, CEO directives, metrics → assess alignment, surface drift

## File Naming Conventions

- Direct report folders: `people/direct-reports/[firstname-lastname]/` (lowercase, hyphenated)
- Direct report profiles: `people/direct-reports/[name]/profile.md`
- Direct report performance logs: `people/direct-reports/[name]/performance.md`
- 1:1 meeting notes: `people/direct-reports/[name]/one-on-ones/YYYY-MM-DD.md` (meeting date)
- Flash reports: `people/direct-reports/[name]/flash-reports/YYYY-MM-DD.md` (Friday date)
- Stakeholder folders: `people/stakeholders/[firstname-lastname]/`
- People inbox files: `people/_inbox/YYYY-MM-DD-description.md`
- Planning inbox files: `planning/_inbox/YYYY-MM-DD-description.md`
- Planning initiative folders: `planning/[initiative-name]/` (lowercase, hyphenated)
- Weekly plans: `planning/current-week.md` (active week)
- Weekly archives: `planning/archive/week-YYYY-MM-DD.md` (Monday date of that week)
- Project archives: `projects/archive/[project-name]-YYYY-MM-DD.md` (completion date)
- MD progress logs: `tracking/md-progress/weekly-logs/log-YYYY-MM-DD.md` (Monday date)
- CEO/board updates: `tracking/md-progress/communications/update-YYYY-MM-DD.md` (creation date)
- Always update "Last Updated: [Date]" footer in files when modified

## Key Business Context

**Organization**: Healthcare/medical practice with operations in Cape Town (South Africa) and London (UK)
**Team Size**: 28 staff + CEO + fractional CFO/CMO
**Direct Reports**: 4 (1 Medical Officer, 1 Practice Manager, 1 CPO, 1 Practice Manager London)
**Vacant Position**: Founders Associate (4 staff currently without proper management)
**Timezone**: South Africa (SAST) base; UK staff meet at 11am+ SAST (9am+ UK)
**Role Split**: Grant Merwitz as MD/CTO targeting 60% MD / 30% CTO / 10% Innovation
**Meeting Budget**: 5.5-7.5 hours/week (light weeks vs heavy weeks with CEO)
**Protected Time**: 22 hours/week deep work (11h MD, 9h CTO, 2h innovation)

## Initial Setup Flow

If files are empty/templated, guide user through `GETTING-STARTED.md` steps:
1. Fill `/business/` files (overview → organization → ceo-directives)
2. Document team in `/people/` (team-roster → hiring → direct-reports profiles and performance logs)
3. Capture work in `/projects/` (active → pipeline)
4. Document `/tracking/` (risks → opportunities → metrics)
5. Plan current week in `/planning/current-week.md`

## Common Requests

**"Help me plan this week"** → Check cycle week number → Read ceo-directives.md, active.md, risks.md, team-roster.md → Copy `weekly-planning/weekly-template.md` to `current-week.md` with appropriate meetings for that cycle week
**"What meetings do I have this week?"** → Check cycle week (1-4) → Refer to `meeting-structure/MEETING-SCHEDULE-SUMMARY.md` → List specific meetings for that cycle
**"Prep me for 1:1 with [Name]"** → Read `direct-reports/[name]/info-base.md` (quick current-state view) + `profile.md` + `performance.md` → check latest `one-on-ones/` and `flash-reports/` → summarize status, review last meeting actions, suggest discussion topics
**"Process inbox"** → Use inbox-processor agent → classify, route content, update info-bases, archive processed files, output summary
**"Should we pursue [opportunity]?"** → Read overview.md, organization.md, active.md, risks.md, opportunities.md → assess fit and provide recommendation
**"What needs my attention?"** → Read active.md, risks.md, metrics.md → flag red/yellow status items
**"Are we aligned with strategy?"** → Read overview.md, ceo-directives.md, active.md → identify drift or misalignment
**"Show me my meeting schedule"** → Display MEETING-SCHEDULE-SUMMARY.md in readable format
**"Who reports to whom?"** → Reference organization.md or resources/Org Chart image
**"Help me set up work boards"** → Read `planning/work-boards/work-board-strategy.md` and `planning/work-boards/asana-setup-guide.md` → Guide through Asana project setup per direct report
**"How should Yaseen's board work?"** → Reference `planning/work-boards/work-board-strategy.md` → Explain Project as Custom Field model with Spotlight/Backlog/Waiting On/Done sections
**"Log my progress this week"** → Use md-progress-tracker agent → Create weekly log in `tracking/md-progress/weekly-logs/`
**"Draft a CEO update"** → Use md-progress-tracker agent → Create concise update in `tracking/md-progress/communications/`
**"What are my expectations for reports?"** → Read `people/direct-report-expectations.md` → Review the 5 expectations: Attitude, Communication, Accountability, Continuous Improvement, Strategic Alignment
**"Set up flash reports"** → Read `planning/flash-reports/flash-report-template.md` and `planning/flash-reports/updates/flash-report-rollout-email.md` → Guide through sending rollout email to direct reports
**"What's the status on [Name]?"** → Read `direct-reports/[name]/info-base.md` → Scan performance status, active concerns, recent wins, open tasks, and feedback register
**"Show me [Name]'s information base"** → Read and display `direct-reports/[name]/info-base.md` — structured current-state database
**"Process planning inbox"** → Use planning-processor agent → scan `planning/_inbox/`, route to initiatives, update info-bases, archive, output summary
**"What's the status of [initiative]?"** → Read `planning/[initiative]/info-base.md` → Scan status, blockers, next milestone, open items
**"Show me all initiatives"** → List all folders in `planning/` with their info-base quick status lines
**"Create a new initiative"** → Copy `planning/_TEMPLATE/` to `planning/[name]/` → Populate info-base.md with initial information

## Git Usage

This repository tracks changes over time. Use git history to:
- Show how priorities have evolved
- Track decision outcomes vs. expectations
- Identify recurring patterns in risks or team issues
- Demonstrate progress on strategic initiatives

Commit messages should clearly describe what changed and why (e.g., "Update CEO directives with Q2 priorities" not "Update file").
