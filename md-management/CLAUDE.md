# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Maintenance Commands
- **"Reflect"**: When I use the word "Reflect" or "Update Docs", perform the following actions:
  1. Scan the `@business`, `@people`, `@planning`, `@projects`, `@resources` and `@tracking` directories to identify new folders or templates.
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
Team oversight and performance tracking:
- `team-roster.md` - All direct reports (6), extended team (18 indirect reports), 1:1 schedule, and team health indicators
- `hiring.md` - Open positions (Founders Associate), recruiting pipeline, and future hiring needs
- `google-drive-structure.md` - Reference for MD Google Drive folder structure with sharing permissions
- `direct-report-expectations.md` - General expectations for all direct reports: Attitude, Communication, Accountability, Continuous Improvement, Strategic Alignment

**Individual Performance Tracking** (`/people/performance/`):
- `TEMPLATE.md` - Template for creating new performance files
- `elena-hilton.md` - Dr Elena Hilton (Medical Officer, Cape Town)
- `ismaeel-ebrahim.md` - Dr Ismaeel Ebrahim (Medical Officer, London)
- `kyle-bennett.md` - Kyle Bennett (Practice Manager)
- `yaseen-harneker.md` - Yaseen Harneker (COO)
- `alida-wiese.md` - Alida Wiese (Finance Manager)

**When discussing people topics, always reference specific performance files and team roster data. Medical officers are UK-based (timezone considerations).**

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
Weekly execution, meeting structure, and decision tracking:

**Meeting Structure:**
- `meeting-structure.md` - Complete meeting framework with rationale, 60/30/10 MD/CTO/Innovation split, timezone considerations
- `MEETING-SCHEDULE-SUMMARY.md` - One-page quick reference of weekly schedule, 4-week cycle pattern, meeting roster

**Weekly Planning System:**
- `EXAMPLE-current-week.md` - Filled example showing how to write priorities, track meetings, and complete reviews
- `archive/` - Historical weekly plans (moved every Monday)

**Concepts & Templates** (`/planning/concepts/`):
*Ideas and templates that may or may not be adopted:*
- `weekly-template.md` - Blank template to copy each Monday for the week ahead
- `current-week.md` - Draft/template for this week's plan: top 3 priorities, meetings, focus blocks, decisions needed, end-of-week review
- `WEEKLY-USAGE-GUIDE.md` - Complete instructions for using the weekly planning system, meeting prep checklists, cycle week reference
- `decisions.md` - Template for tracking active decisions (pending), recent decisions (last 30 days), and major historical decisions with outcomes
- `work-board-strategy.md` - Asana work board strategy for each direct report: shared workspaces, section structures by role, operating principles, and 1:1 integration
- `asana-setup-guide.md` - Step-by-step Asana setup instructions: project creation, section configuration, custom fields by role, board views, and rollout schedule
- `asana-workboard-reference.md` - Quick reference for Asana work board configurations per direct report

**Setup & Utilities:**
- `meeting-setup-checklist.md` - Checklist for tracking calendar meeting setup progress (can be deleted once complete)
- `meeting-template.md` - Generic meeting notes template (date, attendees, agenda, actions) for Google Drive use

**Decision Tracking:**
- `concepts/decisions.md` - Active decisions (pending), recent decisions (last 30 days), and major historical decisions with outcomes

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
- **Friday**: Complete week-end review section in `current-week.md`, archive to `planning/archive/week-YYYY-MM-DD.md`, create MD progress log in `tracking/md-progress/weekly-logs/`
**Bi-Weekly**: Update performance files before Medical Officer 1:1s (Elena W1,3 / Ismaeel W2,4)
**Monthly**: Update metrics, refresh all performance files before scheduled 1:1s, review risks/opportunities
**Quarterly**: Update strategic sections in `business/overview.md`, conduct formal performance reviews, adjust org structure if needed
**Ad Hoc**: CEO feedback → `ceo-directives.md`, project changes → `active.md`, new risks → `risks.md`, decisions → `decisions.md`, post-1:1 → performance files with actions

### Meeting Rhythm (4-Week Cycle)
**Every Week**: Kyle (Mon), Alida (Mon), Yaseen (Tue), Amanda (Wed)
**Week 1 & 3**: Elena (Wed), Project Meeting (Thu), Ricardo if 1st/3rd Thu
**Week 2 & 4**: Ismaeel (Wed), Exco (Thu), CEO James (Thu), CFO if 2nd Thu, CMO if 4th Thu
**Monthly**: CFO (2nd Thu), CMO (4th Thu)
**Bi-Monthly**: Ricardo (1st & 3rd Thu)

### Key Workflows

**Weekly Planning (Every Monday, 10-15 minutes)**
1. Copy `planning/concepts/weekly-template.md` to `planning/current-week.md`
2. Fill in week dates and cycle week number (1, 2, 3, or 4) - determines which meetings occur
3. Read `business/ceo-directives.md` for current CEO priorities
4. Review `projects/active.md` for project health and blockers
5. Check `tracking/risks.md` for emerging issues
6. Review `people/team-roster.md` for scheduled 1:1s this week
7. Set top 3 priorities aligned to strategy with concrete success criteria
8. Prep meeting agendas for the week (direct reports send theirs 24h before)
9. Plan deep work blocks with specific focus areas

**Refer to `planning/concepts/WEEKLY-USAGE-GUIDE.md` for complete workflow and `planning/EXAMPLE-current-week.md` for reference.**

*Note: Templates live in `concepts/` folder. Active weekly plans should be `planning/current-week.md` (root).*

