---
name: create-client-progress-report
description: Create a TJM-branded, client-friendly progress report from client issue sheets, Google Docs and comments, Linear, implementation history, and Axiom before/after evidence. Use for reporting fixes, measurable improvements, delivery timelines, additional improvements, and upcoming work. This produces a client update, not a recurring metrics email or a technical incident report.
---

# Create client progress report

Help a teammate explain what improved for a client, what was done about their feedback, how the outcome was checked, and what comes next. Research the evidence, then produce a compact branded report. Emphasize demonstrated value without turning intended benefits, old safeguards, or unfinished work into new delivered improvements.

## 1. Gather the report inputs

Start with: **“Which client or bot is this for, and do you have an issue sheet, Google Doc, or client feedback link? If not, I can look for their reported issues in Linear.”** Reuse information already supplied instead of repeating questions.

Collect remaining decisions in short rounds:

- Reporting period, timezone, and any previous report. If the period is unknown, inspect the relevant feedback and implementation history, propose a start/end based on the recent fix cycle, and confirm it before calculating headline results.
- Issue-source links/files and any relevant comments or release notes; otherwise identify the client's Linear project/team. Read comments and replies as well as issue bodies.
- The relevant code repository and release/deployment evidence. Discover them from project context and linked issues when possible; ask only for unresolved choices.
- The Axiom dataset and bot/environment filters. Use connected access first. If unavailable, request a query-capable API key through secure input, or a bounded aggregate export; never ask for secrets in ordinary chat.
- Preferred output and destination. Suggest an editable Google Doc plus PDF, using the bundled TJM design. Reuse any client-supplied reference as requested; ask about audience only if it is unclear.

Do not request new brand assets for the standard TJM report. This package includes them. Do not ask the user to manually collect information that accessible connectors or repository history can resolve.

## 2. Build the evidence privately

Read [references/evidence.md](references/evidence.md) before researching. Begin with the supplied issue register or feedback. If absent, search Linear within the correct client/project and relevant time range; distinguish client-reported issues from internal enhancements. Inspect descriptions, comments/replies, attachments when relevant, links, and dated status changes. Page through results rather than treating a truncated response as complete.

Read relevant Google Doc tabs, sheet rows, and comments using available connectors; enumerate tab titles first and preserve the relationship between issue, expected behavior, resolution, and evidence. Use computer use if the needed read/export operation is unavailable through connectors. If neither works, ask for an export or pasted feedback while continuing independent work.

Keep a private working evidence ledger following the reference. For each distinct issue, connect the original concern to the actual code change, release state, and verification. Read relevant diffs and follow-up/revert changes, not only commit titles. Deduplicate recurring incidents without losing distinct concerns or source IDs. Reconcile conflicting status evidence instead of silently selecting the most favorable status.

Find relevant implementation work that predates the chosen period to establish when the fix cycle began. Keep reported date, first evidenced implementation, deployment, and verification dates separate. Include additional client-relevant improvements delivered during the period even if they were not original complaints, with the same evidence standard. Identify upcoming work from actual open issues/plans; do not invent a roadmap or promise dates.

## 3. Measure the result

Follow the Axiom and date rules in [references/evidence.md](references/evidence.md). Check the real schema and use explicit bounded periods, consistent counting units, populations, and deduplication. Pick comparable baseline and post-change windows around a verified release when available; keep their dates and sample sizes.

Calculate average processing time, absolute time saved, percentage time reduction, and relevant completion/reliability metrics only where the evidence supports them. Choose metrics that answer this client's concerns, rather than imposing a universal KPI set. Do not average daily averages without weighting. Do not cherry-pick a favorable day, exclude failures silently, or call observed timing changes proof of causation.

If there is no valid baseline, report the current measurement and say comparison is not yet available. If telemetry is unavailable, continue with verified issue resolutions and identify the missing measurement. “Implemented,” “released,” and “verified in use” are different claims. A successful workflow log is not independent correctness validation.

## 4. Write for the client and apply the design

Read [references/report-design.md](references/report-design.md) and adapt [assets/report-outline.md](assets/report-outline.md). Use this structure, expanding only as the evidence requires:

1. Client/report title, exact reporting period, and a concise evidence-backed performance headline or progress summary.
2. **Issues report:** client concern, current status, and plain-language resolution/evidence. Explain what changed and why it matters to the client.
3. **Additional improvements:** short benefit-led items supported by work delivered in the period.
4. **Upcoming work / next steps:** real unfinished work, remaining verification, or client decisions; include dates only when confirmed. Omit this section when there is nothing supported to include.

Explain the delivery span where known: when this set of improvements began and when it became available. Do not confuse calendar days covered by the report with days of engineering effort.

Use short, concrete statements such as “Address details now appear in the correct fields.” Keep branch names, hashes, stack traces, SQL, selectors, and raw log excerpts in the private evidence ledger. In the client report, describe the checks and their result; use discreet source links only when appropriate and accessible to that audience. Avoid unsupported adjectives, inflated impact, patient identifiers, and implementation detail that does not help the client.

Keep missing verification next to the affected claim, using plain language such as “Implemented; final checks pending.” Existing safeguards and clarified requirements may explain feedback, but do not count them as new fixes. Report neutral or worsened measurements honestly when material.

## 5. Create, check, and hand off

Use available document tools to create the requested artifact. For a user-supplied native Google Doc template, inspect its full tab structure, create a native copy, and adapt the content/styles without changing the source. Replace old client facts throughout the copy. Otherwise use the bundled design and outline to build a fresh document. Use the matching document/PDF skill when available; do not require teammates to have access to a historical client's document.

If document tools are unavailable, provide a complete client-ready Markdown draft and concise instructions for applying the bundled branding or importing it. Do not stop at a report outline or tell the user to do the research themselves.

Check that every in-scope client concern is covered, each status matches its evidence, dates and calculations agree, comparisons use the right population, and upcoming items are separate from delivered work. When exporting PDF, render and inspect every page for logo quality, readable tables, headers, wrapping, clipping, and awkward page breaks. Fix empty rows or formatting residue; never shrink the report until it becomes hard to read.

Return the report/source links and concise notes about any material missing evidence. Keep the detailed ledger separate from the client artifact. Creating a report does not authorize sending it, changing issue statuses, editing source feedback, deploying code, or altering live client data. Carry out separately requested sharing/delivery only within the user's stated scope.

## Sharing this skill

This is a standalone reporting workflow: all required guidance and TJM assets are bundled. Keep report-specific evidence, documents, screenshots, credentials, and client/patient details outside the skill folder. The historical report inspired the design, not the facts of future reports. Do not require a teammate to install the separate metrics-email skill.
