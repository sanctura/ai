# MO Stock Management - Kickoff Task Plan (Detailed)

## Overview

Two parallel workstreams to launch the stock management initiative. These run independently — neither blocks the other.

---

## Workstream A: Stock Management Process

**Goal**: Document how things work today, then design and implement an improved process.

---

### A1. Document the Current ("As-Is") Process (Week 1-2)

Map out exactly how stock management works today, warts and all. This is about capturing reality, not aspirations.

#### A1.1 How stock is currently ordered
- Who decides when to order? (Nurses flagging, MO deciding, ad-hoc?)
- How are orders placed? (Email, phone, supplier portal?)
- Is a Xero PO raised, or are orders placed informally?
- Who approves orders? Is there a budget threshold?
- How are orders tracked from placement to delivery?

#### A1.2 How stock is currently received
- Who receives deliveries?
- What checks are done? (Quantity verification, batch numbers, expiry dates, damage?)
- Is Xero updated on receipt? By whom?
- Where are delivery notes filed?
- How is cold-chain/temperature handled on receipt?

#### A1.3 How stock is currently stored
- Where is stock physically kept? (Location map / room layout)
- Is there separation between IV products, supplements, controlled drugs?
- Is there temperature monitoring in place?
- How are items organised? (By type, alphabetically, by supplier?)
- Is FEFO (First Expired, First Out) practiced?

#### A1.4 How stock is currently used/dispensed
- How is stock drawn for patient use?
- Is usage recorded per patient? Where? (Patient record, separate log, nowhere?)
- Are batch numbers recorded when items are administered?
- Is Xero updated when stock is used? In real-time or periodically?
- How is wastage/breakage recorded?

#### A1.5 How stock takes currently happen
- How often are stock takes done?
- Who does them?
- What's the process? (Printed list, manual count, how are discrepancies handled?)
- Is Xero updated after a stock take?
- How long does a stock take typically take?

#### A1.6 Current pain points and gaps
- Interview nursing staff: what frustrates them about the current process?
- Interview MO: what visibility gaps exist?
- Where do stockouts happen? Which items run out most often?
- What workarounds exist? (e.g., borrowing from another clinic, emergency orders)
- Where does the process break down most frequently?

**Output**: A written "Current State" document capturing the actual process, key pain points, and a gap analysis.

---

### A2. Propose the New ("To-Be") Process (Week 2-4)

Design the improved process, informed by the reality documented in A1.

#### A2.1 Define the target operating model
- What does "good" look like for this practice?
- Roles and responsibilities: who owns what in the new process?
- What level of system support is realistic? (Xero-only vs plugin vs full system)
- What's the minimum viable process that addresses the biggest pain points?

#### A2.2 Design the new ordering process
- Reorder triggers: system alerts vs manual review vs hybrid
- Reorder points and quantities for all active items (based on usage data)
- PO workflow: who raises, who approves, how tracked
- Supplier management: preferred suppliers, backup suppliers, escalation

#### A2.3 Design the new receiving process
- Standardised goods-in checklist
- Batch and expiry recording at point of receipt
- Xero update workflow
- Exception handling (short deliveries, damaged goods, wrong items)

#### A2.4 Design the new dispensing/usage tracking process
- How to record usage per patient in a way that's sustainable for nurses
- Batch traceability requirements (link patient → batch number)
- Real-time vs end-of-day Xero updates — what's practical?
- Wastage recording

#### A2.5 Design the new stock take process
- Frequency: weekly for high-turnover, monthly for full count
- Process: printed sheet vs mobile/tablet scanning
- Discrepancy investigation and resolution workflow
- Xero reconciliation process

#### A2.6 Fill the data gaps
- Backfill purchase prices in Xero (currently £0.00 for most items)
- Document all suppliers (contacts, lead times, MOQs, terms)
- Review zero-stock items (23 items): reorder, discontinue, or flag as seasonal
- Review low-stock items (33 items at 1-5 units): confirm if levels are adequate

#### A2.7 Write SOPs
- Stock Take SOP (one page, for nursing staff)
- Ordering & Reorder SOP (one page, includes approval thresholds)
- Goods Receiving SOP (one page, includes checklist)
- Dispensing & Usage Recording SOP (one page)
- Expiry Management SOP (monthly review, FEFO, quarantine, disposal)

#### A2.8 System/tool recommendation
- Based on the process design, recommend whether to:
  - Stay with Xero only (with better process discipline)
  - Add a Xero plugin (Cin7/DEAR, Unleashed) for reorder alerts and batch tracking
  - Adopt pharmacy-specific software
- Include cost-benefit summary and implementation timeline

**Output**: A written "Proposed Process" document with the new workflow, SOPs, data cleanup plan, and system recommendation.

