# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a **Dynamics 365 Finance & Operations (D365 F&O) Solution Designer** knowledge base. It contains consolidated documentation, configuration analysis, parameter references, and operational frameworks for D365 F&O implementations — primarily supporting the Falco/Prime ERP support context.

There is no application code, build system, or test suite. The repository is a structured collection of text-based knowledge files.

## Repository Structure

- **Root level**: Cross-cutting knowledge files and the requirements compliance matrix (Excel)
  - `GL_param1` / `Source/GL` — General Ledger documentation and parameters
  - `04_PMA_Posting_DeepDives_AssetMgmt.txt` — Posting profiles, asset management deep dives
  - `05_Frameworks_ReportCatalogs_Templates.txt` — Support case analysis templates (S01), sign-off sheets, WMS/Inventory and Financial report catalogs
- **Source/ProjectManagement/** — Project Management & Accounting (PMA) parameter analysis split into two parts:
  - Part 1 (Params 1-10): Line properties, project groups, funding limits, journal defaults, hour/expense/item forecasting
  - Part 2 (Params 11-20): Fixed-price POC configuration, project categories, indirect costs, expense policies, timesheet analysis, cost templates, resource roles, project contracts
- **Source/Production/** — Production module (placeholder, minimal content)

## Knowledge Base File Convention

Files follow a numbered, consolidated format:
- Header block identifies the file number (1 of 5, 2 of 5, etc.), contents summary, original sources, and consolidation date
- Sections are delimited by `========` source file headers
- Content originated from a consolidation on **2026-02-16** from multiple source documents

## Key Domain Concepts

- **Falco / Prime**: The D365 F&O client instances being supported. The knowledge base contains handover briefs, support case templates, and troubleshooting context for these environments.
- **PMA (Project Management & Accounting)**: The core D365 module covered in depth. Configuration parameters are analyzed with functional definitions, operational impact, accounting/subledger impact, and business decision advice.
- **POC (Percentage of Completion)**: The revenue recognition framework documented for fixed-price projects (Cost-to-Cost method, IAS 15 / ASC 606 compliance).
- **WIP (Work in Progress)**: Balance sheet accounting treatment for project costs and accrued revenue prior to invoicing.
- **S01 Analysis**: A structured support case email thread analysis template producing a single-table output with strict evidence-based governance rules.

## Working with This Repository

When answering questions using this knowledge base:
- Use ONLY information explicitly present in the files; never invent D365 navigation paths, field labels, parameter names, tables, or batch job names
- If information is missing or unclear, state: "Insufficient data to verify"
- Maintain British English conventions consistent with the existing documentation
- Respect the numbered file organization (Files 1-5) when referencing source material
