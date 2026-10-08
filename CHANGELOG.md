# Changelog

## 2026-10-09 — Step 6 acoustic analysis (REVIEW)

- User approved Step 5; created research/05_pre_filter/handoff.md and began Step 6.
- Created research/06_audio_analysis/result.md, acoustic_matrix.csv and additional_17.md covering all 29 PASS products (12 higher-priority and 17 medium-priority).
- Recorded 62 acoustic/source/technical evidence records E0227-E0288 and 29 structured rows in data/evaluations.csv.
- Kept Resolution/Separation/Imaging/Dynamics and all H7 comparison delta fields UNKNOWN absent consistent proof; use-case estimates marked low confidence.
- Documented reviewer contradictions (e.g. Audeze MM-100), rig/fit issues, treble versus perceived detail, and differing open-back/closed-back media tradeoffs.
- Flagged FiiO FT3 32/350ohm distinct versions, aune AR5000 MK2 inconsistent published impedance and FiiO FT1 PRO 2024 launch data correction in metadata_corrections.md.
- Candidates.csv 2025 date for FT1 PRO still requires synchronization; no final recommendation or move to Step 7 yet.
- Step 6 is REVIEW pending user approval.


## 2026-10-09 — Step 5 preliminary screening (REVIEW)

- Completed first-pass evidence-aware screening for all 62 candidates without deleting IDs.
- Classified 29 PASS (12 HIGH, 17 MEDIUM), 33 HOLD (2 HIGH, 12 MEDIUM, 19 LOW), and 0 REJECT.
- Compared candidate pairs including ATH-R50x/DT900 PRO X, FT1 PRO/ROG Kithara, K361/K371, SHP9500/SHP9600, and wired versus powered consumer ANC equipment.
- Created `research/05_pre_filter/result.md` and `research/05_pre_filter/triage.csv` with comparator IDs, individual reasons, evidence IDs, recheck questions and research priorities.
- Appended E0200–E0226 expert measurements, reviews, official AUX/analog support and current HD 6XX manufacturer status.
- Preserved high-end future-purchase candidates despite higher sticker prices; chose deferred investigation over unsupported acoustic or performance-per-price rejection.
- Deferred 19 low-priority HOLD candidates from first-wave deep research, focusing Step 6 on 12 PASS/HIGH models.
- Updated candidates.csv and rejection register; Step 5 remains REVIEW pending user approval.


## 2026-10-09 — Approved performance-per-price screening rule

- User approved Step 4 and authorized Step 5 to begin.
- Step 4 finalized with handoff, without treating old or cached asking prices as live confirmed checkout values.
- Updated RULES.md and Step 5 plan: high price alone does not disqualify a future purchase, but a clear **inferior performance-versus-cost** position can justify early REJECT if backed by consistent conditions, comparable lower-cost candidate(s) and at least two independent audio evidences.
- HOLD is the default where comparative evidence, live pricing, usage conditions or an offsetting strength remains uncertain.
- Candidate and rejection logs must preserve reasons, alternatives, confidence and reentry conditions; full Pareto/value analysis remains Step 9.
- Step 5 marked IN_PROGRESS, no candidates yet rejected on the revised methodology.

## 2026-10-09 — Step 4 Korean market price research (REVIEW)

- Recorded 133 separate Korean retailer/comparison-price observations and 62 candidate price summary rows.
- Observed 54 candidates with some Korean listing evidence; 47 have plausible listed new-product lows, 15 remain UNKNOWN.
- Derived conservative approximate typical **advertised** new-product prices only for seven candidates with clustered cross-portal evidence; all price stability UNKNOWN.
- Separated Korean genuine listing categories, imported offers, card/member conditional prices, stock-out, open-box/refurb and limited editions.
- Verified independent Enuri cross-checks for a subset of FiiO, Sony and Sennheiser while noting September refresh dates.
- Excluded sold-out HIFIMAN Korean official-store advertised prices from purchasable low comparison.
- Recorded Step 4 evidence E0143–E0199 and `research/04_price_research/result.md`.
- Price pages are non-live snapshots, and seller checkout/shipping/warranty confirmation remains pending for final purchase decisions.
- Step 4 held at REVIEW, no Step 5 started.

## 2026-10-09 — Step 3 Product Lifecycle Audit (REVIEW)

