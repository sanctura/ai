# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a documentation repository for managing the fractional HR engagement between Saint Raphael Pty Ltd and OptiWorX360 (Pty) Ltd. It contains no code - only markdown documents, PDFs, and Excel files related to the HR services contract, proposals, and communications.

## Current Status

**Stage:** Amended proposal accepted - awaiting Siraaj's implementation timeline
**Provider:** OptiWorX360 (Siraaj Adonis, CEO)
**Original MSA Period:** October 2025 - September 2026
**Amended Scope (accepted 1 Mar 2026):** Payroll migration to PaySpace, leave management (ESS), employee contract alignment, ER support (35 hrs), reduced fractional HR at R850/hr
**Employee count:** ~15
**Additional cost:** ~R1,374/month more than original arrangement

## Repository Structure

- **background/** - Source documents: company profile (PDF), MSA proposal (PDF), emails, Excel proposals
- **information-base/** - Structured summaries and analysis (indexed by 00-index.md)
- **output/** - Generated communications and deliverables (emails, memos)

## Working with This Repository

- The `information-base/00-index.md` file serves as the master index linking all information-base files
- `information-base/06-key-context-decisions.md` tracks current status, open questions, and timeline
- Output files in `output/` must be prefixed with a date stamp: `yyyy-mm-dd-description.md`
- When adding new information, update the relevant information-base file and the index
- All financial figures are in South African Rand (ZAR) and exclude VAT unless stated otherwise
- Excel files require `openpyxl` to read programmatically (use a temp script file, not inline python, on Windows/bash)

## Key Financial Reference

| Item | Original | Amended |
|------|----------|---------|
| Hourly rate | ~R1,117 | R850 |
| Monthly fee | R12,653 | ~R14,027 (includes new services) |
| Hours used (Oct-Feb) | 60 | 60 |
| Total 12-month hours | 144 | Reduced fractional + new scoped services |
