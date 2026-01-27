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
└── plan/                 # Transition plan documents
    ├── 00-plan-index.md  # Start here for plan navigation
    └── summarised-views/ # Condensed responsibility summaries
```

## Key Context

- **Situation**: Financial Manager (Alida Wiese) resigned 26 Jan 2026, last day 23 Feb 2026
- **Scope**: 7 legal entities across UK and South Africa
- **Key people**: James La Porta (CEO), Grant Merwitz (MD), Yaseen Harneker (CPO), Kyle Bennett (Practice Mgr CPT), Amanda Ross (Practice Mgr UK), Ricardo Delgado (Director)
- **External support**: OCFO (consultancy - can provide CFO or bookkeeper), Inaura (SA accounting), Kinari (UK accounting)

## Critical Plan Decisions (Confirmed)

### Transition Approach
- **Phases 1 & 2 run concurrently** (not sequentially) - handover and operational work happen together
- **Alida's focus**: Should be on handover/training, not BAU work
- **Payment controls**: Bookkeeper loads payments → Grant or Yaseen releases (dual control maintained)
- **All stakeholders** receive proposed duties by end of Week 1

### Invoicing Rollout (Critical Workstream)

**Decentralized Model** - invoicing at point of service, not centrally:
| Role | Invoices | Responsibility |
|------|----------|----------------|
| Nurses | IVs, treatments, medications | Invoice at point of delivery |
| Reception | Consultations, supplements | Invoice and collect payment |
| Reception | Patient statement | Print at patient exit |
| Kyle/Amanda | Process ownership | Governance, training, compliance - *not execution* |

**Structure:**
| Role | Person | Responsibility |
|------|--------|----------------|
| Process Owner | Alida | Builds foundation Week 1, leads training Week 2 |
| Rollout Lead (CPT) | Kyle | Supports training Week 2, runs CPT team Weeks 3-4 |
| Rollout Lead (UK) | Amanda | Supports training Week 2, runs UK team Weeks 3-4 |

**Timeline:**
- **Week 1 (26 Jan - 1 Feb)**: Alida builds foundation - configure Xero, create billing manual (80%), brief Kyle & Amanda
- **Week 2 (3-7 Feb)**: Training (Alida leads, Kyle & Amanda support) → **GO LIVE Friday 7 Feb**
- **Week 3 (10-14 Feb)**: Kyle & Amanda run teams independently, Alida support only (~30% time)
- **Week 4 (17-23 Feb)**: Teams fully independent, Alida edge cases only (~10% time)
- **Result**: 12+ days live with expert support before Alida leaves 23 Feb

**Key principle**: CPT and UK go live **simultaneously** - not sequentially. Kyle and Amanda fulfill the same role in their respective locations.

**Three-Phase Billing Evolution:**
| Phase | Focus | Timing |
|-------|-------|--------|
| Phase 1: Survival/Simplify | Basic codes, laminated checklist, invoices presentable for medical aid | Go-live → stable (CURRENT FOCUS) |
| Phase 2: Optimise | Improve pricing, reduce missed charges, add audit rules | Post-departure |
| Phase 3: Interface/Automation | CRM integration, Xero API/marketplace apps | Future |

**Future improvement (Phase 2):** Billing baskets/bundles for common scenarios (e.g., infusion bundle) - must accommodate stock tracking, avoid confusion with advance-purchase bundles.

### OCFO Clarification
OCFO is a **consultancy** that can provide various services:
- Fractional CFO
- Bookkeeper for day-to-day operations
- Or both

Need to also engage an **accounting-focused agency** (not Optiworx) for urgent bookkeeper placement.

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
- **Bokelman transition**: Deferred until Phase 1 stable - not a priority during handover
- **New providers**: Avoid adding (e.g., Imperium) unless essential - focus on stabilizing existing relationships
- **Inaura**: Continues current obligations (VAT, payroll, PAYE, income tax) - no phase-out during transition

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

## Naming Conventions

- Use Kyle when referring to Cape Town operations (not "CPT lead")
- Use Amanda when referring to UK operations (not "UK lead")
- The location context is understood from their names

## Important Dates

| Date | Event |
|------|-------|
| 26 Jan 2026 | Alida's resignation date / transition start |
| 7 Feb 2026 | Target invoicing GO LIVE (end of Week 2) |
| 23 Feb 2026 | Alida's last day |
| 24 Feb onwards | Phase 3 - Transform (post-departure) |
