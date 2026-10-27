# Workplace Operations Command Center

**Public interactive portfolio application** — management dashboard, fictional budget challenge, vendor operations, staffing, hospitality, events, and executive analytics.

Open `index.html` or enable GitHub Pages from `main` / `(root)`.

# Workplace Operations Command Center — Version 3 (Phase 1)

**Independent workplace services portfolio case study, with simulated data only.** Not affiliated with potential employers. No performance or financial results are claimed as actual employment outcomes.

## Modules
- Facilities budgeting: FY2026 illustrated operating plan, month/category variance, scenario modeling, CSV export.
- Vendor performance: weighted quality, timeliness, responsiveness and cost metrics; intervention categories.
- Invoice exception review: synthetic purchase order match, duplicate checks, vendor and receipt checks, overspend alerts.
- Work-order SLAs: priority-specific response and resolution clocks as of fixed 2026-10-24 12:00 UTC.
- **V3 Procurement & Contracts:** synthetic contract register with renewal and insurance expiration alerts; RFQ comparative sourcing (40% price, 35% quality, 25% delivery); savings comparison against prior quoted annual pricing; vendor risk signals; downloadable contracts.

## Test it
Open `index.html` in any modern browser. It uses local CSS and JS and no network requests. Select **Procurement & contracts**. Add bids, reject duplicate RFQ/vendor pairs, add a contract and see metrics update; export CSV. In Budget, **Reset demo** clears local changes across modules. No server or credentials are required.

## Management caveats
- Fully fictional organizations, events, scores, spend and dates.
- Contract figures are not automatically booked to actuals, accounts payable or PO limits. The data models illustrate management controls, not production-grade accounting.
- Prior quoted price minus contract value represents *illustrative negotiated price improvement*, not cash savings achieved.
- RFQ price comparisons assume comparable scope; evaluation is advisory, not automatic contract authorization.
- Renewal alerts use a fixed as-of of 2026-10-24, including expiry at 60 days and insurance at 30 days; expired statuses take priority.
- All changes stay in your browser via localStorage; no authentication, audit trail, live collaboration, or real vendor data.

## GitHub Pages
Publish repository `/` or copy this folder's files to a GitHub Pages source directory. The `index.html` relies on adjacent `app.js` and `styles.css`.

## Future phases
2. Team supervision/coaching. 3. Employee experience/hospitality. 4. Event operations. 5. Integrated executive analytics and controlled record relationships.


## V3 Phase 2 — Team performance & coaching (2026-10-24)

- Simulated four-person staff roster with capacity hours, task completion counts, quality inputs, training deadlines, development goals.
- Workstream assignment form, cumulative workload utilization calculation, per-person over-allocation warning.
- Coaching action log with focus area, next steps and follow-up date; CSV export and local reset.
- The team uses invented identities and static scenario metrics, not real personnel records or evidence of actual people management.
- Example measurement date is fixed at 2026-10-24 for deterministic results.
- Metrics are decision-support prompts, not employee evaluations or substitutes for supervisory judgment.
- LocalStorage stores demonstration edits only; avoid entering personal or sensitive data.

### Phase 2 acceptance checks

1. Assigned hours aggregate by employee and across team.
2. An assignment above capacity raises an over-allocation flag.
3. Training due dates prior to 2026-10-24 are flagged overdue.
4. Coaching logs save, render and survive local refresh.
5. Reset restores fictional sample.
6. Team CSV exports workload and quality indicators.

## Phase 3: Workplace hospitality and employee experience

The interactive dashboard adds fictional employee service requests (owner, due date, status), feedback scores and documented service-recovery actions, plus simulated amenity-readiness inspections. Low scores of 1–2 require a follow-up action. KPIs include overdue open requests, mean satisfaction among rated requests, low-score counts and amenities needing attention. Records can be edited, exported as CSV and reset using browser-local storage. Fixed evaluation date: 2026-10-24. This is a portfolio demonstration, not potential employers data or evidence of actual employee survey performance.


## Phase 4 — Event Operations & Budget Management

Adds event requests, approved budgets, fictional vendor/PO commitments, staff allocations, budget-variance and capacity warnings, closeout expenses, attendance, optional attendee feedback, CSV export and reset. The event register is simulated and persists only in browser localStorage. Fixed evaluation date: 2026-10-24. Completed-event actuals replace commitments for event exposure, rather than being added to them. Event costs do **not** automatically post to existing budget or invoice ledgers; PO identifiers are demonstrative and do not authorize expenditure. The portfolio demonstrates decision rules, not actual potential employers operations.


## Phase 5: Executive management analytics

Executive overview integrates rules-derived risk flags from annual budget modeling, vendor scorecards, contract alerts, team capacity (including planned event hours), employee requests, amenities, and event exceptions. Risks are ranked High/Medium/Low. Users can record an accountable owner, decision, due date and status, and export the exception register to CSV. Dashboard recomputes when opened. Notes are stored locally in the browser. All data and conclusions are fictional and illustrate decision controls only; events are not double-counted into operating budget actuals and invoices are not approved through the dashboard.


## Debug and release audit (2026-10-24)
- Restored and verified canonical five-module HTML source on this branch; earlier GitHub source was behind the local complete release.
- Corrected executive contract exceptions to use `Monitored` for healthy contracts.
- Corrected expired insurance / contracts severity detection to case-insensitive matching.
- Static validation: 153 HTML identifiers checked against 143 JavaScript static references, zero missing, JavaScript syntax passes.
- Interactive Chromium testing was blocked by this runtime's administrator navigation policy; browser acceptance testing and GitHub Pages setup remain pending.
- `workplace-operations-v3/index.html` is the canonical all-in-one app; all data is simulated.


## Fictional-data and non-affiliation disclaimer

