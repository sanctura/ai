# Stock Management Initiative

## Project Overview

A stock management initiative for a UK-based integrative medicine practice, led by MO and Grant. The goal is to improve efficiency in ordering supplies, managing supplier relationships, maintaining stock levels, and ensuring regulatory compliance for importing health products into the UK.

## Current State

- **Accounting Platform**: Xero (partially adopted for inventory management)
- **Stock Management**: Nurses perform periodic stock takes and order on demand
- **Inventory Source**: Last export from Xero (see `background-information/Inventory-list.csv`)

## Key Objectives

1. **Streamline ordering** - Establish efficient processes for ordering new stock and managing reorder levels
2. **Supplier management** - Improve workflows with suppliers, particularly for imported products
3. **System adoption** - Better utilise Xero's inventory features or identify a more suitable solution
4. **Regulatory compliance** - Understand and comply with UK import regulations for supplements and IV medications
5. **Process definition** - Document clear SOPs for pharmacy management

## Project Structure

```
mo-stock-management/
├── README.md                          # This file - project overview
├── background-information/            # Original source materials
│   ├── initial-info.md
│   ├── prompt.md
│   └── Inventory-list.csv
├── docs/
│   ├── inventory-analysis.md          # Analysis of current inventory
│   ├── stock-categories.md            # Product categorisation breakdown
│   ├── regulatory-considerations.md   # UK import & licensing notes
│   └── system-options.md              # Software/plugin options to explore
└── processes/
    └── stock-management-workflow.md    # Proposed workflow & SOPs
```

## Inventory Summary

- **Total SKUs**: 157
- **Tracked items** (physical stock managed): 78
- **Untracked items** (services, lab tests, fees): 79
- **Item categories**: IV Concentrates/Medications, Oral Supplements, Lab Tests/Pathology, Consultations/Services

## Regulatory Context

- Oral vitamins and supplements are generally **not classified as medications** in the UK
- IV vitamin infusions **may be classified as medications** and could be subject to import licensing (MHRA)
- Import licensing requirements need to be confirmed for each product category
