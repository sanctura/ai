# Sanctura Entity Structure & Financial Operations

**Last Updated:** 17 February 2026

---

## Entity Overview

Sanctura is a medical practice operating across South Africa and the United Kingdom through 7 legal entities.

### Structure Diagram

```
                    ┌──────────────────┐
                    │  Sanctura        │
                    │  Holdings (UK)   │
                    │  [Kinari]        │
                    └────────┬─────────┘
                             │ owns
                    ┌────────▼─────────┐
                    │  Sanctura Ltd    │
                    │  (UK Clinic)     │
                    │  [Xero]         │
                    └──────────────────┘

    ┌───────────────┐          ┌───────────────┐
    │ James La      │◄─────────│ Saint Raphael │
    │ Porta Inc     │ services │ (Management)  │
    │ [Medical]     │          │ [Operations]  │
    └───────┬───────┘          └───────┬───────┘
            │                          │
            │ linked                   │ employs
            ▼                          ▼
    ┌───────────────┐          ┌───────────────┐
    │ Trust & TTC   │          │ All Staff     │
    │ [James Pers]  │          │ (except Mma)  │
    └───────────────┘          └───────────────┘
```

### Entity Details

| Entity | Country | Type | Accounting | Managed By |
|--------|---------|------|------------|------------|
| **James La Porta Inc** | SA | Medical practice (primary income) | Xero | Ronald |
| **Saint Raphael (Pty) Ltd** | SA | Management/services company | Xero | Ronald |
| **La Porta Industries** | SA | Additional entity | Compliance only | Ronald (compliance) |
| **Sanctura Limited** | UK | Medical clinic (operating) | Xero | Ronald + Kinari |
| **Sanctura Holdings** | UK | Holding company | Kinari | Kinari (Ronald liaises) |
| **James La Porta Trust** | SA | Personal trust | Atlantic Trust | Atlantic Trust |
| **TTC** | SA | Janine's company | Inaura | Inaura |

### Key Entity Rules

- **Inc** = all medical-related expenses (prescriptions, doctor supplies)
- **Saint Raphael** = all non-medical expenses (supplements, operations, staff costs) and employs all staff except the medical officer
- **Sanctura Ltd** = UK operating clinic
- **Sanctura Holdings** = entirely managed by Kinari (UK accountants)
- **All assets should be in Saint Raphael's name** (including financed equipment)

---

## Banking

| Bank | Entity | Country | Access |
|------|--------|---------|--------|
| **Investec** | Inc, Saint Raphael | SA | James (Level 4), Grant (load/release non-SARS), Yaseen (load/release non-SARS) |
| **Barclays** | Sanctura Ltd (debit + 2 credit cards) | UK | Kinari, Grant |
| **Revolut** | Sanctura Ltd (KYC pending) | UK | TBC |

### Payment Workflow

```
Ronald prepares payment schedule
    → Grant loads into Investec
        → Grant or Yaseen releases non-SARS payments
        → James releases SARS payments (only he can)
```

**Critical gap:** James is the only Level 4 signatory for SARS payments. No backup exists.

---

## External Service Providers

| Provider | Services | Entities | Status |
|----------|----------|----------|--------|
| **Inaura** | Payroll, PAYE, VAT, income tax, financial statements | SA entities | Active - **planned phase-out** (Mar-Jun) |
| **Kinari / Capricorn Capital** | Banking, payroll, PAYE, financials, full Holdings management | UK entities | Active - continuing |
| **Imperium (Theo)** | Annual returns, UBO, CIPC secretarial | SA entities | Active |
| **Atlantic Trust** | Trust admin, payment execution | James's Trust | Active |
| **Intersure (Brian/Patricia)** | Insurance broker | SA entities | Active |
| **Ashley Page (Ashley/Olivia)** | Insurance broker | UK entity | Active |
| **Optiworx** | HR policies and contracts | SA entities | Active |
| **GPE** | UK rental management | Sanctura Ltd | Active |
| **TAFTS** | Equipment financing | Inc/Saint Raphael | Active |
| **AON** | James personal insurance | Personal | Relationship handover needed |

---

## Asset Financing

| Asset | Financier | Loan Entity | Paid By |
|-------|-----------|-------------|---------|
| Hypothermia baths | TAFTS | Inc | Saint Raphael |
| Ultrasound machine | TAFTS | Inc | Saint Raphael |
| New compressor | TAFTS (pending) | TBC | Saint Raphael |

---

## Property & Leases

### South Africa
| Property | Lessee | Notes |
|----------|--------|-------|
| Practice premises | Inc | Too complex to move to Saint Raphael |
| Storage units x2 | Saint Raphael | |
| Parking bays | Saint Raphael | |
| New office (from 1 Apr) | Saint Raphael | Lease pending |
| Temp offices (Ideas Cartel) | Saint Raphael | Ends March, then back to SuperStrike |

### United Kingdom
- Managed through GPE (rental agent)
- Yaseen handles lease agreement
