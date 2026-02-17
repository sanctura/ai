# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

This is **not a code repository**. It is a structured information management project for Grant Merwitz (Managing Director, Sanctura) to organise, review, and respond to plans and proposals from Ronald Mushonga, a newly engaged Interim CFO on a 4-month contract (Feb-Jun 2026). The project tracks the financial operations transition following the resignation of Sanctura's long-standing Financial Manager.

## Folder Structure

- **`background/`** - Original context documents. Do not modify these.
- **`new-information/`** - Drop zone where Grant places new documents (emails, plans, proposals from Ronald or others). Files here are unprocessed.
- **`new-information/processed/`** - Files that have been read, integrated into the information base, and moved here.
- **`information-base/`** - Living reference documents (numbered 01-09). These are the project's core knowledge base and should be updated as new information arrives.
- **`output/`** - Draft responses and communications for Grant to send. Files prefixed `yyyy-mm-dd`.

## Custom Command: "Process New Information"

When Grant says **"Process New Information"**, execute this workflow:
1. Read all files in `new-information/` (excluding `processed/` subfolder)
2. Analyse each file and integrate into the relevant `information-base/` documents
3. Update `08-ronalds-plans-and-suggestions.md` if it contains proposals from Ronald
4. Update `09-action-items.md` if Grant needs to respond to anything
5. Update `05-risks-and-open-items.md` with any new risks, decisions, or open items
6. Update `04-transition-timeline.md` if there are timeline-relevant items
7. Update `01-executive-summary.md` if the overall picture has changed
8. Move processed files to `new-information/processed/`
9. Report back what was processed and flag items requiring Grant's attention

## Information Base Documents

| File | Purpose |
|------|---------|
| `01-executive-summary.md` | High-level situation overview, critical dates, Grant's active response queue |
| `02-ronald-mushonga-profile.md` | Ronald's background, contract terms, phased deliverables |
| `03-entity-structure.md` | All 7 Sanctura entities, banking, payment workflows, service providers |
| `04-transition-timeline.md` | Completed/upcoming milestones, handover status, contract phase visual |
| `05-risks-and-open-items.md` | Risk register, pending decisions, open questions, decision log |
| `06-people-and-responsibilities.md` | Roles, responsibility matrix, escalation paths, decision rights |
| `07-compliance-calendar.md` | Monthly/bi-monthly/annual compliance tasks and known gaps |
| `08-ronalds-plans-and-suggestions.md` | Tracker for all of Ronald's proposals with Grant's review status |
| `09-action-items.md` | Grant's response queue with detailed analysis and suggested approaches |

## Key Rules

- **Ronald's title is "Interim CFO"** - not "CFO" or "Chief Financial Officer". Correct this in any draft communications.
- **Patient care override** - Any financial controls, spend freezes, or approval thresholds must explicitly exclude urgent/critical patient care. James (CEO/Lead Doctor) has full discretion on clinical spend. Sanctura is a medical clinic - process must never delay care.
- **Ronald requires Grant's approval** before contacting external parties or sending communications that establish authority/controls.
- **UK matters route through Amanda** (Practice Manager, UK) - Ronald coordinates with her rather than contacting UK suppliers/partners directly.
- **Output files** (draft responses) should be prefixed with `yyyy-mm-dd` date format.
- When reviewing Ronald's proposals, distinguish between finance function work (his lane) and commercial/clinical decisions (Grant/James territory). Ronald can analyse and recommend; Grant/James decide.
