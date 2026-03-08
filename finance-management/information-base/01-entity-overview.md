# Entity Overview

## The Four Entities

### Dr James La Porta Inc (South Africa)
- **Role:** Revenue generator - the medical practice
- **Revenue:** All patient fees (consultations, IV therapy, treatments, medications)
- **Costs:** Medical supplies/prescriptions + management fees to Saint Raphael
- **VAT:** Registered (bi-monthly SARS submissions)
- **Employees:** None directly (payroll transferred to Saint Raphael mid-2025)
- **Banking:** Investec (Cash Management Account 1100595242540 + Operating Account)
- **Accounting:** Xero. Inaura handles payroll/PAYE/VAT/financials.

### Saint Raphael (Pty) Ltd t/a Sanctura (South Africa)
- **Role:** Operational backbone - employs all SA staff, pays all non-medical costs
- **Revenue:** Management services fees invoiced to Inc and Sanctura Holdings
- **Costs:** Staff salaries, non-medical suppliers, property leases, equipment financing, operational expenses
- **VAT:** Not registered
- **Employees:** All SA staff (nurses, reception, admin) - ~R700K/month total payroll
- **Banking:** Investec (Account 10013670683)
- **Accounting:** Xero. Inaura handles payroll/PAYE/financials.
- **Key assets:** R18.3M medical equipment, R14.2M finance leases (Hypothermia machines)

### Sanctura Limited (United Kingdom)
- **Role:** UK clinic operations (24 Newman Street, London)
- **Revenue:** UK patient fees (direct + agency + pathology)
- **Costs:** UK staff, UK medical stock, UK operational costs
- **VAT:** Not registered (medical exemption)
- **Employees:** UK-based staff (growing team)
- **Banking:** Barclays (Account 20717503880184) + Credit Card
- **Accounting:** Xero. Kinari / Capricorn Capital Services handles full UK accounting.
- **Key services:** mEHT Hyperthermia, Infusions, HBOT, Consultations, Endovascular Laser, Pathology

### Sanctura Holdings Limited (United Kingdom)
- **Role:** UK holding company, owns Sanctura Limited, leases equipment
- **Revenue:** Equipment lease income (£9,532/month to Sanctura Ltd)
- **Costs:** Minimal (bank fees, FX, accounting)
- **Banking:** Regent FE (EUR + USD + GBP accounts)
- **Accounting:** Xero. Kinari / Capricorn Capital Services.
- **Key assets:** Oncotherm lease equipment (£558K), licensing (£88K), medical equipment (£138K)
- **Key liabilities:** PG Loan (£1,232,000), Deferred Lease Income (£257K)

## How They Work Together

### Money Flow - South Africa
```
Patients → Dr James La Porta Inc (collects all revenue ~R1.8M/month avg)
  ├── Pays medical suppliers (COGS ~R780K/month avg)
  ├── Pays SARS (VAT bi-monthly, PAYE monthly)
  ├── Pays SANC Management fee to Saint Raphael (~R1.26M/month)
  └── Pays MGNT fee components to Saint Raphael (~R130-190K/month, billed periodically)

Saint Raphael (receives management fees ~R1.7M/month)
  ├── Pays all SA staff salaries (~R700K/month)
  ├── Pays non-medical suppliers
  ├── Pays property leases (~R80-90K/month)
  ├── Pays equipment financing (R14.2M in finance leases)
  └── Pays SARS (PAYE monthly)
```

### Money Flow - United Kingdom
```
Patients → Sanctura Limited (collects revenue ~£92K/month, growing)
  ├── Pays UK staff salaries
  ├── Pays UK medical stock suppliers
  ├── Pays UK operational costs
  ├── Pays rent (£23,750/month)
  └── Pays HMRC (PAYE via Kinari)

Sanctura Holdings
  ├── Receives lease income from Sanctura Ltd (£9,532/month)
  ├── Provides intercompany funding to Sanctura Ltd (£985K outstanding)
  └── Holds cash reserves (£377K across EUR/USD/GBP accounts)

Saint Raphael → invoices Sanctura Holdings for management services
```

### Expense Separation
| Expense Type | Paid By |
|---|---|
| Medical supplies & prescriptions | Dr James La Porta Inc |
| All SA staff salaries | Saint Raphael |
| All non-medical SA operations | Saint Raphael |
| All UK operations & staff | Sanctura Limited |
| Equipment leasing (UK) | Sanctura Holdings → Sanctura Limited |

## Payment Controls (SA - Investec Dual Control)
| Role | Load | Release |
|---|---|---|
| Ronald (former CFO) | Yes | Non-SARS only |
| Grant | Yes | Non-SARS only |
| Yaseen | Yes | Non-SARS only |
| James | No | SARS payments only (Level 4) |

## Supporting Entities
| Entity | Purpose |
|---|---|
| Epic Simian | Related entity with loans across Inc (R441K), Saint Raphael (R429K), and Holdings (£410K) |
| La Porta Industries (Pty) Ltd | SA entity, annual compliance only |
| James's Personal Trust (Archangel Michael Trust) | Has R1.18M loan to Inc |
| TTC | Annual income tax returns only (Inaura) |
