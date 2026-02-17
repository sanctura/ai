# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Type

This is a **documentation and planning repository** — not a software project. There are no build tools, package managers, tests, or application code. All content is markdown documents and one CSV data file.

## What This Project Is

A stock management initiative for a UK-based integrative medicine practice, led by MO and Grant. The repository contains analysis, process documentation, regulatory research, and project planning for improving how the practice manages ~78 physical stock items (IV concentrates and oral supplements).

## Repository Structure

- `background-information/` — Source materials: original brief (`initial-info.md`, `prompt.md`) and the Xero inventory export (`Inventory-list.csv`, semicolon-delimited, 157 SKUs)
- `docs/` — Analysis and research: inventory breakdown, stock categories, regulatory considerations (UK/MHRA), system/software options
- `processes/` — Workflow designs and SOPs
- `output/` — Deliverables for stakeholders (summary and detailed task plans)

## Key Context

- **Xero** is the existing accounting platform (partially adopted for inventory)
- Item codes: `CON1xxx` = IV concentrates/injectables, `SUP1xxx` = oral supplements
- 78 tracked physical items, 79 untracked services/tests
- German-sourced IV products (Pascoe, Kohler, Burghardt) have MHRA import licensing implications
- Controlled drugs in inventory: Modafinil (Schedule 4), Nebido (testosterone)
- Two active workstreams: **A) Stock Management Process** (document current → propose new) and **B) Regulatory & Legal Adherence**

## Working Conventions

- All documents are markdown — keep formatting consistent with existing files
- When analysing the inventory CSV, note it uses semicolons as delimiters
- Purchase prices in Xero are mostly £0.00 (a known data gap)
- Use British English spelling (e.g., "categorise", "licence", "organised")
