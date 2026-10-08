# Client report structure, voice, and TJM design

## The reference pattern

The inspected reference was a two-page client update: original TJM logo at the top, purple report title, a reporting-period line with date chips, one prominent processing-time comparison, a three-column issue table, and short additional-improvement sections. Reuse this visual and editorial pattern. Do not import the prior client's name, figures, issue details, status labels, source links, or dates as facts for another report.

The package is a research/reporting workflow, not a frozen copy of that historical document. Use [the outline](../assets/report-outline.md) for new reports and [the synthetic example](../assets/sample-report.md) for tone. A supplied native template governs structure when the user asks to preserve it; follow the document tools' native copy/adaptation workflow and keep its source unchanged.

## Bundled assets and visual system

Use [the original logo](../assets/brand/tjm-logo.png) and [the brand guide](../assets/brand/brand-guidelines.pdf). They are bundled; teammates need no Drive access or separate metrics-report installation.

| Role | Treatment |
|---|---|
| Primary accent | Purple `#5C288F` |
| Secondary accent | Lavender `#E9DFFC` |
| Body text | Charcoal `#2E2E2E` |
| Alternating table rows | White / light gray `#F4F4F5` |
| Subtle rules | Warm beige `#D9D4CC` |
| Report title / section headings | DM Serif Display; Georgia fallback |
| Body, tables, numeric headline | Inter; Arial/Helvetica fallback |

The reference uses Letter pages, 48 pt left/right margins, 54 pt top and 42 pt bottom margins. Title: about 27 pt. Section headings: about 15 pt. Body: about 10–11 pt; table: about 9.5–10 pt. The headline number is about 23 pt with a smaller comparison label. These are starting values, not a reason to squeeze a long report into two pages.

Preserve the logo's aspect ratio, colors, and clear space. Use a compact original wordmark near the top; keep headers inside printable bounds. No regenerated logo, decorative stock imagery, or branding rediscovery is needed.

Use a purple table header with white bold labels, alternating neutral rows, and comfortable cell padding around 7 pt. Suggested column widths are 28% concern, 20% status, and 52% resolution/evidence; adapt to content. Avoid blank trailing rows, unnecessary border grids, and splitting a short issue row over pages. Repeat table headings when a table continues. Prefer an extra page to unreadable type.

## Content order

**Opening:** small “TJM LABS / CLIENT PROGRESS REPORT” label, client/bot title, exact reporting period, and one to three useful outcomes. Include the implementation/release span if established. Use a measured headline when comparable evidence exists; otherwise lead with concrete delivered capabilities. Do not force a percentage into every report.

**Issues report:** use the columns “Client concern,” “Status,” and “What changed / evidence.” Keep a stable issue reference where it helps the client map back to their feedback. Each resolution describes the corrected behavior and a short verification statement. Distinguish “implemented,” “available,” and “checked in use” in plain language.

**Additional improvements:** short benefit-led headings followed by one sentence about what changed. Include genuine delivered work beyond the original feedback; avoid duplicating issue rows merely to make the report look larger.

**Upcoming work / next steps:** real planned work, unfinished verification, or a clear client decision. Keep it separate from completed improvements, with dates only when confirmed. Omit empty sections.

The report can normally be one or two pages. Cover all relevant client concerns first; extend the document when needed. An issue table can carry the resolution and evidence without adding a technical methodology section. Put exact comparison dates, units, sample sizes, and any material limitation in a small adjacent caption instead of an unrelated disclaimer footer.

## Client-level wording

Lead with the change the client can observe. Describe a technical mechanism only when it explains a useful outcome.

| Internal implementation description | Client-facing wording, when supported |
|---|---|
| Added field parsing and validation | Address details now appear in the correct fields. |
| Added idempotent retry handling | Interrupted work can resume without creating duplicate records. |
| Added UI readback after saving | The bot checks that the saved details match the intended values. |
| Removed repeated lookups | Processing requires fewer repeated searches; include a measured speed result only if established. |
| PR merged; deployment unknown | The update is implemented; availability in your workflow is being confirmed. |
| Tracker says fixing; team reports a test pass | The team reports the fix passed testing; the tracking entry still needs reconciliation. |

Do not promise error-free operation, guarantee clinical correctness, or describe code changes alone as measured safety/performance gains. Avoid bare “Fixed / tested” when the test scope or release state is still unresolved. If a requirement was clarified, explain the clarification without portraying it as a bug fix.

## Final quality check

Check every issue's status against evidence, recalculate the headline from unrounded aggregates, confirm report/comparison dates and sample definitions, and ensure no old client facts survived adaptation. Remove raw logs, commit hashes, internal-only links, personal data, placeholders, and blank rows from the client copy. Maintain a separate private evidence ledger.

For a native Google Doc, read it back after editing and preserve necessary date chips, table roles, and tab structure. Export the actual result to PDF, render every page, and inspect page breaks, headers, text wrapping, table continuity, logo proportions, and legibility. A successful export or a text extraction alone does not establish visual quality. If rendering is unavailable, state that visual review remains incomplete.
