# Step 4 — Korean Market Price Research

Date: 2026-10-09  
Status: REVIEW

## Purpose

Collect Korean seller/price-comparison observations for all 62 candidates without treating MSRP, limited card offers, imported stock, open-box/refurbished stock or sold-out pages as normal new-product market prices.

**NO subjective audio ranking, value ranking or product elimination is performed here.**

## Coverage summary

- **62** candidate IDs maintained (C001–C062).
- **133** raw price observations in `data/prices.csv` (P0001–P0133).
- **54** candidates have at least one portal/retailer price observation.
- **47** have a plausible listed new-goods low-price observation, requiring recheck at seller checkout.
- **7** have a conservative cross-portal typical advertised-price approximation.
- **20** have conditional card/member/coupon observations separated from ordinary prices.
- **15** do not have a sufficiently supported currently comparable new-product listed low price.
- Sources include Danawa, Enuri, Schezade and selected official Korean brand/retailer catalogs. Source timestamps and refresh recency vary widely.

**Warning:** Check date records the research date, not an assertion the indexed price is fresh that day or actually purchasable at checkout. Much of Danawa indexed content is 1–3 months old; Enuri samples were refreshed in September 2026. Actual seller inventory, shipping, import tax and coupon conditions can change. Even a seemingly official-category Danawa listing is not proof that a seller is an authorized Korean distributor.

## Definitions & calculation

- `prices.csv`: a raw **seller or price-comparison quote**, with source, shipping when known, official-category/import classification, terms and URL. "LISTED" does not guarantee **IN STOCK**.
- `price_summary.csv`: one candidate-level summary row per product.
- `Current_Low_Price_KRW`: lowest nominal **unconditional listed price** from a plausibly available new-product group. Genuine Korean quotes take priority; import-only price is separately labeled IMPORT_ONLY. This is **not a real-time confirmed checkout price**.
- `Deal_Price_KRW`: card, coupon, membership or point conditions kept separate. It may be above another seller's unconditional low; deals are seller-specific.
- `Normal_Price_KRW`: only when **at least two independent source portals** provide multiple reasonably clustered new-product asking prices. Rounded median of matching quotes. **It is an approximate current advertised market band, not a verified historically stable transaction price.** If not independently supported, UNKNOWN.
- `Price_Stability`: all UNKNOWN without an actual comparable history of time-stamped price observations.
- `OFFICIAL_ONLY` means quoted genuine/local listing group, **not conclusive seller authorization**. `IMPORT_ONLY` is overseas purchase; it cannot be compared to genuine local warranty and taxes without adjustment.
- Discount/list/MSRP strikethrough is **never** automatically the normal selling price.
- Out-of-stock and open-box/refurbished prices remain in raw observations but are excluded from sealed-new available low comparisons.
- Check shopping cart before purchase.

## Selected cross-brand market comparisons

These are **market-price context**, not recommendations:

| ID | Model | Estimated typical advertised | Listed low* | Conditional deal* | Scope | Confidence |
|---|---|---:|---:|---:|---|---|
| C001 | Sennheiser HD 560S | UNKNOWN | 216,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C002 | Sennheiser HD 550 | UNKNOWN | 268,900원 | 255,280원 | OFFICIAL_ONLY | LOW |
| C003 | Sennheiser HD 600 | UNKNOWN | 332,800원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C006 | beyerdynamic DT 900 PRO X | UNKNOWN | 425,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C010 | Audio-Technica ATH-R50x | 269,000원 | 249,000원 | 242,100원 | OFFICIAL_ONLY | MEDIUM |
| C011 | Audio-Technica ATH-R70xa | 439,000원 | 429,000원 | UNKNOWN | OFFICIAL_ONLY | MEDIUM |
| C012 | Audio-Technica ATH-R30x | 178,400원 | 173,880원 | UNKNOWN | OFFICIAL_ONLY | MEDIUM |
| C013 | Sony MDR-M1 | UNKNOWN | 305,970원 | 290,670원 | OFFICIAL_ONLY | LOW |
| C014 | Sony MDR-MV1 | UNKNOWN | 498,000원 | 474,050원 | OFFICIAL_ONLY | LOW |
| C015 | FiiO FT1 | 230,000원 | 230,000원 | 213,900원 | OFFICIAL_ONLY | MEDIUM |
| C016 | FiiO FT1 PRO | 315,000원 | 312,930원 | 285,300원 | OFFICIAL_ONLY | MEDIUM |
| C019 | HIFIMAN HE400se | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C020 | HIFIMAN SUNDARA | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C021 | HIFIMAN Edition XS | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C022 | HIFIMAN ANANDA NANO | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C024 | AKG K371 | UNKNOWN | 235,000원 | 234,000원 | OFFICIAL_ONLY | LOW |
| C031 | aune AR5000 | UNKNOWN | 420,000원 | UNKNOWN | IMPORT_ONLY | LOW |
| C032 | aune AR5000 MK2 | UNKNOWN | 538,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C037 | Audeze MM-100 | UNKNOWN | 638,680원 | 621,200원 | OFFICIAL_ONLY | LOW |
| C039 | Focal Azurys | UNKNOWN | 664,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C040 | Focal Hadenys | UNKNOWN | 766,500원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C044 | Corsair VIRTUOSO PRO | UNKNOWN | 240,490원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C045 | HyperX Cloud III | UNKNOWN | 99,000원 | 93,100원 | OFFICIAL_ONLY | LOW |
| C046 | Logitech G PRO X 2 LIGHTSPEED | UNKNOWN | 259,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C047 | Razer BlackShark V3 Pro | UNKNOWN | 399,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C048 | JBL TUNE 770NC | UNKNOWN | 107,100원 | 102,920원 | OFFICIAL_ONLY | LOW |
| C050 | Bose QuietComfort Headphones (2nd Gen) | UNKNOWN | 359,000원 | 341,050원 | OFFICIAL_ONLY | LOW |
| C051 | Marshall Monitor III ANC | UNKNOWN | 489,000원 | 440,100원 | OFFICIAL_ONLY | LOW |
| C052 | ASUS ROG Kithara | UNKNOWN | 480,700원 | 435,880원 | OFFICIAL_ONLY | LOW |
| C055 | Audio-Technica ATH-M50x | 229,000원 | 219,000원 | 206,100원 | OFFICIAL_ONLY | MEDIUM |
| C057 | Sony INZONE H6 Air | 263,800원 | 246,050원 | 250,170원 | OFFICIAL_ONLY | MEDIUM |
| C061 | Sennheiser HD 599 | UNKNOWN | 160,550원 | 152,520원 | OFFICIAL_ONLY | LOW |

*Not real-time checkout confirmed; separate import and stock notes in data files.*

## Independent source examples / research findings

1. **FiiO FT1 and FT1 PRO:** The FT1 has a repeatedly observed 230,000 KRW Korean new-product listing across Danawa, Enuri and a specialist shop. FT1 PRO has genuine-channel observations around 312,930–317,000 KRW; **import variants** around 215,000–221,000 KRW are separate, and the 285,300 KRW card rate is conditional. Do **not** use the overseas rate as normal domestic genuine price.
2. **Audio-Technica ATH-R50x:** Danawa 249,000/269,000 KRW and specialist store 269,000 KRW; Korean manufacturer's seasonal holiday 249,000 KRW is recorded as a promotion, not lasting normal price. Cross-portal asking-price center is ~269,000 KRW.
3. **Audio-Technica ATH-M50x:** domestic genuine listed roughly 219,000–229,000 KRW, but overseas-purchase entries near 100,000 KRW. Warranty, model identity and accessories must be checked before comparing.
4. **HIFIMAN:** HE400se, SUNDARA, Edition XS and ANANDA NANO Korean official pages show prices but **SOLD OUT**. Edition XS refurbished/open-box variants also show prices, but cannot stand in for a sealed-new, currently buyable retail offer. Edition XV was evidenced only as an open-box listing. The corresponding current-new low fields remain UNKNOWN.
5. **Sennheiser HD 480 PRO:** only older indexed overseas-purchase price observations were found; approximately 613,580–624,520 KRW (and a card-conditional 570,630 KRW) may not represent a currently valid checkout option. Import-only, LOW confidence; normal price UNKNOWN.
6. **Sennheiser/Drop HD6XX:** Danawa import listing 429,900 KRW in recent cached index; a much older Enuri page gave another value. The stale Enuri number was **not** used for current normal price.
7. **beyerdynamic DT 990/770 PRO X:** current Korean site sells special **Limited Black (LB)** variants at 335,000 KRW. The standard C007/C008 versions were not silently assigned the variant-only price; current low UNKNOWN pending exact SKU confirmation.
8. **Focal Hadenys/Azurys:** Korean AudioGallery visibly discounts Hadenys to 766,500 KRW and Azurys to 664,000 KRW; original strikethrough list values are not treated as typical actual selling prices.
9. **Sony INZONE H6 Air:** Korean genuine listing 246,050 KRW Danawa vs 269,000 KRW Sony Korea official catalog; Enuri ~268,640 KRW as a third comparison. Membership/card variations tracked separately.
10. **Corsair VIRTUOSO PRO:** more recent Danawa indexed observations around 240,490 KRW differ from Step 2 ~170,000 KRW discovery figure. Step 4 quote supersedes the older snapshot for subsequent market-value calculations; 170k is NOT asserted still available.
11. **Bose QuietComfort Headphones 2nd Gen:** official Korean store 359,000 KRW ordinary listed quote, 341,050 KRW with store-member coupon. Bose is a consumer ANC product and cannot be judged by price alone against passive analog hi-fi headphones.

