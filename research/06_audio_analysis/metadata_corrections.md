# Step 6 Product Data Corrections / Pending Verification
Date: 2026-10-09
Status: OPEN DATA-QUALITY ACTIONS (not a reason to invent sound scores)

## Correction 1: FiiO FT1 PRO (C016)
- The existing data/candidates.csv says Release_Year=2025.
- DIY-Audio-Heaven measured/published the FT1 PRO on November 27, **2024**, and explicitly describes the product as launched November 2024.
- **Correction pending:** Release_Year=2024 (current CSV 2025 is stale).
- Primary supporting link: https://diyaudioheaven.wordpress.com/measurements/fiio/ft1-pro/
- Do not confuse the Korean Danawa listing/registration month in 2025 with global launch year.

## Correction 2: FiiO FT3 (C017)
- One CSV row 'FT3' covers at least **32Ω and 350Ω versions**, and these do NOT share identical tuning, diaphragm construction or electrical load.
- Until exact model/SKU and matching Korean price are resolved, treat FT3 acoustic comparison as **variant-unknown**. Do not assign 350Ω test measurements to 32Ω purchase candidate.
- Official FiiO references:
  - https://www.fiio.com/newsinfo/877944.html
  - https://www.fiio.com/newsinfo/825261.html
- Follow-up: split C017 into SKU-specific model rows or lock exact variant prior to any Step 8 delta or Step 9 price/performance verdict.

## Verification 3: aune AR5000 MK2 (C032)
- Reviewer's 2026 specification: impedance 64Ω (Pragmatic Audio).
- Headphones.com description: 28Ω.
- Until unambiguous manufacturer specification from product technical details/manual is verified, **Impedance_Ohm stays UNKNOWN**.
- https://www.pragmaticaudio.com/reviews/2026/05/aune-ar5000-mk2/
- https://headphones.com/products/aune-ar5000-mk2-headphones

## Interpretation
These are product-record hygiene issues. They do not justify rejecting the models or inventing quality differences. Step 6 audio matrix retains the evidence and marks confidence accordingly. The original candidate CSV must be synchronized when a permitted small patch/write route is available.
