# Step 3 — Product Status & Lifecycle

Date: 2026-10-09
Status: REVIEW
Scope: Existing candidates C001–C062 only. No product rankings, no price-based rejection.

## Interpretation of status

- **CURRENT** in candidates.csv = currently marketed/listed/supported by manufacturer's active channels; **not proof of ongoing production**, Korean in-stock inventory, or recently manufactured serial numbers.
- **DISCONTINUED** = official Korean manufacturer/support page explicitly marks discontinued.
- **UNKNOWN** = evidence insufficient to establish current-new-product marketing/supply or discontinuation.
- **Official_KR_Distribution = TRUE** only when a domestic model channel is evident; generic brand distribution alone does not establish model-specific Korean warranty or physical stock.
- **Parts_Availability = OFFICIAL_PARTS** means manufacturer lists actual replacement products or spare part numbers; **REPLACEABLE** means design/serviceability documented but no current Korean part-stock assurance.
- **Inventory_Age_Risk = UNKNOWN** means no verified manufacture date or age of remaining stock. **MEDIUM** for discontinued Philips models reflects possible old-stock exposure, not evidence that an actual seller holds aged units.
- Release years carried from Step 2 without new model-specific launch proof remain provisional; a year in the CSV must not be read as fully verified unless supported by a recorded source.

## Audit count

- 62 unique models assessed.
- 47 **CURRENT marketed/supported**.
- 2 **DISCONTINUED** by Philips Korea.
- 13 **UNKNOWN** lifecycle because reliable proof of current new-stock production or discontinuation was insufficient.
- 54 new Step 3 evidence records, E0089–E0142, from manufacturer/product/support sources.
- Original candidate IDs, discovery flags and notes preserved.

## Key verified corrections

1. **C005 Sennheiser HD 480 PRO** — originally mislabeled OPEN in Step 2; manufacturer officially launched **CLOSED-back** HD 480 PRO on **2026-04-21**. Data corrected; manufacturer lists detachable cable and Korean product page.
2. **C034 aune AR3000** — featured at the August 2026 audio exhibition. Exhibition does NOT demonstrate retail launch; previous `Release_Year=2026` overwritten to UNKNOWN pending sale date.
3. **C026 Philips Fidelio X2HR** and **C059 Philips SHP9600** — both officially **DISCONTINUED** on their Korean Philips support pages. Do not delete them before the actual market/value analysis.
4. **C049 JBL LIVE 770NC** — a newer **LIVE 780NC** generation was announced **2026-05-12** and has its own JBL Korea product page. An old page/seller listing does not demonstrate ongoing 770NC manufacture.
5. **C053 SteelSeries Arctis Nova 7 Wireless** — **Gen 2 released 2025-10-14**. Keep the earlier model as a separate row; do not conflate generations or claim Gen 1 definitively discontinued.
6. **C031 aune AR5000** — **AR5000 MK2** officially launched **2026-04-16**; prior model's production status remains UNKNOWN without a manufacturer discontinuation notice.
7. **C057 Sony INZONE H6 Air** — genuine 2026 open-back model on **Sony Korea** with official Korean support; no longer flagged as Korea-unknown.
8. **C042 Fostex T50RPmk4** — official Japanese store displays new stock, and manufacturer sells replacement pads and cables. **Korean importer/warranty remains UNKNOWN**.
9. **C044 Corsair VIRTUOSO PRO** — manufacturer spare-parts catalogue explicitly lists analog 3.5mm replacement cables. **Not equivalent to confirming local spare parts stock**.

## Warranty conflict requiring written confirmation

**HIFIMAN Korea website contains contradictory language variants:**
- Korean-language warranty policy: general headphones **1 year** (E0130).
- English-language warranty policy on the same regional site: general headphones **2 years** (E0131).

Neither period is assumed as the final contractual warranty in this research. Confirm in writing using **exact model + sales channel + purchase date** before purchase, especially open-box/refurbished products. The Korean store displays both new-product and open-box/refurbished categories; those must not be conflated.

## Current vs replacement parts vs domestic warranty

