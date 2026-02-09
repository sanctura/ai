# How Money Flows

## Bank Accounts

### South Africa - Investec

| Account | Entity | Used For |
|---------|--------|----------|
| Operating Account | James La Porta Inc | Patient revenue, medical supplier payments, SARS payments |
| Operating Account | Saint Raphael | Staff salaries, non-medical supplier payments, management expenses |

**Your access:** None currently. You can view via Xero bank feeds, but you cannot load or release payments in Investec.

### United Kingdom - Barclays

| Account | Entity | Used For |
|---------|--------|----------|
| Debit Account | Sanctura Ltd | Operations, salaries, patient receipts |
| Credit Card (Amanda) | Sanctura Ltd | Purchases, 600 GBP limit |
| Credit Card (Maria) | Sanctura Ltd | Purchases, 600 GBP limit |

**Your access:** Kinari manages UK banking. You monitor via Xero.

### United Kingdom - Revolut

| Account | Entity | Status |
|---------|--------|--------|
| Operations | Sanctura Ltd | KYC pending, managed by Kinari |

---

## Payment Controls

This is critical to understand. There is a strict dual-control system:

### SA Supplier Payments (Non-SARS)

```
1. You receive and reconcile supplier invoice
2. You prepare a payment schedule (amounts, bank details, references)
3. You give the schedule to Grant
4. Grant loads the payment into Investec
5. Grant or Yaseen releases the payment
```

### SARS Payments (VAT, Income Tax)

```
1. Inaura calculates VAT/PAYE
2. You review the calculation
3. You give the go-ahead and prepare the payment details
4. Grant loads the payment into Investec
5. Only James can release SARS payments - follow up with him
```

**Why this matters:** James has Level 4 banking access - no one else can release tax payments. If James is unavailable, SARS payments are stuck. Flag any upcoming SARS payments to Grant early so we can coordinate James's availability.

### UK Payments

```
1. Invoice received
2. Kinari processes through Barclays
3. You monitor via Xero
```

UK payments are handled by Kinari - you don't need to process them directly.

---

## Revenue Flow

### South Africa
```
Patients pay for services
    --> Revenue into Inc (Investec)
    --> Inc pays medical suppliers
    --> Saint Raphael invoices Inc for management services
    --> Saint Raphael pays staff, operations, non-medical suppliers
```

### United Kingdom
```
Patients pay for services
    --> Revenue into Sanctura Ltd (Barclays)
    --> Sanctura Ltd pays UK suppliers, staff
    --> Sanctura Ltd receives invoices from Saint Raphael for management services
```

### Inter-Company
```
Saint Raphael --> invoices Inc (management services)
Saint Raphael --> invoices Sanctura Holdings (management services)
```

These inter-company invoices are important for the correct distribution of costs and revenue across entities.

---

## Cash Flow Monitoring

**Your responsibility:** Monitor SA bank balances and flag any concerns.

Key things to watch:
- **Sufficient funds for payroll** - salaries must always be paid on time
- **SARS payment timing** - advise when there's enough in the account, then coordinate release with James
- **Supplier payment timing** - batch payments weekly, don't let suppliers fall too far behind
- **UK balance** - monitor via Xero, flag any concerns to Grant who will coordinate with Kinari

---

## Supplier Payment Rhythm

| Activity | Frequency | Detail |
|----------|-----------|--------|
| Receive supplier invoices | Ongoing | Log them as they arrive |
| Reconcile to PO/delivery | Before payment | Ensure goods/services were received |
| Prepare payment schedule | Weekly | Batch all approved invoices |
| Grant loads payments | Weekly | You hand the schedule to Grant |
| Exco releases | Weekly | Grant or Yaseen releases |
| Monthly supplier review | Monthly | Review aged payables, flag issues |
