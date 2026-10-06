# Changelog

All notable changes to the research methodology and project structure are recorded here.

## 2026-10-06 — Execution structure completed

### Added
- Split the master plan from stage-specific execution plans.
- Added `plan/00` through `plan/11` detailed stage specifications.
- Added explicit stage status, dependencies, inputs, exact tasks, minimum coverage, outputs, completion gates, prohibited shortcuts, and handoff requirements.
- Added data schemas for candidates, prices, evidence, and evaluations.
- Added reusable research templates, including stage plan, stage report, product review, source record, and handoff templates.
- Added decision and rejection logs.
- Added repository navigation and operating procedure.
- Added Public repository safety rules.
- Added recency rules: 2025~2026 recommendation/market material is preferred, while older stable measurements may still be used.
- Added source-access integrity rules so inaccessible original pages are never treated as directly verified.

### Changed
- `PLAN.md` now serves as the Master Index rather than duplicating every stage procedure.
- `STATUS.md` now points directly to the current stage detail file.
- Stage completion now follows a defined state transition and mandatory Gate review.
- Candidate discovery now explicitly includes Reddit, Head-Fi, professional measurement/review sources, Naver reviews, Korean community material, and Korea-market reverse discovery.
- Naver-style recommendation/ranking content is treated primarily as candidate-discovery evidence unless independently validated.

## 2026-10-06 — Initial setup

### Added
- Created the `audio-gear-research` repository.
- Defined the research project as an evidence-based upgrade investigation from Creative Sound BlasterX H7 + Sound Blaster AE-5.
- Added an 11-step research workflow.
- Added mandatory stage gates.
- Added rules separating product discovery, pricing, audio analysis, comfort analysis, H7 comparison, value analysis, and counter-review.

### Methodology Decisions
- MSRP and nominal discount percentage will not be used to determine product class or value.
- Korean real-world selling prices will be the primary price basis.
- Candidate discovery will use three independent paths: brand-based, community/expert-based, and Korea-market-based.
- Newer products receive preference only when price and performance are otherwise comparable.
- Long-term comfort, QC, support, replaceable parts, and product lifecycle will be explicitly evaluated.
- Final recommendations must pass a deliberate counter-review step.