## Missing, restricted, or insufficient observations

**No comparable currently advertised new-product low for these 15 products:**

C007 beyerdynamic DT 990 PRO X; C008 beyerdynamic DT 770 PRO X; C009 beyerdynamic TYGR 300 R; C019 HIFIMAN HE400se; C020 HIFIMAN SUNDARA; C021 HIFIMAN Edition XS; C022 HIFIMAN ANANDA NANO; C023 HIFIMAN Edition XV; C029 Meze 99 Classics 2nd Gen; C034 aune AR3000; C035 MOONDROP PARA2; C036 MOONDROP HORIZON; C038 Audeze Maxwell 2; C042 Fostex T50RPmk4; C053 SteelSeries Arctis Nova 7 Wireless.

Reasons: no reliable comparable Korean page, outdated/incomplete search results, official **SOLD OUT**, unclear stock, only open-box/refurb, or a price for a different limited model. These remain in the candidate population and are **not rejected**.

**Direct Naver Shopping/Blog:** Original page access not consistently available in this research pathway. Do not label third-party mirrored quotes as verified Naver originals.

**Enuri:** Successfully found and used independent price comparisons for **some** FiiO models, Sony INZONE H6 Air, and Sennheiser HD 480 PRO, with historical price-refresh dates (e.g. September 2026). Contrary to Step 2's initial weaker discovery coverage, Enuri is **partially usable** for independent cross-checks. Direct retail checkout still not verified.

**Price-history:** No sufficiently reliable longitudinal time series available for the 62-product pool to quantify price stability, so all Price_Stability = UNKNOWN.

## Full candidate price summary

