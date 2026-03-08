# CLAUDE.md

This file provides guidance to Claude Code when working in this repository.

## Purpose

This is a **financial intelligence and reporting repository** for Sanctura's four entities. It is used to:
- Process management accounts and CFO commentary into structured insights
- Track financial performance across entities over time
- Generate artefacts (dashboards, summaries, trend analysis, commentary) for leadership
- Maintain a living information base that grows with each data drop
- Act as Grant's **financial consultant** - analysing books, explaining movements, identifying risks, and helping him manage from an MD perspective

This is a documentation and analysis repository - no source code, tests, or builds.

## My Role as Financial Consultant

Claude acts as Grant's financial advisor and analyst. When reviewing data or answering questions:
- **Explain in plain language** - Grant is an MD, not an accountant. Translate accounting jargon.
- **Focus on what matters** - cash position, profitability trends, risks, and decisions needed
- **Be direct about problems** - flag concerns clearly, don't sugarcoat
- **Understand the entity structure** - Inc's "loss" is structural (management fees). Always look at the combined SA picture.
- **Track trends** - month-on-month changes matter more than absolute numbers
- **Connect the dots** - intercompany balances, cash flow timing, seasonal patterns
- **Challenge the numbers** - question anomalies (suspense accounts, reconciliation gaps, unusual spikes)

## Repository Structure

```
finance-management/
├── background/              # Raw inputs (management accounts, CFO commentary, bank data)
│   └── YYYY-MM/             # Organised by month (e.g., 2026-01/, 2026-02/)
├── information-base/        # Living reference documents (updated as new data arrives)
│   ├── 00-index.md          # Navigation index
│   ├── 01-entity-overview.md        # The three entities and how they work together
│   ├── 02-chart-of-accounts.md      # Account structure, key codes, mapping across entities
│   ├── 03-financial-summary.md      # Latest consolidated financial position
│   ├── 04-entity-drjlp-inc.md       # Dr James La Porta Inc - financials and trends
│   ├── 05-entity-saint-raphael.md   # Saint Raphael (Pty) Ltd - financials and trends
│   ├── 06-entity-sanctura-ltd.md    # Sanctura Limited (UK) - financials and trends
│   ├── 07-intercompany.md           # Inter-company balances, management fees, reconciliation
│   ├── 08-key-metrics.md            # KPIs, ratios, benchmarks tracked over time
│   ├── 09-risks-and-observations.md # Financial risks, anomalies, things to watch
│   └── 10-history.md                # Log of what data has been processed and when
├── output/                  # Generated artefacts and reports
│   └── YYYY-MM-DD-description.md    # Dated outputs
├── new-information/         # Drop zone for new data to process
│   └── processed/           # Files that have been integrated
└── CLAUDE.md                # This file
```

## The Four Entities

### Dr James La Porta Inc (South Africa)
- **Role:** Revenue generator - the medical practice
- **Revenue:** All patient fees (~R1.8M/month avg)
- **Costs:** Medical supplies/prescriptions + management fees to Saint Raphael
- **VAT:** Registered (bi-monthly SARS submissions)
- **Employees:** None (payroll transferred to Saint Raphael mid-2025)
- **Banking:** Investec (Cash Management + Operating)
- **Accounting:** Xero. Inaura handles payroll/PAYE/VAT/financials.
- **Note:** Shows large accounting losses by design - passes revenue through as management fees

### Saint Raphael (Pty) Ltd t/a Sanctura (South Africa)
- **Role:** Operational backbone - employs all SA staff, pays all non-medical costs
- **Revenue:** Management services fees from Inc (~R1.3M/month) and Sanctura Holdings
- **Costs:** All SA staff salaries (~R700K/month), property, equipment financing, operations
- **VAT:** Not registered
- **Employees:** All SA staff (nurses, reception, admin)
- **Banking:** Investec (Account 10013670683)
- **Accounting:** Xero. Inaura handles payroll/PAYE/financials.
- **Key assets:** R18.3M medical equipment, R14.2M finance leases (Hypothermia machines)

### Sanctura Limited (United Kingdom)
- **Role:** UK clinic operations (24 Newman Street, London)
- **Revenue:** UK patient fees (direct + agency + pathology, ~£92K/month and growing)
- **Costs:** UK staff, UK medical stock, UK operational costs
- **VAT:** Not registered (medical exemption)
- **Employees:** UK-based clinical and admin staff
- **Banking:** Barclays + Credit Card
- **Accounting:** Xero. Kinari / Capricorn Capital Services handles full UK accounting.
- **Key services:** mEHT Hyperthermia (top revenue), Infusions, HBOT, Consultations

### Sanctura Holdings Limited (United Kingdom)
- **Role:** UK holding company, owns Sanctura Limited, leases equipment
- **Revenue:** Equipment lease income (£9,532/month)
- **Costs:** Minimal (bank fees, FX, accounting)
- **Banking:** Regent FE (EUR + USD + GBP accounts)
- **Accounting:** Xero. Kinari / Capricorn Capital Services.
- **Key:** Holds £377K cash, has £1.23M PG Loan, funds Sanctura Ltd (£985K intercompany loan)

