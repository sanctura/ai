# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Purpose

This repository is a **documentation and planning repository** (not a codebase) for managing a financial manager transition at Sanctura. It contains no source code, tests, or build processes.

## Repository Structure

```
accounting-handover/
├── background/           # Source materials and raw inputs
│   ├── *.txt             # Meeting transcripts, notes, CEO thinking
│   └── invoice-plan/     # Pre-existing invoicing transformation project docs
├── information-base/     # Structured reference documentation
│   └── 00-index.md       # Start here for information base navigation
├── plan/                 # Transition plan documents
│   ├── 00-plan-index.md  # Start here for plan navigation
│   └── summarised-views/ # Condensed responsibility summaries
├── tasks/                # Asana-style task tracking
│   ├── 01-invoicing-transformation.md
│   ├── 02-non-invoicing-handover.md
│   ├── 03-contact-handover-checklist.md
│   └── 04-responsibility-handover-checklist.md
├── ronald-guide/         # Handover documentation package for Ronald Mushonga
│   ├── 00-welcome-letter.md
│   ├── 01-your-first-week.md
│   ├── 02-your-role-and-expectations.md
│   ├── 03-the-business.md
│   ├── 04-the-people.md
│   ├── 05-how-money-flows.md
│   ├── 06-systems-and-access.md
│   ├── 07-service-providers.md
│   ├── 08-whats-happening-now.md
│   ├── 09-compliance-calendar.md
│   └── 10-key-processes.md
├── output/               # Generated deliverables (SOW, emails, etc.)
└── new-information/      # Newly discovered items to incorporate
    └── overlooked-items.md
```

## Key Context

- **Situation**: Financial Manager (Alida Wiese) resigned 26 Jan 2026, last day 23 Feb 2026
- **Scope**: 7 legal entities across UK and South Africa
- **Key people**: James La Porta (CEO), Grant Merwitz (MD), Yaseen Harneker (CPO), Kyle Bennett (Practice Mgr CPT), Amanda Ross (Practice Mgr UK), Ricardo Delgado (Director)
- **Replacement resource**: Ronald Mushonga (via Clearshell Management Solutions) - Fractional CFO, 40hrs/week, 9 Feb - 9 Jun 2026
- **External support**: Inaura (SA accounting - being transitioned to Bokelman or equivalent), Kinari / Capricorn Capital Services (UK accounting)

## Critical Plan Decisions (Confirmed)

### Transition Approach
- **Phases 1 & 2 run concurrently** (not sequentially) - handover and operational work happen together
- **Alida's focus**: Should be on handover/training, not BAU work
- **Payment controls**: Ronald prepares payment schedules → Grant loads into Investec (Ronald has no banking access) → Grant or Yaseen releases non-SARS; James releases SARS only
- **All stakeholders** receive proposed duties by end of Week 1

### Invoicing & Quoting Rollout (Critical Workstream)

**Xero Live:** 28 Jan 2026

**Decentralized Model** - invoicing and quoting at point of service, not centrally:
| Role | Invoices | Responsibility |
|------|----------|----------------|
| Nurses | IVs, treatments, medications | Invoice at point of delivery |
| Reception | Consultations, supplements | Invoice and collect payment |
| Reception | Patient statement | Print at patient exit |
| Kyle/Amanda | Process ownership | Governance, training, compliance - *not execution* |

**Structure:**
| Role | Person | Responsibility |
|------|--------|----------------|
| Process Owner | Alida | Xero live Week 1, leads training Week 2 |
| Rollout Lead (CPT) | Kyle | Supports training Week 2, runs CPT team Weeks 3-4 |
| Rollout Lead (UK) | Amanda | Supports training Week 2, runs UK team Weeks 3-4 |

**Timeline:**
- **Week 1 (26 Jan - 1 Feb)**: Xero live (28 Jan), billing/quoting manual (80%), brief Kyle & Amanda
- **Week 2 (3-7 Feb)**: Training (Alida leads, Kyle & Amanda support), staff ready for independent operation
- **Week 3 (10-14 Feb)**: Kyle & Amanda run teams independently, Alida support only (~30% time)
- **Week 4 (17-23 Feb)**: Teams fully independent, Alida edge cases only (~10% time)
- **Result**: System live from Week 1, teams trained and independent before Alida leaves 23 Feb

**Key principle**: CPT and UK go live **simultaneously** - not sequentially. Kyle and Amanda fulfill the same role in their respective locations.

**Three-Phase Billing & Quoting Evolution:**
| Phase | Focus | Timing |
|-------|-------|--------|
| Phase 1: Survival/Simplify | Basic codes, laminated checklist, invoices presentable for medical aid | Go-live → stable (CURRENT FOCUS) |
| Phase 2: Optimise | Improve pricing, reduce missed charges, add audit rules | Post-departure |
| Phase 3: Interface/Automation | CRM integration, Xero API/marketplace apps | Future |

**Future improvement (Phase 2):** Billing/quoting baskets/bundles for common scenarios (e.g., infusion bundle) - must accommodate stock tracking, avoid confusion with advance-purchase bundles.