- **Manufacturer replacement parts documented:** selected beyerdynamic PRO / PRO X, Shure SRH440A/SRH840A, Meze 99/105, Audeze MM-100, Fostex T50RPmk4, Marshall Monitor III ANC, Corsair VIRTUOSO PRO, JBL Live 770NC.
- **Replaceable construction documented without confirmed current Korean accessory stock:** Sony MDR-M1, FiiO FT series, Austrian Audio Hi-X65, ASUS Kithara and others in the matrix.
- **Actual Korean authorised distributor:** confirmed for some brands such as Meze and Audeze, but a distributor listing alone does not prove every SKU is supported or available.
- **High-value unknowns for next steps:** manufacturer-refurbished HIFIMAN vs sealed-new supply, JBL LIVE770NC vs new LIVE780NC, SteelSeries Gen1 vs Gen2, older Philips inventory, aune AR3000 launch, Korea-specific per-model A/S and spare pads.

## Individual model matrix

`Official KR`: TRUE means visible official Korean model support/sales channel. UNKNOWN means not sufficiently verified. **It is not a binary assertion of unavailability.**

| ID | Brand / Model | Release year | Lifecycle | Successor | Official KR | Parts | Step 3 evidence |
|---|---|---|---|---|---|---|---|
| C001 | Sennheiser HD 560S | 2020 | 공식 현행 표기 | — | TRUE | UNKNOWN | 브랜드/기존자료 |
| C002 | Sennheiser HD 550 | 2025 | 공식 현행 표기 | — | TRUE | UNKNOWN | 브랜드/기존자료 |
| C003 | Sennheiser HD 600 | UNKNOWN | 공식 현행 표기 | — | TRUE | UNKNOWN | 브랜드/기존자료 |
| C004 | Sennheiser HD 490 PRO | 2024 | 공식 현행 표기 | — | TRUE | UNKNOWN | 브랜드/기존자료 |
| C005 | Sennheiser HD 480 PRO | 2026 | 공식 현행 표기 | — | TRUE | REPLACEABLE | E0089, E0090 |
| C006 | beyerdynamic DT 900 PRO X | UNKNOWN | 공식 현행 표기 | — | TRUE | OFFICIAL_PARTS | 브랜드/기존자료 |
| C007 | beyerdynamic DT 990 PRO X | UNKNOWN | 공식 현행 표기 | — | TRUE | OFFICIAL_PARTS | 브랜드/기존자료 |
| C008 | beyerdynamic DT 770 PRO X | 2024 | 공식 현행 표기 | — | TRUE | OFFICIAL_PARTS | 브랜드/기존자료 |
| C009 | beyerdynamic TYGR 300 R | UNKNOWN | 공식 현행 표기 | — | UNKNOWN | UNKNOWN | E0136 |
| C010 | Audio-Technica ATH-R50x | 2025 | 공식 현행 표기 | — | TRUE | UNKNOWN | E0092 |
| C011 | Audio-Technica ATH-R70xa | 2025 | 공식 현행 표기 | — | TRUE | UNKNOWN | 브랜드/기존자료 |
| C012 | Audio-Technica ATH-R30x | 2025 | 공식 현행 표기 | — | TRUE | UNKNOWN | 브랜드/기존자료 |
| C013 | Sony MDR-M1 | 2024 | 공식 현행 표기 | — | TRUE | REPLACEABLE | E0094 |
| C014 | Sony MDR-MV1 | 2023 | 공식 현행 표기 | — | TRUE | REPLACEABLE | E0095 |
| C015 | FiiO FT1 | 2024 | 공식 현행 표기 | — | UNKNOWN | REPLACEABLE | E0097 |
| C016 | FiiO FT1 PRO | 2025 | 공식 현행 표기 | — | UNKNOWN | REPLACEABLE | E0098 |
| C017 | FiiO FT3 | UNKNOWN | 공식 현행 표기 | — | UNKNOWN | REPLACEABLE | E0137 |
| C018 | FiiO FT5 | UNKNOWN | 공식 현행 표기 | — | UNKNOWN | REPLACEABLE | E0138 |
| C019 | HIFIMAN HE400se | UNKNOWN | 확인 불가 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C020 | HIFIMAN SUNDARA | UNKNOWN | 확인 불가 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C021 | HIFIMAN Edition XS | UNKNOWN | 확인 불가 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C022 | HIFIMAN ANANDA NANO | UNKNOWN | 공식 현행 표기 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C023 | HIFIMAN Edition XV | 2025 | 확인 불가 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C024 | AKG K371 | UNKNOWN | 공식 현행 표기 | — | UNKNOWN | REPLACEABLE | E0100 |
| C025 | Philips SHP9500 | 2014 | 확인 불가 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C026 | Philips Fidelio X2HR | UNKNOWN | 단종 확인 | — | UNKNOWN | UNKNOWN | E0103 |
| C027 | Shure SRH440A | 2022 | 공식 현행 표기 | — | TRUE | OFFICIAL_PARTS | E0105 |
| C028 | Shure SRH840A | 2022 | 공식 현행 표기 | — | TRUE | OFFICIAL_PARTS | E0106 |
| C029 | Meze 99 Classics 2nd Gen | 2025 | 공식 현행 표기 | — | UNKNOWN | OFFICIAL_PARTS | E0108 |
| C030 | Meze 105 AER | 2024 | 공식 현행 표기 | — | UNKNOWN | OFFICIAL_PARTS | 브랜드/기존자료 |
| C031 | aune AR5000 | 2023 | 확인 불가 | AR5000 MK2 | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C032 | aune AR5000 MK2 | 2026 | 공식 현행 표기 | — | UNKNOWN | UNKNOWN | E0109 |
| C033 | aune SR7000 | UNKNOWN | 공식 현행 표기 | — | UNKNOWN | UNKNOWN | E0139 |
| C034 | aune AR3000 | UNKNOWN | 확인 불가 | — | UNKNOWN | UNKNOWN | E0110 |
| C035 | MOONDROP PARA2 | UNKNOWN | 공식 현행 표기 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C036 | MOONDROP HORIZON | UNKNOWN | 공식 현행 표기 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C037 | Audeze MM-100 | 2024 | 공식 현행 표기 | — | UNKNOWN | OFFICIAL_PARTS | E0112 |
| C038 | Audeze Maxwell 2 | 2026 | 공식 현행 표기 | — | UNKNOWN | UNKNOWN | E0113 |
| C039 | Focal Azurys | 2024 | 공식 현행 표기 | — | UNKNOWN | UNKNOWN | E0114 |
| C040 | Focal Hadenys | 2024 | 공식 현행 표기 | — | UNKNOWN | UNKNOWN | E0115 |
| C041 | Austrian Audio Hi-X65 | 2022 | 공식 현행 표기 | — | UNKNOWN | REPLACEABLE | E0116 |
| C042 | Fostex T50RPmk4 | UNKNOWN | 공식 현행 표기 | — | UNKNOWN | OFFICIAL_PARTS | E0140, E0141 |
| C043 | Sennheiser / Drop HD 6XX | UNKNOWN | 확인 불가 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C044 | Corsair VIRTUOSO PRO | 2023 | 공식 현행 표기 | — | UNKNOWN | OFFICIAL_PARTS | E0117 |
| C045 | HyperX Cloud III | 2023 | 공식 현행 표기 | — | UNKNOWN | UNKNOWN | E0142 |
| C046 | Logitech G PRO X 2 LIGHTSPEED | 2023 | 공식 현행 표기 | — | TRUE | REPLACEABLE | E0118 |
| C047 | Razer BlackShark V3 Pro | 2025 | 공식 현행 표기 | — | UNKNOWN | REPLACEABLE | E0119 |
| C048 | JBL TUNE 770NC | 2023 | 공식 현행 표기 | — | TRUE | REPLACEABLE | E0120, E0121, E0134 |
| C049 | JBL LIVE 770NC | 2024 | 확인 불가 | LIVE 780NC | UNKNOWN | OFFICIAL_PARTS | E0122, E0123 |
| C050 | Bose QuietComfort Headphones (2nd Gen) | 2026 | 공식 현행 표기 | — | TRUE | UNKNOWN | E0124 |
| C051 | Marshall Monitor III ANC | 2024 | 공식 현행 표기 | — | TRUE | OFFICIAL_PARTS | E0125 |
| C052 | ASUS ROG Kithara | 2026 | 공식 현행 표기 | — | TRUE | REPLACEABLE | E0126, E0127 |
| C053 | SteelSeries Arctis Nova 7 Wireless | 2022 | 확인 불가 | Arctis Nova 7 Wireless Gen 2 | UNKNOWN | UNKNOWN | E0128, E0129, E0135 |
| C054 | Sennheiser HD 505 Copper Edition | 2025 | 공식 현행 표기 | — | TRUE | UNKNOWN | 브랜드/기존자료 |
| C055 | Audio-Technica ATH-M50x | UNKNOWN | 공식 현행 표기 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C056 | Anker soundcore Space One | UNKNOWN | 확인 불가 | Space One Pro | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C057 | Sony INZONE H6 Air | 2026 | 공식 현행 표기 | — | TRUE | UNKNOWN | E0096 |
| C058 | Nothing Headphone (1) | 2025 | 공식 현행 표기 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C059 | Philips SHP9600 | UNKNOWN | 단종 확인 | — | UNKNOWN | UNKNOWN | E0104 |
| C060 | AKG K361 | UNKNOWN | 공식 현행 표기 | — | UNKNOWN | REPLACEABLE | E0101 |
| C061 | Sennheiser HD 599 | UNKNOWN | 확인 불가 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |
| C062 | Audio-Technica ATH-AD500X | UNKNOWN | 확인 불가 | — | UNKNOWN | UNKNOWN | 브랜드/기존자료 |