---

## Workstream B: Regulatory & Legal Adherence

**Goal**: Ensure the practice is compliant with UK regulations for importing, storing, and dispensing medicines and supplements.

---

### B1. Classify All Stock by Regulatory Status (Week 1-2)
- Review all 78 tracked items and classify each as:
  - **Food supplement** (FSA regulated) — most oral supplements
  - **Licensed medicine** (has UK Marketing Authorisation) — e.g., Ceftriaxone, Cordarone X, Promethazine
  - **Unlicensed special** (no UK MA, imported under specials scheme) — most German IV products (Pascoe, Kohler, Burghardt)
  - **Controlled drug** (Home Office requirements) — Modafinil (Schedule 4), Nebido (testosterone)
  - **Prescription-only medicine (POM)** — requires prescriber oversight
- Flag items in each category in `docs/regulatory-considerations.md`
- **Output**: Complete regulatory classification table for all tracked items

### B2. Import Licensing Review (Week 1-3)
- Determine how German IV products are currently being sourced:
  - Direct from manufacturer? Via a UK-based specials importer? Via an EU distributor?
- Check if the practice holds or needs:
  - **Wholesale Dealer's Licence (WDL)** — required to distribute/supply medicines
  - **Manufacturer's/Importer's Licence (MIA)** — required to import medicines into UK
- If using a specials importer, verify they hold appropriate MHRA licences
- Check current import route against post-Brexit requirements (UK batch testing/release)
- **Output**: Clear picture of licensing status, gap list if any licences needed

### B3. Controlled Drug Compliance (Week 2-3)
- Audit current controlled drug storage:
  - Is there a compliant locked cabinet/safe for Modafinil and Nebido?
  - Is there a controlled drug register in use?
  - Are entries being made for every receipt and dispensing?
- Review Home Office requirements for Schedule 4 (Modafinil) and testosterone (Nebido)
- Check if a **Controlled Drug Accountable Officer** is designated
- Ensure destruction/disposal procedures are documented
- **Output**: Controlled drug compliance status, remediation actions if needed

### B4. Storage & Handling Audit (Week 2-4)
- Audit temperature-controlled storage:
  - Are fridge items (many IV concentrates) stored at 2-8°C?
  - Is there temperature monitoring and logging?
  - Are there SOPs for temperature excursions?
- Check storage segregation:
  - Controlled drugs separate from general stock
  - Expired/quarantined items separated
- Review cold chain management for deliveries
- **Output**: Storage compliance report, remediation actions if needed

### B5. Designate a Responsible Person (Week 2-3)
- Confirm whether a **Responsible Person (RP)** for medicines management is designated
- If not, determine who should hold this role (likely needs pharmacy qualification)
- Define their responsibilities:
  - Oversight of medicines ordering, storage, dispensing
  - Regulatory compliance monitoring
  - Staff training on medicines handling
- **Output**: Named Responsible Person with documented responsibilities

### B6. Dispensing & Record-Keeping Review (Week 3-5)
- Review current dispensing practices:
  - Are batch numbers recorded when items are administered to patients?
  - Is there a dispensing log or is this captured in patient records?
  - Can you trace from patient back to batch number?
- Ensure record keeping meets MHRA requirements:
  - Purchase records for all medicines
  - Dispensing records for POMs
  - Controlled drug register entries
  - Batch/expiry records
- Identify gaps and create templates if needed
- **Output**: Record-keeping compliance status, templates for any gaps

### B7. Engage Regulatory Advisor if Needed (Week 3-6)
- If B1-B6 surface any unclear areas (likely around import licensing), engage:
  - MHRA helpline for guidance on specials importing
  - A pharmaceutical regulatory consultant for licensing advice
  - Home Office for controlled drug queries
- Budget for professional advice if licensing applications are needed
- **Output**: Professional guidance on any grey areas, action plan for compliance

---

## Parallel Timeline View

```
Week:    1       2       3       4       5       6
         |       |       |       |       |       |
STOCK    [A1: Document Current Process  ]
MGMT              [A2: Design & Propose New Process         ]

REGULATORY [B1 Classification][B3 Controlled Drugs]
           [B2 Import Licences    ][B5 Resp Person]
                    [B4 Storage Audit    ]
                              [B6 Records Review  ]
                                   [B7 Advisor if needed]
```

---

## Key Reference Documents
- `docs/inventory-analysis.md` — zero-stock and low-stock item lists
- `docs/stock-categories.md` — category definitions
- `docs/regulatory-considerations.md` — regulatory flags and licensing checklist
- `docs/system-options.md` — plugin evaluation criteria
- `processes/stock-management-workflow.md` — workflow and SOP framework