- Reviewed all 62 candidates against manufacturer catalog/support and Korean manufacturer distribution pages where available.
- Added 54 official evidence records E0089–E0142 and `research/03_product_status/result.md` containing a 62-product status matrix.
- Recorded 47 currently marketed/supported, 2 explicitly discontinued, 13 uncertain lifecycle.
- Corrected HD 480 PRO open/closed error; corrected AR3000 unverified exhibition-versus-retail launch status.
- Recorded 2026 JBL LIVE780NC successor and 2025 SteelSeries Nova7 Gen2; retained old generation candidates until pricing.
- Verified Sony Korea support for INZONE H6 Air; verified some manufacturer ear-pad/cable supply routes.
- Found conflicting HIFIMAN Korea warranty policy durations (1 versus 2 years depending language) requiring written confirmation.
- Kept per-model Korean official distribution UNKNOWN for 40 products where specific authorised channel was not confirmed.
- Lifecycle CURRENT now explicitly means currently manufacturer-marketed/supported, not verified ongoing manufacture.
- No product was removed or ranked; Step 3 is pending user review.

## 2026-10-08 — Step 2 bias correction

- Preserved the original 43 candidate records and identifiers.
- Expanded discovery outside the initial 15-brand audiophile map.
- Reviewed current mainstream gaming and consumer ANC products using 2026 RTINGS, SoundGuys, other expert sources and mixed-use community discussions.
- Rechecked Korean budget through upper-reference market examples using Danawa and official Korean retail where accessible. A separate 2025 Korean community listening roundup surfaced four further budget candidates validated against Danawa listings.
- Added 19 candidate records C044–C062 (total 62) and 35 evidence records E0054–E0088.
- Added `research/02_candidate_discovery/supplemental_review.md`; linked it from the original result and source matrix.
- Correctly flagged direct Naver access limitations and insufficient independent Enuri confirmation.
- Maintained Step 2 as REVIEW. Did not rank products or advance to Step 3.

All notable changes to the research methodology and project structure are recorded here.

## 2026-10-07 — Step 0 baseline prepared

### Added
- Confirmed current headset revision as Sound BlasterX H7 Tournament Edition.
- Recorded current 3.5mm analog → AE-5 headphone-output signal path.
- Added official H7 TE and AE-5 specifications.
- Added independent passive-mode measurement evidence and professional listening reviews.
- Added long-term comfort/material user evidence.
- Defined the qualitative H7 + AE-5 baseline for audio, comfort and use cases.
- Defined the later upgrade threshold and user-priority tiers.

### Data Model
- Added `USER_CONTEXT` evidence type for non-sensitive project inputs such as current hardware configuration and reported listening preferences.

### Status
- Step 0 moved to REVIEW.
- Product candidate research has not started.

## 2026-10-06 — Final structure audit

### Fixed
- Prevented Step 5 from rejecting candidates on price before deep audio analysis.
- Split seller-level price observations from candidate-level market price summaries using `prices.csv` and `price_summary.csv`.
- Aligned Step 8 H7 comparison fields with `evaluations.csv`.
- Distinguished bass quantity change from bass quality improvement.
- Added domain-level confidence fields for audio, use cases, comfort, QC, and H7 comparison.
- Added `Revision` and `Inventory_Age_Risk` to candidate lifecycle data.
- Replaced candidate-only evidence ownership with `Subject_Type/Subject_ID` so baseline, brand, market, and candidate evidence can all be recorded.
- Added source access status to prevent indirect search snippets from being treated as directly verified sources.
- Prevented Step 1 from writing premature product candidates before Step 2.
- Added explicit handoff file convention for every completed stage.
- Added a single source-of-truth rule for stage status to avoid status drift.
- Added Pareto/dominance-based value analysis and prohibited unsupported pseudo-precise value scores.
- Made Step 11 refresh price data and route newly discovered competitors back through the normal workflow.

### Result
- No known structural blocker remains before Step 0.

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

## 2026-10-06 — Initial setup

### Added
- Created the `audio-gear-research` repository.
- Defined the research project as an evidence-based upgrade investigation from Creative Sound BlasterX H7 + Sound Blaster AE-5.
- Added an 11-step research workflow.
- Added mandatory stage gates.
- Added rules separating product discovery, pricing, audio analysis, comfort analysis, H7 comparison, value analysis, and counter-review.
