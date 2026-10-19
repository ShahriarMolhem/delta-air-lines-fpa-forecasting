# Delta Excel Model | Assumptions, Mechanics and Artifact Status

## Workbook available in this repository
[Download the Excel FP&A model](delta_air_lines_fpa_model.xlsx) — nine worksheets, approximately 202 formula cells. The GitHub file matches the locally prepared workbook by Git blob hash and passed ZIP package integrity checks.

The companion Excel includes historical GAAP operating results, operating KPIs, an FY2024–FY2025 expense bridge, a driver-based FY2026–FY2028 forecast, scenario sensitivity and calculation validation.

## Calculation mechanics
- Passenger sales forecast = modeled ASM × modeled passenger revenue per ASM. Remember amounts are in **millions** and cents/ASM must be converted correctly.
- Cargo sales and Other revenue use separate student-selected growth assumptions.
- Fuel gallons forecast = preceding period gallons × ASM growth adjusted for assumed improvement in gal/ASM.
- Fuel expense = modeled gallons × modeled implied dollar expense per gallon.
- Labor expense = forecast ASM × modeled labor cost per ASM.
- Residual expenses = forecast ASM × modeled consolidated nonfuel/nonlabor cost per ASM.
- Modeled operating income = forecast consolidated revenue − all modeled consolidated operating expenses.
- Sensitivity cell = unshocked FY2026 EBIT + change in modeled passenger yield revenue − change in modeled fuel expense.

## Checks
- Historical GAAP 2021–2025 revenue and operating expense reconciliations: zero differences.
- FY2024–FY2025 operating income bridge: −$173m.
- Base FY2026 operating revenue: $65,638m (rounded).
- Base FY2026 modeled operating income: $5,257m (rounded).
- Zero-shock sensitivity cell: $5,257m.
- Workbook was locally checked for common formula errors; local formula inspection is not an external financial audit.

## Release dependency
Both binary files have been uploaded to their respective folders on the release branch and verified by byte-for-byte Git object identity and archive integrity. The repository must remain **Private** until owner review and explicit approval to publish.

## Disclosure
All FY2026–FY2028 projections are student-created **illustrative assumptions**, not Delta-issued guidance, internal budgets, or assertions about future earnings.
