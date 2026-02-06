# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

This repository contains documentation for the **2026 Staff Salary Increase Review** (RemCo - Remuneration Committee). It is an information management project, not a code repository.

## Repository Structure

### `/background/`
Raw source documents containing briefing materials and notes from the previous COO. These are the original inputs.

### `/information-base/`
Structured, organized reference documents derived from the background materials:

| File | Contents |
|------|----------|
| `01-project-overview.md` | Key dates, scope, proposed increase ranges, eligibility rules |
| `02-staff-roster-complete.md` | Full staff list with roles, managers, locations, eligibility status |
| `03-economic-factors.md` | SA and UK economic indicators (CPI, electricity, lending rates) |
| `04-special-cases.md` | Staff requiring individual decisions, confirmed exclusions |
| `05-open-questions.md` | Unresolved questions and project checklist |
| `06-framework-principles.md` | Agreed framework from December 2025 RemCo meeting |
| `07-final-proposals-feb2026.md` | Final proposals with resolved special cases and totals |
| `08-reference-links.md` | Google Sheet link and other external references |

### `/new-information/`
Working documents and updated data files. CSVs are versioned exports from the Google Sheet (source of truth):

| File | Contents |
|------|----------|
| `Proposal To Be Sent to Directors - V4.csv` | Current master spreadsheet (V4) with all staff, recommendations, and calculations |
| `2026-02-06_JamesFirstFeedback.txt` | CEO feedback on initial proposal |

Earlier CSV versions (V1-V3) are retained for history.

### `/outputs/`
Final deliverables for distribution. Date-prefixed (`yyyy-mm-dd`) for version history:

| File | Contents |
|------|----------|
| `2026-02-06-Directors-Email.md` | Combined email for directors (intro, spreadsheet link, summary, proposals, justification) |
| `2026-02-06-Directors-Summary.md` | Detailed summary with methodology and individual proposals |
| `2026-02-06-increase-summary.md` | Succinct summary by currency (GBP/ZAR) with costs |
| `2026-02-06-Response-to-James.md` | Draft response to CEO feedback |
| `notes.md` | Working notes and status tracking |

## Key Context

- **Review deadline**: End of February 2026
- **Effective date**: March 2026 (financial year start)
- **Standard rates**: South Africa **7%**, United Kingdom **4%**
- **Exception**: Lexee Duval at **8%** (CEO recommendation, standout performance)
- **Special cases at 0%**: Yaseen Harneker (KPI-based), Dr Ismaeel Ebrahim, Kyle Bennett, Nuhaa Peterson
- **Eligibility**: Staff with >6 months service, not on probation
- **Total annual cost**: £6,856 + R162,256
- **Source of truth**: [Google Sheet](https://docs.google.com/spreadsheets/d/14CTOWKv_aNJ3FnmhDuXGdSfvkXo8tjG3EENFmEk1Lno/edit?gid=0#gid=0)
- **Deferred to March**: KPI/incentive framework, James's own remuneration, consulting fees on Xero

## Working with This Repository

When answering questions about the increase review:
1. Consult `outputs/` for final deliverables ready for distribution (use latest date-prefixed versions)
2. Consult `information-base/` files for structured reference information
3. Reference `background/` for original source material if needed
4. Check `07-final-proposals-feb2026.md` for current decisions and totals
5. The Google Sheet is the source of truth for staff data — CSV exports in `new-information/` are snapshots