| ID | Candidate | Typical advertised | Listed low* | Conditional deal* | Scope | Confidence |
|---|---|---:|---:|---:|---|---|
| C001 | Sennheiser HD 560S | UNKNOWN | 216,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C002 | Sennheiser HD 550 | UNKNOWN | 268,900원 | 255,280원 | OFFICIAL_ONLY | LOW |
| C003 | Sennheiser HD 600 | UNKNOWN | 332,800원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C004 | Sennheiser HD 490 PRO | UNKNOWN | 675,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C005 | Sennheiser HD 480 PRO | UNKNOWN | 613,580원 | 570,630원 | IMPORT_ONLY | LOW |
| C006 | beyerdynamic DT 900 PRO X | UNKNOWN | 425,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C007 | beyerdynamic DT 990 PRO X | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C008 | beyerdynamic DT 770 PRO X | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C009 | beyerdynamic TYGR 300 R | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C010 | Audio-Technica ATH-R50x | 269,000원 | 249,000원 | 242,100원 | OFFICIAL_ONLY | MEDIUM |
| C011 | Audio-Technica ATH-R70xa | 439,000원 | 429,000원 | UNKNOWN | OFFICIAL_ONLY | MEDIUM |
| C012 | Audio-Technica ATH-R30x | 178,400원 | 173,880원 | UNKNOWN | OFFICIAL_ONLY | MEDIUM |
| C013 | Sony MDR-M1 | UNKNOWN | 305,970원 | 290,670원 | OFFICIAL_ONLY | LOW |
| C014 | Sony MDR-MV1 | UNKNOWN | 498,000원 | 474,050원 | OFFICIAL_ONLY | LOW |
| C015 | FiiO FT1 | 230,000원 | 230,000원 | 213,900원 | OFFICIAL_ONLY | MEDIUM |
| C016 | FiiO FT1 PRO | 315,000원 | 312,930원 | 285,300원 | OFFICIAL_ONLY | MEDIUM |
| C017 | FiiO FT3 | UNKNOWN | 361,090원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C018 | FiiO FT5 | UNKNOWN | 567,790원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C019 | HIFIMAN HE400se | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C020 | HIFIMAN SUNDARA | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C021 | HIFIMAN Edition XS | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C022 | HIFIMAN ANANDA NANO | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C023 | HIFIMAN Edition XV | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C024 | AKG K371 | UNKNOWN | 235,000원 | 234,000원 | OFFICIAL_ONLY | LOW |
| C025 | Philips SHP9500 | UNKNOWN | 69,800원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C026 | Philips Fidelio X2HR | UNKNOWN | 129,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C027 | Shure SRH440A | UNKNOWN | 157,440원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C028 | Shure SRH840A | UNKNOWN | 178,000원 | UNKNOWN | IMPORT_ONLY | LOW |
| C029 | Meze 99 Classics 2nd Gen | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C030 | Meze 105 AER | UNKNOWN | 576,030원 | 518,440원 | OFFICIAL_ONLY | LOW |
| C031 | aune AR5000 | UNKNOWN | 420,000원 | UNKNOWN | IMPORT_ONLY | LOW |
| C032 | aune AR5000 MK2 | UNKNOWN | 538,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C033 | aune SR7000 | UNKNOWN | 863,330원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C034 | aune AR3000 | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C035 | MOONDROP PARA2 | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C036 | MOONDROP HORIZON | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C037 | Audeze MM-100 | UNKNOWN | 638,680원 | 621,200원 | OFFICIAL_ONLY | LOW |
| C038 | Audeze Maxwell 2 | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C039 | Focal Azurys | UNKNOWN | 664,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C040 | Focal Hadenys | UNKNOWN | 766,500원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C041 | Austrian Audio Hi-X65 | UNKNOWN | 699,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C042 | Fostex T50RPmk4 | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C043 | Sennheiser / Drop HD 6XX | UNKNOWN | 429,900원 | UNKNOWN | IMPORT_ONLY | LOW |
| C044 | Corsair VIRTUOSO PRO | UNKNOWN | 240,490원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C045 | HyperX Cloud III | UNKNOWN | 99,000원 | 93,100원 | OFFICIAL_ONLY | LOW |
| C046 | Logitech G PRO X 2 LIGHTSPEED | UNKNOWN | 259,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C047 | Razer BlackShark V3 Pro | UNKNOWN | 399,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C048 | JBL TUNE 770NC | UNKNOWN | 107,100원 | 102,920원 | OFFICIAL_ONLY | LOW |
| C049 | JBL LIVE 770NC | UNKNOWN | 109,920원 | UNKNOWN | IMPORT_ONLY | LOW |
| C050 | Bose QuietComfort Headphones (2nd Gen) | UNKNOWN | 359,000원 | 341,050원 | OFFICIAL_ONLY | LOW |
| C051 | Marshall Monitor III ANC | UNKNOWN | 489,000원 | 440,100원 | OFFICIAL_ONLY | LOW |
| C052 | ASUS ROG Kithara | UNKNOWN | 480,700원 | 435,880원 | OFFICIAL_ONLY | LOW |
| C053 | SteelSeries Arctis Nova 7 Wireless | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| C054 | Sennheiser HD 505 Copper Edition | UNKNOWN | 236,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C055 | Audio-Technica ATH-M50x | 229,000원 | 219,000원 | 206,100원 | OFFICIAL_ONLY | MEDIUM |
| C056 | Anker soundcore Space One | UNKNOWN | 89,900원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C057 | Sony INZONE H6 Air | 263,800원 | 246,050원 | 250,170원 | OFFICIAL_ONLY | MEDIUM |
| C058 | Nothing Headphone (1) | UNKNOWN | 389,000원 | UNKNOWN | OFFICIAL_ONLY | LOW |
| C059 | Philips SHP9600 | UNKNOWN | 101,370원 | 96,310원 | IMPORT_ONLY | LOW |
| C060 | AKG K361 | UNKNOWN | 190,000원 | 171,000원 | OFFICIAL_ONLY | LOW |
| C061 | Sennheiser HD 599 | UNKNOWN | 160,550원 | 152,520원 | OFFICIAL_ONLY | LOW |
| C062 | Audio-Technica ATH-AD500X | UNKNOWN | 92,420원 | UNKNOWN | IMPORT_ONLY | LOW |

## Completion gate

- [x] Raw source/seller observations and URLs saved.
- [x] Actual advertised quotes, conditional offers, and list/MSRP clearly separated.
- [x] Distribution groups (genuine/local listings versus import) recorded independently.
- [x] Sold-out / limited-edition / open-box / refurbished distinctions preserved.
- [x] Observation date, source URL, shipment when confirmed, and price conditions documented; unknown shipping not filled with 0.
- [x] Normal advertised price derived only for supported multi-portal cases, otherwise UNKNOWN, with explicit confidence.
- [x] Naver source access limitations and Enuri's partial verification recorded.
- [ ] User reviews Step 4, including the price uncertainty and unknown cases.

## Next-step boundary

Step 5 may filter **objective technical, physical or purchase availability problems**, but **must not reject any product solely due to high asking price** before performance comparison.

Step 9 must recheck changed prices for the actual shortlisted products. This Step 4 data is a dated comparison baseline, not a permanent price guarantee.
