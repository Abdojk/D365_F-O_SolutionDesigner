# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a **Dynamics 365 Finance & Operations (D365 F&O) Solution Designer** knowledge base. It contains consolidated documentation, configuration analysis, parameter references, and operational frameworks for D365 F&O implementations — primarily supporting the Falco/Prime ERP support context.

There is no application code, build system, or test suite. The repository is a structured collection of text-based knowledge files.

## Knowledge Base File Map (Files 1–5)

All content was consolidated on **2026-02-16** from multiple source documents into a numbered 5-file series:

| File # | Path | Coverage |
|--------|------|----------|
| 1 of 5 | `Source/GL` (also at `Source/General_Ledger/GL Param`) | Memory Bank Core — WMS deep-dive, GL documentation, AP parameters, Falco/Prime support handover context, posting types |
| 2 of 5 | `Source/ProjectManagement/02_PMA_Parameters_Part1_Params1to10` | PMA Parameters Part 1 — line properties, project groups, funding limits, journal defaults, hour/expense/item forecasting |
| 3 of 5 | `Source/ProjectManagement/03_PMA_Parameters_Part2_Params11to20.txt` | PMA Parameters Part 2 — fixed-price POC configuration, project categories, indirect costs, expense policies, timesheet analysis, cost templates, resource roles, project contracts |
| 4 of 5 | `Source/ProjectManagement/04_PMA_Posting_DeepDives_AssetMgmt` | PMA ledger posting framework deep-dives (fixed-price vs T&M, inter-company, WIP reversal, advanced revenue recognition) + Asset Management (EAM) preventive maintenance |
| 5 of 5 | `05_Frameworks_ReportCatalogs_Templates.txt` | Operational frameworks — S01 support case analysis template, sign-off sheet template, WMS/Inventory report catalogue, Financial reports catalogue |

Other paths:
- `Source/Production/` — Production module placeholder (minimal content)

## Knowledge Base File Convention

- Header block identifies the file number, contents summary, original sources, and consolidation date
- Sections are delimited by `========` source file headers
- Within each file, individual source documents are separated by `SOURCE:` lines beneath the delimiter

## Key Domain Concepts

- **Falco / Prime**: The D365 F&O client instances being supported. The knowledge base contains handover briefs, support case templates, and troubleshooting context for these environments.
- **PMA (Project Management & Accounting)**: The core D365 module covered in depth. Configuration parameters are analysed with functional definitions, operational impact, accounting/subledger impact, and business decision advice.
- **POC (Percentage of Completion)**: The revenue recognition framework documented for fixed-price projects (Cost-to-Cost method, IAS 15 / ASC 606 compliance).
- **WIP (Work in Progress)**: Balance sheet accounting treatment for project costs and accrued revenue prior to invoicing.
- **S01 Analysis**: A structured support case email thread analysis template producing a single-table output with strict evidence-based governance rules.
- **EAM (Enterprise Asset Management)**: Preventive maintenance work orders documented with three architectural paths (OOB, Power Platform, X++).

## Working with This Repository

When answering questions using this knowledge base:
- Use ONLY information explicitly present in the files; never invent D365 navigation paths, field labels, parameter names, tables, or batch job names
- If information is missing or unclear, state: "Insufficient data to verify"
- Maintain British English conventions consistent with the existing documentation
- Respect the numbered file organisation (Files 1–5) when referencing source material
- When citing information, reference the specific file number and SOURCE section (e.g. "File 3 of 5, SOURCE: PMA_Pamaters_11.txt")
