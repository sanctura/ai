# Invoicing Transformation Project

## Project Overview

A strategic initiative was already underway to fundamentally change how Sanctura handles patient invoicing. This project is directly relevant to the financial manager transition.

### The Change

Moving from **retrospective billing** (Alida invoices after service) to **real-time, upfront-aligned billing** (staff invoice at point of service).

### Strategic Relevance to Transition

This project was designed to:
1. **Remove invoicing dependency** on a central finance person
2. **Distribute invoicing** to nurses and reception at point of delivery
3. **Shift bookkeeper role** from creating invoices to auditing/oversight
4. **Reduce revenue leakage** from services delivered but not invoiced

**Key Insight:** If implemented, this project directly addresses one of the highest-risk areas of Alida's departure - patient invoicing operations.

---

## Current State Problems (Why This Project Exists)

| Problem | Impact |
|---------|--------|
| Revenue leakage | Services delivered but never invoiced |
| Administrative burden | Staff time spent chasing payments |
| Reconciliation complexity | Difficult to match services to payments |
| Patient confusion | Unexpected bills arriving weeks later |
| Cash flow unpredictability | Unclear when revenue would be realised |
| Central dependency | All invoicing flows through Alida |

---

## New Model Summary

### Core Principles

| Element | Description |
|---------|-------------|
| **Real-Time Invoicing** | Services invoiced at time of delivery (same day) |
| **Payment on the Day** | Default expectation for all services |
| **Packages** | Discounted upfront bundles (15-20% off) for treatment protocols |
| **Optional Deposits** | Patient-elected prepayment for fewer touchpoints |
| **High-Cost Prepayment** | Items above threshold paid before ordering |

### Payment Rules

| Service Type | Payment Timing |
|-------------|----------------|
| Consultations | On the day |
| Supplements | On the day |
| IV Infusions | On the day |
| Hyperthermia / HBOT | Package (upfront) or on the day |
| High-cost tests/medications | Before ordering |

### Cancellation Policy

| Notice Given | Charge |
|--------------|--------|
| Less than 24 hours | 50% |
| Less than 1 hour / no-show | 100% |
| Clinical discretion | Waived for genuine medical emergencies |

### Medical Aid Position

- Sanctura does **not** bill medical aid directly
- Patients pay Sanctura, then reclaim independently
- Sanctura provides compliant invoices and support documentation

---

## Operational Process Flow (New Model)

