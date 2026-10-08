# TJM Client Progress Report Skill

Create a client-friendly, branded report connecting customer feedback to verified improvements. This is for client progress updates, not automatic daily metrics emails.

## Use it

Ask your assistant to install this skill:

> Install the create-client-progress-report skill from https://github.com/seifhany-tjm/create-client-progress-report. Its SKILL.md is at the repository root.

Install the complete `create-client-progress-report` folder in your assistant's skill directory, keeping its assets and references together. Then ask:

> Use create-client-progress-report to prepare a progress report for our client. Here is their issue document. Check the fixes and compare performance before and after the recent release.

If you do not have an issue sheet:

> Use create-client-progress-report for our client. Find their feedback in Linear, trace the recent fixes, and prepare a branded update with verified improvements and upcoming work.

## What it asks for

- Client/bot and an issue sheet, Google Doc, or feedback link; otherwise the relevant Linear project.
- Reporting period and any previous report.
- Relevant repository/release evidence and Axiom access, where not discoverable from context.
- Desired output, normally an editable Google Doc and PDF.

## What it does

Reads feedback and comments, traces changes and their release/verification state, compares suitable before/after measurements, and explains the outcome in client-level language. It includes additional improvements and real next steps, while distinguishing new fixes from existing safeguards, clarified requirements, and pending work.

The TJM logo, brand guide, report outline, and fictional writing example are bundled. No access to a previous client's documents is required. The assistant uses available connectors or computer use; if an integration is unavailable, it asks for the missing export and continues with supported evidence. Without document tools, it can deliver a complete Markdown report.

## Evidence and privacy

The assistant keeps a private evidence ledger separate from the client report. Missing metrics or deployment evidence are disclosed, not invented. Do not put client documents, patient information, API keys, or private evidence in this skill folder. Creating the report does not automatically send it or change issue statuses.

## Contents

- [Workflow](SKILL.md)
- [Evidence and measurement rules](references/evidence.md)
- [Branding and report design](references/report-design.md)
- [Report outline](assets/report-outline.md)
- [Fictional example](assets/sample-report.md)
- Bundled assets in `assets/brand/`