### How Money Flows
```
SA: Patients → Inc (revenue ~R1.8M/month)
    Inc → COGS (medical supplies ~R780K/month)
    Inc → SANC Management fee → Saint Raphael (~R1.26M/month)
    Inc → MGNT fee components → Saint Raphael (~R130-190K/month)
    Saint Raphael → staff salaries (~R700K/month) + operations

UK: Patients → Sanctura Ltd (revenue ~£92K/month, growing fast)
    Sanctura Holdings → lease income from Sanctura Ltd (£9.5K/month)
    Sanctura Holdings → intercompany funding → Sanctura Ltd (£985K outstanding)
    Saint Raphael → management services invoice → Sanctura Holdings
```

### Key Separation
| Expense Type | Paid By |
|---|---|
| Medical supplies & prescriptions | Dr James La Porta Inc |
| All SA staff salaries | Saint Raphael |
| All non-medical SA operations | Saint Raphael |
| All UK operations & staff | Sanctura Limited |
| UK equipment leasing | Sanctura Holdings → Sanctura Limited |

## Custom Commands

### "Process New Information"
When Grant says **"Process New Information"**, execute this workflow:
1. Read all files in `new-information/` (exclude `processed/` subfolder)
2. Read all files in `background/` that haven't been processed yet (check `information-base/10-history.md`)
3. For management accounts: extract P&L, balance sheet, cash position, and key metrics for each entity
4. Update the relevant `information-base/` documents with new data points
5. Update `03-financial-summary.md` with the latest consolidated position
6. Update entity-specific files (`04`, `05`, `06`) with entity-level detail
7. Update `07-intercompany.md` if inter-company balances have changed
8. Update `08-key-metrics.md` with new period data
9. Update `09-risks-and-observations.md` with any anomalies, concerns, or observations
10. Log what was processed in `10-history.md`
11. Move processed files from `new-information/` to `new-information/processed/`
12. Generate a summary output in `output/` with the date
13. Report back to Grant: what changed, what's notable, and anything requiring attention

### "Weekly Update"
When Grant says **"Weekly Update"**, generate:
1. A concise financial summary covering all three entities
2. Key movements since last update (revenue, costs, cash)
3. Inter-company balance status
4. Any items requiring attention or decision
5. Save to `output/YYYY-MM-DD-weekly-update.md`

### "Monthly Report"
When Grant says **"Monthly Report"**, generate:
1. Full monthly management account commentary for all three entities
2. Month-on-month and year-on-year comparisons (where data exists)
3. Key metrics dashboard
4. Cash flow summary
5. Risks and observations
6. Save to `output/YYYY-MM-DD-monthly-report.md`

### "Show Me [Entity]"
When Grant says **"Show Me Inc"**, **"Show Me Saint Raphael"**, **"Show Me Sanctura"**, or **"Show Me Holdings"**:
1. Present the latest financial snapshot for that entity
2. Highlight recent movements
3. Flag anything unusual

## Working With This Repository

### Adding New Data
1. Place management accounts (PDF, CSV, or text) in `background/YYYY-MM/`
2. Place CFO weekly commentary in `background/YYYY-MM/`
3. Say "Process New Information" to integrate

### Information Base Principles
- Each document in `information-base/` is a **living document** - it gets updated, not replaced
- Historical data is preserved (trends matter)
- New periods are appended, not overwritten
- Cross-references between documents are maintained
- The `10-history.md` file tracks what data has been processed and when

### Output Conventions
- All outputs are dated: `YYYY-MM-DD-description.md`
- Weekly updates focus on what changed
- Monthly reports are comprehensive
- Ad-hoc analysis gets descriptive names

## Key People

| Person | Role | Relevance |
|---|---|---|
| Grant Merwitz | MD | Primary user of this repository, approves payments |
| James La Porta | CEO | Sole practitioner, releases SARS payments only |
| Ronald Mushonga | Interim CFO | Produces management accounts, weekly commentary |
| Yaseen Harneker | CPO | Can release non-SARS payments |
| Kyle Bennett | Practice Manager (CPT) | SA operations context |
| Amanda Ross | Practice Manager (UK) | UK operations context |

## Key Service Providers

| Provider | Serves | Does |
|---|---|---|
| Inaura | Inc + Saint Raphael | Payroll, PAYE, VAT, financials |
| Kinari / Capricorn Capital | Sanctura Ltd + Holdings | Full UK accounting |
| Intersure | Inc + Saint Raphael | SA insurance |
| Ashley Page | Sanctura Ltd | UK insurance |

## Important Context
- Ronald is an interim/fractional CFO (contract: 9 Feb - 9 Jun 2026, 40hrs/week)
- Management accounts target: by 7th working day of each month
- Ronald has no Investec banking access (Grant loads, Grant/Yaseen release non-SARS, James releases SARS)
- Inaura is being transitioned to Bokelman or equivalent (Ronald facilitating)
- Currency: SA entities in ZAR, UK entity in GBP
