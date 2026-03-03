# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

This is a documentation-only project (no code/builds/tests) managing the GoHighLevel (GHL) CRM setup for ShiftOne Digital's UK and South African clinics. It tracks workflows, configuration decisions, and communications with the implementation partner.

## Repository Structure

- `background/` — Original project brief and workflow specifications. **Do not modify these files.**
- `information-base/` — Living reference documents (numbered 01–06). These are the primary knowledge base and should be updated as new information arrives.
- `output/` — Drafted communications and deliverables, prefixed with `yyyy-mm-dd`.

## Key Conventions

- **Output files** must be prefixed with the date in `yyyy-mm-dd` format.
- **Information base** documents are numbered for ordering. When adding new topics, continue the numbering sequence.
- **Changelog** (`information-base/06-changelog.md`) should be updated whenever information-base documents are modified.
- **Open items** (`information-base/05-open-items-and-decisions.md`) tracks unresolved questions and confirmed decisions — update both tables as items are raised or resolved.

## Domain Context

- Two clinic locations: **UK** and **SA** (South Africa), running on a single GHL license.
- Two core workflows: "Front Desk Launchpad" (inquiry → consultation) and "Clinical Conversion Cycle" (consultation → treatment).
- All patient communication is **manual** — no automated emails/SMS to patients.
- Internal staff notifications/reminders are acceptable automation.
- The bridge between Workflow 1 and 2 is the `Pre-Consult Doc Link` field — it must be populated before a lead transitions.
- Key people: Grant Merwitz (global lead), Kyle Bennet (SA manager), Amanda Ross (UK manager).