```
┌─────────────────────────────────────────────────────────────────┐
│                     REAL-TIME INVOICING FLOW                    │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   TREATMENTS & MEDICATIONS          CONSULTATIONS & BOOKINGS   │
│   ────────────────────────          ────────────────────────   │
│                                                                 │
│   Nurse delivers service            Reception books/completes  │
│           ↓                                   ↓                │
│   Nurse creates invoice             Reception creates invoice  │
│   in Xero for patient               in Xero for patient        │
│           ↓                                   ↓                │
│           └──────────────┬──────────────────┘                  │
│                          ↓                                      │
│              Invoice added to patient account                   │
│                          ↓                                      │
│              Reception prints patient statement                 │
│                          ↓                                      │
│              Statement shows outstanding balance                │
│              (credits from packages/deposits offset)            │
│                          ↓                                      │
│              Patient pays outstanding amount                    │
│                          ↓                                      │
│              Payment recorded in Xero                           │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Role Responsibilities (New Model)

| Role | Invoicing Responsibility | When |
|------|-------------------------|------|
| **Nurses** | Treatments, IV infusions, medications dispensed | At time of delivery |
| **Reception** | Consultations, bookings, supplements sold at front desk | At time of service/sale |
| **Finance/Bookkeeper** | Package credits, deposit credits, adjustments, auditing | When payment received / ongoing |

---

## Shifted Role: From Invoicing to Auditing

### Current State (Alida's Role)
- Creating invoices retrospectively
- Chasing missing billing information
- Reconciling unbilled services
- Managing patient accounts

### Future State (New Bookkeeper Role)

| Activity | Frequency |
|----------|-----------|
| Spot-check invoice accuracy | Weekly |
| Review unbilled appointments | Weekly |
| Audit package credit balances | Weekly |
| Reconcile payments to invoices | Weekly |
| Identify training gaps/errors | Ongoing |
| Monthly financial reporting | Monthly |

**Key Shift:** From **reactive invoicing** to **proactive quality control**

---

## Rollout Plan

### Strategy
- **Phased rollout** - Cape Town first, UK to follow
- **Platform** - Xero (already in UK, to be deployed fresh in Cape Town)
- **Method** - Dry run → Training → Test run → Go live

### Why Cape Town First?
- Fresh Xero deployment provides clean starting point
- Lessons learned will inform UK transition
- UK already has established Xero workflows to adapt

### Rollout Phases

| Phase | Activity | Duration | Status |
|-------|----------|----------|--------|
| **Phase 1: Foundation** | Deploy Xero, configure accounts, templates, products | 2 weeks | Pending |
| **Phase 2: Dry Run** | Finance team tests full process internally | 1 week | Pending |
| **Phase 3: Training** | Train nurses and reception on invoicing in Xero | 1 week | Pending |
| **Phase 4: Test Run** | Supervised live transactions, daily review | 1-2 weeks | Pending |
| **Phase 5: Go Live CPT** | Independent operation, finance shifts to audit mode | Ongoing | Pending |
| **Phase 6: UK Rollout** | Apply lessons, repeat phases 2-5 for UK | 4-6 weeks | Pending |

### Phase 1 Tasks (Foundation)

| Task | Owner | Status |
|------|-------|--------|
| Deploy Xero in Cape Town | Finance/IT | Pending |
| Configure chart of accounts, service items, tax codes | Finance | Pending |
| Set up patient contacts in Xero | Admin | Pending |
| Configure invoice templates | Finance | Pending |
| Set up statement templates | Finance | Pending |
| Define package products and credit mechanics | Finance | Pending |

### Success Criteria

**Go-Live Readiness:**
- [ ] All staff can create invoices independently
- [ ] All staff understand which services they invoice
- [ ] Reception can print and explain patient statements
- [ ] Reception can record payments correctly
- [ ] Finance can record credits/deposits
- [ ] No critical errors in test run period
- [ ] Patient-facing templates are clear and professional

**Ongoing Metrics:**

| Metric | Target |
|--------|--------|
| Invoices created same-day | 100% |
| Invoice errors requiring correction | < 5% |
| Unbilled services identified in audit | < 2% |
| Patient complaints about billing | Minimal |
| Time from service to payment | Same day (default) |

---

## Risks and Mitigations

| Risk | Impact | Mitigation |
|------|--------|------------|
| Staff resistance to new process | Delays, errors | Clear communication on "why", involve staff early |
| Xero setup delays | Timeline slip | Start Xero deployment immediately |
| Training insufficient | Errors post go-live | Extended test run period, ongoing support |
| Patients confused by new process | Complaints, friction | Patient communication, reception scripts |
| Nurses too busy to invoice in real-time | Missed invoices | Simplify process, consider tablet/mobile Xero access |

---

## Transition Implications

### Opportunity

This project could **accelerate** in response to Alida's departure:
- The new model reduces dependency on a central invoicing person
- If implemented, it directly mitigates the invoicing risk from the transition
- Nurses and reception take over invoicing responsibilities

### Challenge

This project was **in planning stages** with Alida as a key driver:
- All phases are still pending
- Alida would have led Xero setup and training
- Without her, someone else must own implementation

### Recommendations

1. **Assess feasibility** of accelerating this project as part of transition response
2. **Identify new project owner** (OCFO? New hire? Internal?)
3. **Prioritise Phase 1** (Xero deployment for Cape Town) if proceeding
4. **Consider UK first** as alternative - Xero already deployed, less setup work
5. **Factor into OCFO scope** - could OCFO help implement this model?

---

## Key Decisions Required

| Decision | Options | Impact |
|----------|---------|--------|
| Proceed with project? | Yes / Pause / Modify | Determines invoicing approach |
| Which location first? | Cape Town (as planned) / UK (Xero ready) | Implementation complexity |
| Who owns implementation? | OCFO / New hire / Internal | Resource allocation |
| Timeline? | Accelerate / Maintain / Defer | Risk vs effort balance |

---

## Source Documents

- `background/invoice-plan/01-summary-overview.md`
- `background/invoice-plan/02-detailed-process-guide.md`
- `background/invoice-plan/03-rollout-plan.md`
