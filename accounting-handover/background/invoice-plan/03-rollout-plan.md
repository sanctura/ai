# Sanctura Invoicing Model - Rollout Plan

## 1. Rollout Strategy Overview

### Approach
- **Phased rollout** - Cape Town first, UK to follow
- **Platform** - Xero (already deployed in UK, to be deployed in Cape Town)
- **Method** - Dry run → Training → Test run → Go live

### Why Cape Town First?
- Fresh Xero deployment provides clean starting point
- Lessons learned will inform UK transition
- UK already has established Xero workflows to adapt

---

## 2. Operational Process Flow

### 2.1 How It Works in Xero

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

### 2.2 Role Responsibilities

| Role | Invoicing Responsibility | When |
|------|-------------------------|------|
| **Nurses** | Treatments, IV infusions, medications dispensed | At time of delivery |
| **Reception** | Consultations, bookings, supplements sold at front desk | At time of service/sale |
| **Finance/Bookkeeper** | Package credits, deposit credits, adjustments | When payment received |

### 2.3 Patient Account Mechanics in Xero

| Scenario | Xero Action | Statement Shows |
|----------|-------------|-----------------|
| Service delivered | Invoice created | Amount owing increases |
| Patient pays in advance | Payment/credit recorded | Credit balance (negative owing) |
| Package purchased | Credit recorded for package value | Credit balance |
| Service against package | Invoice created, offset by credit | Reduced credit or amount owing |
| Patient pays at reception | Payment recorded | Zero balance or remaining credit |

### 2.4 Example Patient Journey

**Patient purchases 10-session hyperthermia package (R15,000 after discount)**

1. Finance records R15,000 credit on patient account
2. Patient attends Session 1 → Nurse invoices R1,800 → Statement shows R13,200 credit
3. Patient has consultation → Reception invoices R1,500 → Patient pays R1,500 on the day
4. Patient attends Session 2 → Nurse invoices R1,800 → Statement shows R11,400 credit
5. ...continues until credit depleted, then patient owes money again

---

## 3. Shifted Role: Accounting/Bookkeeper Function

### From: Invoicing
- Creating invoices retrospectively
- Chasing missing billing information
- Reconciling unbilled services

### To: Auditing & Oversight
| Activity | Frequency |
|----------|-----------|
| Spot-check invoice accuracy | Weekly |
| Review unbilled appointments | Weekly |
| Audit package credit balances | Weekly |
| Reconcile payments to invoices | Weekly |
| Identify training gaps/errors | Ongoing |
| Monthly financial reporting | Monthly |

This shift moves the bookkeeper from **reactive invoicing** to **proactive quality control**.

---

## 4. Rollout Phases

### Phase 1: Foundation (Cape Town)

| Step | Activity | Owner | Status |
|------|----------|-------|--------|
| 1.1 | Deploy Xero in Cape Town | Finance/IT | Pending |
| 1.2 | Configure chart of accounts, service items, tax codes | Finance | Pending |
| 1.3 | Set up patient contacts in Xero | Admin | Pending |
| 1.4 | Configure invoice templates | Finance | Pending |
| 1.5 | Set up statement templates | Finance | Pending |
| 1.6 | Define package products and credit mechanics | Finance | Pending |

### Phase 2: Dry Run (Finance Team)

| Step | Activity | Owner | Status |
|------|----------|-------|--------|
| 2.1 | Finance team runs through full process internally | Finance | Pending |
| 2.2 | Test invoice creation (treatments, consultations) | Finance | Pending |
| 2.3 | Test credit/deposit recording | Finance | Pending |
| 2.4 | Test statement generation | Finance | Pending |
| 2.5 | Test payment recording and reconciliation | Finance | Pending |
| 2.6 | Document issues and refine process | Finance | Pending |

### Phase 3: Staff Training

| Step | Activity | Owner | Status |
|------|----------|-------|--------|
| 3.1 | Prepare training materials | Finance | Pending |
| 3.2 | Train nursing team on invoice creation | Finance + Clinical Lead | Pending |
| 3.3 | Train reception on invoice creation & payments | Finance + Office Manager | Pending |
| 3.4 | Train reception on statement printing | Finance | Pending |
| 3.5 | Q&A and scenario walkthroughs | Finance | Pending |

### Phase 4: Test Run (Supervised Live)

| Step | Activity | Owner | Status |
|------|----------|-------|--------|
| 4.1 | Staff process real transactions with supervision | All + Finance oversight | Pending |
| 4.2 | Finance reviews all invoices same-day | Finance | Pending |
| 4.3 | Correct errors and provide feedback | Finance | Pending |
| 4.4 | Run for defined period (e.g. 1-2 weeks) | All | Pending |
| 4.5 | Sign-off that team is ready | Finance + Management | Pending |

### Phase 5: Go Live (Cape Town)

| Step | Activity | Owner | Status |
|------|----------|-------|--------|
| 5.1 | Official go-live date communicated | Management | Pending |
| 5.2 | Staff operate independently | Nurses + Reception | Pending |
| 5.3 | Finance shifts to audit/spot-check mode | Finance | Pending |
| 5.4 | Weekly review meetings (first month) | Finance + Management | Pending |
| 5.5 | Refine process based on learnings | All | Pending |

### Phase 6: UK Rollout

| Step | Activity | Owner | Status |
|------|----------|-------|--------|
| 6.1 | Document lessons learned from Cape Town | Finance | Pending |
| 6.2 | Adapt process for UK context (if needed) | Finance | Pending |
| 6.3 | Repeat Phases 2-5 for UK team | Finance + UK Team | Pending |

---

## 5. Timeline Template

| Phase | Duration | Target Start | Target Complete |
|-------|----------|--------------|-----------------|
| Phase 1: Foundation | 2 weeks | TBD | TBD |
| Phase 2: Dry Run | 1 week | TBD | TBD |
| Phase 3: Training | 1 week | TBD | TBD |
| Phase 4: Test Run | 1-2 weeks | TBD | TBD |
| Phase 5: Go Live CPT | Ongoing | TBD | - |
| Phase 6: UK Rollout | 4-6 weeks | TBD | TBD |

---

## 6. Success Criteria

### Go-Live Readiness (Phase 4 → Phase 5)

- [ ] All staff can create invoices independently
- [ ] All staff understand which services they invoice
- [ ] Reception can print and explain patient statements
- [ ] Reception can record payments correctly
- [ ] Finance can record credits/deposits
- [ ] No critical errors in test run period
- [ ] Patient-facing templates are clear and professional

### Ongoing Success Metrics

| Metric | Target |
|--------|--------|
| Invoices created same-day | 100% |
| Invoice errors requiring correction | < 5% |
| Unbilled services identified in audit | < 2% |
| Patient complaints about billing | Minimal |
| Time from service to payment | Same day (default) |

---

## 7. Risks and Mitigations

| Risk | Impact | Mitigation |
|------|--------|------------|
| Staff resistance to new process | Delays, errors | Clear communication on "why", involve staff early |
| Xero setup delays | Timeline slip | Start Xero deployment immediately |
| Training insufficient | Errors post go-live | Extended test run period, ongoing support |
| Patients confused by new process | Complaints, friction | Patient communication, reception scripts |
| Nurses too busy to invoice in real-time | Missed invoices | Simplify process, consider tablet/mobile Xero access |

---

## 8. Next Steps

1. **Confirm Xero deployment timeline for Cape Town**
2. **Assign owners to each rollout step**
3. **Set target dates for each phase**
4. **Begin preparing training materials**
5. **Draft patient communication (if needed)**