## Gate check

- [x] All 62 candidates assessed with explicit CURRENT/DISCONTINUED/UNKNOWN.
- [x] Exact model and meaningful revision/variant issues reviewed and corrected where verified.
- [x] Successor recorded where identifiable; UNKNOWN retained otherwise.
- [x] Korean model channels and manufacturer parts documented to the degree verified, with gaps marked UNKNOWN.
- [x] Old-stock risk separated from actual manufacturing date; no seller inventory age invented.
- [x] No candidate rejected merely because of age or price.
- [ ] User review/approval of Step 3.

## Scope limitations and handoff for Step 4

**Not verified:** normal Korean selling prices, every seller's import type, individual serial manufacture date, each Korean distributor's warranty undertaking for every product, current stock of every replacement pad. These require targeted live verification in Step 4 or on a proposed finalist.

Do not use CURRENT/UNKNOWN as an acoustic-quality score.

Step 4 must separately price-check **official new**, **parallel import**, **international import**, and **open-box/refurbished** for the same model where relevant.

## Primary official source pointers

- Sennheiser HD 480 PRO: https://newsroom.sennheiser.com/sennheiser-launches-the-closed-back-hd-480-pro-headphones-cmho7q
- Philips X2HR discontinued: https://www.philips.co.kr/c-p/X2HR_00/fidelio-headphones/support
- Philips SHP9600 discontinued: https://www.philips.co.kr/c-p/SHP9600_00/over-ear-headphones/support
- Bose 2nd Gen: https://www.bose.com/pressroom/bose-updates-the-iconic-quietcomfort-headphones
- Sony INZONE H6 Air Korea: https://www.sony.co.kr/gaming-gear/products/inzone-h6-air
- JBL 2026 generation: https://kr.jbl.com/LIVE780NC.html
- SteelSeries 2025 generation: https://steelseries.com/press/158-steelseries-unleashes-the-power-of-the-arctis-nova-7-gen-2-series
- HIFIMAN Korean warranty: https://kr.hifiman.com/pages/warranty-policy
- HIFIMAN English warranty: https://kr.hifiman.com/en/pages/warranty-policy

Complete evidence references are in data/evidence.csv, E0089–E0142.