### Replacement Resource (Confirmed)
- **Who**: Ronald Mushonga, engaged via Clearshell Management Solutions (Pty) Ltd
- **Title**: Fractional CFO
- **Contract**: 9 February 2026 - 9 June 2026, 40 hours/week
- **Reports to**: Grant Merwitz (MD)
- **Access limitations**: No Investec banking access (cannot load or release payments)
- **External provider contact**: Must liaise with Grant before initiating any direct contact with service providers
- **SOW**: See `output/sow-ronald-mushonga-revised.md`
- **Xero scope**: 2 SA organisations (Saint Raphael, Dr James La Porta Inc) + 1 UK organisation (Sanctura Limited)
- **Management accounts**: By 7th working day of each month (goal: ASAP after month-end)
- **Payroll data**: Provides to Inaura (SA) and Capricorn Capital Services / Kinari (UK)

### Debt Collection Escalation
| Stage | Owner | Scenario |
|-------|-------|----------|
| Initial contact | OCFO | Pull debtors list, communicate with debtors |
| Product/service dispute | Kyle (SA) / Amanda (UK) | "I didn't receive this" - investigate |
| Service explanation | Doctor | "What is this charge?" - explain clinical service |
| Debt support/hardship | Exco | Review and decide on payment arrangements |

### Supplier Invoice Management
Key workstream - workflow: Receive → Log → Reconcile to PO → Approve → Schedule payment → Monthly review. OCFO responsible, Kyle/Amanda consulted on reconciliation.

### Provider Decisions
- **Bokelman transition**: Active deliverable - Ronald to facilitate transition from Inaura and current providers to Bokelman or equivalent (Phase 2-3 of his contract)
- **Inaura**: Continues current obligations during transition period, but planned phase-out to Bokelman or equivalent
- **Kinari / Capricorn Capital Services**: Continues UK operations; receives payroll data from Ronald

### Open Questions (from CEO review)
| Question | Owner | By When |
|----------|-------|---------|
| UBO submissions - who owns, when next due? | Grant | TBD |
| Supplier invoice destination - which mailbox? | Grant + Alida | Week 1 |
| Pricing source of truth - MedPrax vs Xero? | Grant + Alida | Week 2 |
| Facility fee rules - when does >2 hour rule apply? | Alida | Week 2 |

## Key Documents

| Document | Purpose |
|----------|---------|
| `plan/01-executive-summary.md` | High-level overview for leadership |
| `plan/04-responsibility-matrix.md` | RACI matrix, debt collection escalation, supplier invoice workflow |
| `plan/05-key-decisions.md` | Decisions tracker and open questions |
| `plan/08-invoicing-rollout-integration.md` | Detailed invoicing rollout plan |
| `plan/06-handover-checklists.md` | Tracking checklists with sign-off |
| `plan/summarised-views/` | Condensed responsibility summaries for quick reference |
| `information-base/08-people-and-team.md` | Roles, capacity, and responsibilities |
| `tasks/01-invoicing-transformation.md` | Task tracking for invoicing & quoting rollout |
| `tasks/02-non-invoicing-handover.md` | Task tracking for all other handover activities |
| `tasks/03-contact-handover-checklist.md` | Service providers & contacts to hand over |
| `tasks/04-responsibility-handover-checklist.md` | All responsibilities & where they're going |
| `new-information/overlooked-items.md` | Log of newly discovered items to incorporate |
| `output/sow-ronald-mushonga-revised.md` | Revised Statement of Work for Ronald Mushonga (Fractional CFO) |
| `ronald-guide/` | Complete handover documentation package for Ronald (welcome letter, first week guide, business overview, people, processes, compliance) |

## Working With This Repository

When asked to update or extend documentation:
1. Check the relevant index file (`information-base/00-index.md` or `plan/00-plan-index.md`) for structure
2. Maintain consistent formatting with existing documents
3. Update index files when adding new documents
4. Cross-reference related documents where appropriate

When asked about the transition:
1. Reference `information-base/01-situation-overview.md` for context
2. Reference `plan/01-executive-summary.md` for the plan overview
3. Reference `plan/08-invoicing-rollout-integration.md` for invoicing details
4. Reference `information-base/08-people-and-team.md` for roles and responsibilities
5. Reference `tasks/01-invoicing-transformation.md` for invoicing & quoting tasks
6. Reference `tasks/02-non-invoicing-handover.md` for all other handover tasks

When asked about Ronald's onboarding or handover:
1. Reference `ronald-guide/` for the complete handover package
2. Reference `output/sow-ronald-mushonga-revised.md` for his Statement of Work
3. Reference `ronald-guide/01-your-first-week.md` for his day-by-day plan
4. Reference `ronald-guide/08-whats-happening-now.md` for current state of play

When tracking tasks:
- `tasks/` contains Asana-style task lists with checkboxes
- Mark tasks complete by changing `[ ]` to `[x]`
- Add new task files as `##-workstream-name.md`

When discovering overlooked items:
- Add to `new-information/overlooked-items.md` with date and checkbox
- Once incorporated into the plan, check the box

## Naming Conventions

- Use Kyle when referring to Cape Town operations (not "CPT lead")
- Use Amanda when referring to UK operations (not "UK lead")
- The location context is understood from their names

## Important Dates

| Date | Event |
|------|-------|
| 26 Jan 2026 | Alida's resignation date / transition start |
| 28 Jan 2026 | Xero live for invoicing & quoting |
| 7 Feb 2026 | End of Week 2 - staff ready for independent operation |
| 23 Feb 2026 | Alida's last day |
| 9 Feb 2026 | Ronald Mushonga (Fractional CFO) starts |
| 24 Feb onwards | Phase 3 - Transform (post-departure) |
| 9 Jun 2026 | Ronald's contract end date |
