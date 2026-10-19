# Development Plan | Four Genuine Review Milestones

**Repository:** `ShahriarMolhem/delta-air-lines-fpa-forecasting` · **Initial state:** Private.

| PR | Scope | Review requirement |
| --- | --- | --- |
| **1 — Research foundations** | Research design, original SEC 10-K references, methodology, project README | Confirm official data sources, terminology, and no-internal-budget boundary |
| **2 — Historical data** | FY2021–2025 GAAP and operating-driver datasets, operating-income bridge, reconciliation report | Reconcile every year's sales, expense, and GAAP EBIT; review FY2021 grant anomaly |
| **3 — Forecast & sensitivity** | Three-year driver-based forecast with editable assumptions, scenario analysis, Excel artifact handoff | Distinguish facts/forecasts, reproduce base forecast and sensitivity center |
| **4 — Present & release** | Executive summary, speaking script, PowerPoint, link and completeness checks | Verify communication quality and owner presentation readiness |

## Scope boundary
The aim is to show **BBA-level financial analysis and FP&A reasoning**, not pretend to have worked at Delta or accessed its private management budgets. Real data support historical analysis; forecast years are transparent author-selected hypotheticals.

## Packaging
The core reports belong in `.md` files, historical data in `.csv`, a formula-driven workbook in `.xlsx`, and a 10-slide presentation in `.pptx`. Large binary files may require one manual GitHub upload because this connector offers only text-file writes.

## Release rule
- Merge approved phase PRs in sequence.
- Keep the repository **Private** until historical checks pass, binaries are uploaded and verified, and the portfolio owner approves public release.