Disclaimer: This is an independent, fictional portfolio demonstration. All names, company names, vendors, employee profiles, financial figures, events, and operational records are provided solely for illustrative purposes. Any resemblance to real persons or organizations is coincidental. No affiliation, endorsement, employment relationship, or connection with any real company is stated or implied.


## Public engagement experience (portfolio branch root)

The branch-root `index.html` adds a no-login landing screen, navigation to the full dashboard, and a fictional Budget Optimization Challenge. Visitors select cost interventions, view scenario savings and risk scores, save choices locally in their own browser, and export a decision report to CSV. An external feedback link opens the repository's GitHub Issues page (posting requires a GitHub account). This is illustrative training content, not professional financial advice or real workplace results. GitHub Pages must be configured separately to publish this branch root.


## Reports & Downloads Center

The `Reports & downloads` tab provides one-click access to existing CSV exports across the ten dashboard categories, an editable fictional sample budget CSV, and four printable management summaries (Executive, Budget, Vendor, Budget Challenge). The report is downloaded as a self-contained HTML document; open it in a browser and use Print → Save as PDF. This is **not direct PDF generation**. Reports reflect simulated dashboard indicators and are not certified financial or operational statements. No server-side data collection or external analytics is implemented.


## Forecast model and direct PDF downloads

The Budget Forecast estimates full-year operating spending using a selected number of observed months from fictional records. Each remaining month is projected as: monthly plan × observed actual/plan ratio × (1 + inflation assumption) + monthly cost adjustment, floored at zero. Lower- and higher-cost cases vary future estimates only. The forecast can be downloaded as CSV.

The Reports & Downloads Center generates PDF summaries directly in the browser for executive, budget, vendor, challenge, and forecast views. PDF exports use a simple built-in text-based renderer and are not audited reports. All scenario records and values are invented for illustration and are not related to actual companies.


## 12-month forecast visualization

The budget forecast now includes a responsive SVG chart with the monthly approved plan, recorded spend through the selected cutoff month, future baseline forecast, and a shaded scenario variation envelope. Chart values recalculate from the same `forecastData()` output as the table and CSV whenever assumptions change. Example records are fictional; later months in the fictional FY2026 may be treated as scenarios, not observed financial results. Full live-browser acceptance testing is still pending.


## Executive forecast assessment

The Budget Forecast now generates a year-end over/under-plan assessment, ranks up to three expense categories with positive projected variances, and suggests prioritized management follow-ups with a CSV action export. Forecast category allocation uses the observed aggregate actual-to-plan ratio and distributes optional monthly extra costs in proportion to category plan. It is a simulated, assumption-driven model; action suggestions do not indicate that contracts were renegotiated or spending actually saved. Recalculate when changing assumptions. Browser interaction validation is still pending.


## Forecast accuracy and continuous improvement

The forecast module can save immutable forecast assumptions/values as local snapshots for months not yet observed. As the observed-through month moves forward, it evaluates those saved future-month predictions against the current fictional budget actuals. It reports MAE (average absolute dollar error), MAPE (mean absolute percentage error over nonzero actual months), WAPE (total absolute error divided by absolute actual total), and mean signed error (forecast minus actual). If there are no eligible actual months, results are N/A; zero actuals are excluded from MAPE. Visitors can select/delete snapshots and export a comparison CSV. Snapshots are stored in browser localStorage and are not server-backed, independently verified or linked to accounting records. No automatic historical backtest or timestamp attestation is claimed.


## Community launch and forecast comparison

The Forecast Accuracy panel shows saved forecasts versus later simulated actuals, alongside a monthly approved-plan baseline calculated over the identical evaluated months. This is a descriptive baseline, not a validated forecasting competition. See [CONTRIBUTING.md](CONTRIBUTING.md) and [COMMUNITY.md](COMMUNITY.md). Starter issues: [Forecast tests](https://github.com/StiliIlist/workplace-operations-command-center/issues/1), [Accessibility](https://github.com/StiliIlist/workplace-operations-command-center/issues/2), [Method comparison](https://github.com/StiliIlist/workplace-operations-command-center/issues/3).

To publish the site, configure GitHub Pages under Settings > Pages: deploy from branch `main`, folder `/(root)`. Publication and live-browser acceptance testing must be verified separately.


## Forecast accuracy visualizations and comparison

The Forecast Accuracy section includes a forecast-versus-actual SVG line chart, monthly absolute-error trend, and comparable MAE/WAPE scores against the approved monthly budget. New snapshots also preserve the pre-cutoff observed monthly mean as a third baseline, so it is evaluated without using future data. Older snapshots lacking this preserved historical mean show only available comparisons. Figures use fictional data and browser-local state. Results require future months to be marked observed, and do not demonstrate verified real-world forecasting improvement.


## Quality audit — 2026-10-26

Static source checks found no duplicated literal HTML IDs and no missing IDs among direct `getElementById`, `faEl`, `$fc`, `byId`, and `execEl` references. Mobile improvements: horizontally scrollable sticky tab navigation, single-column layouts for narrow screens, responsive forms, keyboard focus indicators, and reduced-motion support. JavaScript execution, PDF opening, CSV downloads, persistence, and full cross-module acceptance remain unverified in a live browser. GitHub Pages public accessibility could not be confirmed; do not promote the proposed URL as tested.


## Automated browser acceptance QA

A GitHub Actions workflow at `.github/workflows/browser-qa.yml` runs Playwright Chromium smoke checks on pushes to `main` and can be started manually from Actions. The checks cover landing navigation, budget challenge calculations, forecast rendering and CSV download, forecast snapshot/accuracy display, and report PDF/CSV downloads, plus uncaught browser errors. Inspect the latest Actions run before considering them passed. The workflow does not enable GitHub Pages; the public URL and complete financial correctness still require independent validation.
