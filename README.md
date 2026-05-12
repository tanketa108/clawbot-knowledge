# Clawbot Knowledge Bank

Canonical research knowledge base for Clawbot.

This repository is not just a document library. It is the persistent operating layer where Clawbot and its agents store, reuse, audit, and update investment research knowledge.

## Core principle

Reusable knowledge belongs above the company level.

- Sector-level knowledge lives in `research_bank/sectors/`.
- Company-specific knowledge lives in `research_bank/companies/`.
- Reusable analytical frameworks live in `research_bank/frameworks/`.
- Templates and workflows define how agents write into the bank.

## Repository map

```text
research_bank/
  sectors/      reusable sector knowledge
  companies/    company-specific research files
  frameworks/   cross-sector analytical frameworks
templates/      standard document templates
indexes/        navigation and active coverage indexes
workflows/      operating workflows for research updates
agents/         agent rules, permissions and review checklists
legacy_review/  temporary holding area for old Knowledge migration
```

## Operating rule

Before researching a new company, Clawbot must:

1. identify its sector,
2. read the relevant sector files,
3. reuse existing frameworks,
4. create only the company-specific delta,
5. update the sector bank if the new company produces reusable insight.
