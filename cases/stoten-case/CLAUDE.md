# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a **medical case management repository** for the Louise Stoten case - a potential medical negligence claim against Sanctura clinic. It contains documentation, invoices, and consolidated information to support legal defense preparation.

## Folder Structure

- `background/` - Original source documents (markdown files, PDFs, correspondence)
- `background/invoices/` - All billing records (43 invoices: 8 London, 35 Cape Town)
- `information-base/` - Consolidated, organized case information for defense preparation
- `new-information/` - Intake folder for new documents to be incorporated
- `output/` - Shareable documents (PDFs) for legal counsel and stakeholders
- `context.md` - Initial instructions and file descriptions

## New Information Workflow

The `new-information/` folder is used to bring additional documents into the case after initial processing:

1. **Adding new items:**
   - Place new documents in `new-information/items/`
   - Log the item in `new-information/new-items-log.md` with date and description
   - Use checkbox format: `- [ ] **Date** - "path" - Description`

2. **Incorporating items:**
   - Read the new document from `items/`
   - Update relevant `information-base/` files with the new information
   - Copy the source document to `background/` for archival
   - Mark the item as incorporated: `- [x]` with cross-references to updated files

3. **Log format example:**
   ```
   - [x] **2 Feb 2026** - "items\document.md" - Description
     - Added to: `04-medical-correspondence.md` (Section X)
     - Added to: `02-timeline.md` (relevant entries)
   ```

## Key Files in information-base/

| File | Purpose |
|------|---------|
| `00-case-summary.md` | Executive summary and current defense status |
| `01-patient-profile.md` | Patient details and medical history |
| `02-timeline.md` | Chronological events with invoice references |
| `03-treatment-records.md` | Treatment protocols and medications |
| `04-medical-correspondence.md` | Letters from specialists, referrals |
| `05-allegations-response.md` | Each allegation vs clinic's defense position |
| `06-invoice-summary.md` | Complete billing summary (London + Cape Town) |
| `07-action-items.md` | Outstanding tasks and priorities |
| `08-key-contacts.md` | All relevant personnel with roles |
| `09-medicolegal-defense.md` | Full medicolegal defense position |

## Output Files

Shareable documents for legal counsel and stakeholders (PDF + source markdown):

| File | Purpose |
|------|---------|
| `01-executive-summary` | Concise case briefing for legal counsel |
| `02-action-checklist` | Printable todo list with deadlines |
| `03-response-letter-paul-stoten-draft-X` | Draft response letter to complainant (versioned) |

### Draft Versioning

For documents requiring review and revision (e.g., response letters), use `-draft-X` suffix:
- `03-response-letter-paul-stoten-draft-1.md` - Initial draft
- `03-response-letter-paul-stoten-draft-2.md` - After first round of feedback
- etc.

Keep previous drafts for reference until final version is approved.

## Working With This Repository

1. **Start with `00-case-summary.md`** for current status and defense strength
2. **New documents** should be added to `background/` with date prefix (e.g., `2026-02-01 DocumentName.pdf`)
3. **Update information-base files** when new evidence is added
4. **Read PDFs directly** - this repository relies on PDF reading capability for invoices and medical documents

## Key Case Facts

- **Patient:** Louise Stoten (died September 16, 2025)
- **Complainant:** Paul Stoten (husband)
- **Clinic:** Sanctura (London + Cape Town locations)
- **Defense Status:** Strong - per Dr Laporta: "We have everything we need, only loop hole is antibiotic prescription we need Maria to fill"
- **Critical Outstanding:** Sister Maria Tam's prescription records