**Meeting Structure Understanding**
1. Refer to `planning/MEETING-SCHEDULE-SUMMARY.md` for quick weekly schedule reference
2. Understand 4-week cycle: Week 1 (light), Week 2 (heavy with CEO), Week 3 (light), Week 4 (heavy with CEO)
3. Monday = MD Day (6h deep work), Tuesday = CTO Day (7h deep work)
4. Wednesday = Medical Officers (bi-weekly alternating) + Innovation time (9-11am, no calendar)
5. Thursday = Project/Exco (alternating) + CEO (bi-weekly on Exco weeks) + Strategic partners (rotating)
6. Friday = Review & flex (no external meetings)
7. UK-based staff (Amanda, Ismaeel) meet at 11am+ SA time for timezone compatibility

**Decision Support**
1. Read relevant context files (`business/overview.md`, `ceo-directives.md`, `organization.md`)
2. Review related projects, risks, and metrics
3. Check `planning/concepts/decisions.md` for precedent decisions
4. Provide recommendation with clear rationale referencing business context
5. Document decision in `planning/concepts/decisions.md` once made

**People Management**
1. Read `people/team-roster.md` for team overview
2. Read specific `people/performance/[name].md` file for individual context
3. Review recent 1:1 notes and performance trends
4. Provide guidance considering team health, organizational constraints, and strategic priorities

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
1. Refer to `planning/concepts/work-board-strategy.md` for overall approach and per-person section structure
2. Use `planning/concepts/asana-setup-guide.md` for setup and configuration instructions
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
- **People**: Read team roster and individual performance files → prepare for 1:1s, identify issues
- **Projects**: Read active projects and strategic priorities → assess health, flag misalignment
- **Strategy**: Read business overview, CEO directives, metrics → assess alignment, surface drift

## File Naming Conventions

- Performance files: `people/performance/[firstname-lastname].md` (lowercase, hyphenated)
- Weekly plans: `planning/current-week.md` (active week)
- Weekly archives: `planning/archive/week-YYYY-MM-DD.md` (Monday date of that week)
- Project archives: `projects/archive/[project-name]-YYYY-MM-DD.md` (completion date)
- MD progress logs: `tracking/md-progress/weekly-logs/log-YYYY-MM-DD.md` (Monday date)
- CEO/board updates: `tracking/md-progress/communications/update-YYYY-MM-DD.md` (creation date)
- Always update "Last Updated: [Date]" footer in files when modified

## Key Business Context

**Organization**: Healthcare/medical practice with operations in Cape Town (South Africa) and London (UK)
**Team Size**: 28 staff + CEO + fractional CFO/CMO
**Direct Reports**: 6 (2 Medical Officers, 2 Practice Managers, 1 COO, 1 Finance Manager)
**Vacant Position**: Founders Associate (4 staff currently without proper management)
**Timezone**: South Africa (SAST) base; UK staff meet at 11am+ SAST (9am+ UK)
**Role Split**: Grant Merwitz as MD/CTO targeting 60% MD / 30% CTO / 10% Innovation
**Meeting Budget**: 5.5-7.5 hours/week (light weeks vs heavy weeks with CEO)
**Protected Time**: 22 hours/week deep work (11h MD, 9h CTO, 2h innovation)

## Initial Setup Flow

If files are empty/templated, guide user through `GETTING-STARTED.md` steps:
1. Fill `/business/` files (overview → organization → ceo-directives)
2. Document team in `/people/` (team-roster → hiring → individual performance files)
3. Capture work in `/projects/` (active → pipeline)
4. Document `/tracking/` (risks → opportunities → metrics)
5. Plan current week in `/planning/current-week.md`

## Common Requests

**"Help me plan this week"** → Check cycle week number → Read ceo-directives.md, active.md, risks.md, team-roster.md → Copy `concepts/weekly-template.md` to `current-week.md` with appropriate meetings for that cycle week
**"What meetings do I have this week?"** → Check cycle week (1-4) → Refer to MEETING-SCHEDULE-SUMMARY.md → List specific meetings for that cycle
**"Prep me for 1:1 with [Name]"** → Read performance/[name].md → summarize status, review last meeting actions, suggest discussion topics
**"Should we pursue [opportunity]?"** → Read overview.md, organization.md, active.md, risks.md, opportunities.md → assess fit and provide recommendation
**"What needs my attention?"** → Read active.md, risks.md, metrics.md → flag red/yellow status items
**"Are we aligned with strategy?"** → Read overview.md, ceo-directives.md, active.md → identify drift or misalignment
**"Show me my meeting schedule"** → Display MEETING-SCHEDULE-SUMMARY.md in readable format
**"Who reports to whom?"** → Reference organization.md or resources/Org Chart image
**"Help me set up work boards"** → Read `planning/concepts/work-board-strategy.md` and `planning/concepts/asana-setup-guide.md` → Guide through Asana project setup per direct report
**"How should Yaseen's board work?"** → Reference work-board-strategy.md → Explain Project as Custom Field model with Spotlight/Backlog/Waiting On/Done sections
**"Log my progress this week"** → Use md-progress-tracker agent → Create weekly log in `tracking/md-progress/weekly-logs/`
**"Draft a CEO update"** → Use md-progress-tracker agent → Create concise update in `tracking/md-progress/communications/`
**"What are my expectations for reports?"** → Read `people/direct-report-expectations.md` → Review the 5 expectations: Attitude, Communication, Accountability, Continuous Improvement, Strategic Alignment

## Git Usage

This repository tracks changes over time. Use git history to:
- Show how priorities have evolved
- Track decision outcomes vs. expectations
- Identify recurring patterns in risks or team issues
- Demonstrate progress on strategic initiatives

Commit messages should clearly describe what changed and why (e.g., "Update CEO directives with Q2 priorities" not "Update file").
