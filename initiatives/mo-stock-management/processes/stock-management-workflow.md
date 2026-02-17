# Stock Management Workflow

## Proposed Process Overview

```
Stock Take → Review Levels → Raise Purchase Orders → Receive Goods → Update System → Repeat
```

---

## 1. Regular Stock Takes

**Frequency**: Weekly (high-turnover items) / Monthly (all items)

**Who**: Nursing staff

**Process**:
1. Print/export current stock list from system
2. Physically count each tracked item
3. Record actual quantities
4. Compare against system quantities
5. Investigate and resolve any discrepancies
6. Update system with actual counts

---

## 2. Reorder Process

**Trigger**: Stock falls below defined reorder point

**Process**:
1. System generates alert (or identified during stock take)
2. Review reorder quantity based on:
   - Average usage rate
   - Supplier lead time
   - Minimum order quantities
   - Budget considerations
3. Raise purchase order in Xero
4. Send PO to supplier
5. Track order status

### Suggested Reorder Points (to be refined with usage data)

| Category | Reorder Point | Reorder Qty | Notes |
|----------|---------------|-------------|-------|
| High-volume IV (Ascorbic Acid, Curcumin) | 2 weeks supply | 1 month supply | Based on usage data |
| Standard IV concentrates | 5 units | 10-20 units | Adjust per item |
| Oral supplements | 3 units | 6-12 units | Adjust per demand |
| High-value items (Bosvene, NAD+) | 2 units | 5 units | Smaller orders, higher value |
| Controlled drugs (Modafinil, Nebido) | 2 units | As needed | Stricter ordering process |

---

## 3. Receiving Goods

**Process**:
1. Check delivery against purchase order
2. Verify quantities, batch numbers, expiry dates
3. Inspect for damage or temperature excursions
4. Record batch numbers and expiry dates
5. Update stock quantities in system
6. Store in appropriate location (temperature, controlled drug storage)
7. File delivery note with PO

---

## 4. Dispensing / Using Stock

**Process**:
1. Record each item used per patient
2. Update system (ideally in real-time or end-of-day)
3. Note batch number used (for traceability)
4. For controlled drugs: update controlled drug register

---

## 5. Expiry Management

**Process**:
1. Monthly review of items approaching expiry (within 3 months)
2. Prioritise use of items closest to expiry (FEFO - First Expired, First Out)
3. Quarantine expired items
4. Dispose of expired items per regulations
5. Record wastage

---

## 6. Supplier Management

### Current Supplier Categories (to be populated)

| Supplier | Products | Lead Time | Min Order | Payment Terms |
|----------|----------|-----------|-----------|---------------|
| TBC | German IV products | TBC | TBC | TBC |
| TBC | UK supplements | TBC | TBC | TBC |
| TBC | Natrocuetics range | TBC | TBC | TBC |
| TBC | Biosomo range | TBC | TBC | TBC |
| TBC | HEEL products | TBC | TBC | TBC |

---

## 7. Reporting

**Weekly**: Stock alerts, items below reorder point
**Monthly**: Stock valuation, usage trends, wastage report
**Quarterly**: Full stock take reconciliation, supplier review, cost analysis

---

## Roles & Responsibilities

| Role | Responsibilities |
|------|-----------------|
| MO / Grant | Strategic oversight, supplier relationships, system decisions, regulatory compliance |
| Nursing Staff | Daily stock usage recording, weekly stock takes, flagging low stock |
| Admin/Accounts | Purchase order processing, Xero updates, supplier payments |

---

## Open Questions

- [ ] What is the current average weekly/monthly usage for each item?
- [ ] Who are the current suppliers and what are their terms?
- [ ] What is the current storage setup (temperature monitoring, controlled drug safe)?
- [ ] Is there a budget allocated for a new inventory system/plugin?
- [ ] Who will be the primary system administrator?
- [ ] What training is needed for staff adoption?
