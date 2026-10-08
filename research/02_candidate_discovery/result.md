# Step 2 — Candidate Discovery Result

Date: 2026-10-08
Status: REVIEW

**CURRENT TOTAL: 58 candidates (original 43 retained; 15 added on 2026-10-08).**

**Supplemental bias-correction report:** [supplemental_review.md](supplemental_review.md). The original 43-candidate findings below are the first-pass snapshot, not the current total.

## Scope

This stage discovers candidates; it does not rank or recommend them.

Three independent paths were used:
- 2A Brand-based
- 2B Community / Expert-based
- 2C Korea-market reverse discovery

Naver Shopping / Blog original pages are directly access-limited in the current web path. They are not treated as directly verified originals.

## 2A — Brand-based Discovery

Sennheiser:
HD 560S, HD 550, HD 600, HD 490 PRO, HD 480 PRO

beyerdynamic:
DT 900 PRO X, DT 990 PRO X, DT 770 PRO X, TYGR 300 R

Audio-Technica:
ATH-R30x, ATH-R50x, ATH-R70xa

Sony:
MDR-M1, MDR-MV1

FiiO:
FT1, FT1 PRO, FT3, FT5

HIFIMAN:
HE400se, SUNDARA, Edition XS, ANANDA NANO, Edition XV

AKG:
K371

Philips:
Fidelio X2HR

Shure:
SRH440A, SRH840A

Meze:
99 Classics 2nd Gen, 105 AER

aune:
AR5000, AR5000 MK2, SR7000, AR3000

MOONDROP:
PARA2, HORIZON

Audeze:
MM-100, Maxwell 2

Focal:
Azurys, Hadenys

Austrian Audio:
Hi-X65

## 2B — Community / Expert Discovery

Repeated recent groups:
- FiiO FT1 / FT1 PRO
- HIFIMAN Edition XS / SUNDARA / ANANDA NANO
- aune AR5000
- Sennheiser HD 560S / HD 600 / HD 6XX
- Audio-Technica ATH-R50x
- Sony MDR-MV1
- Meze 105 AER
- Audeze MM-100
- Audeze Maxwell family
- beyerdynamic TYGR 300 R

Recent $200–300 music + general gaming + movie discussions repeatedly compare FT1 PRO, Edition XS, AR5000 and HD 560S.

New brands/models discovered outside the Step 1 fixed map:
- Fostex T50RPmk4
- Sennheiser / Drop HD 6XX

## 2C — Korea-market Reverse Discovery

These are discovery snapshots only. Step 4 will perform full price research.

| Approx. band | Example | Market snapshot |
|---|---|---|
| 5–10만원 | Philips SHP9500 | Danawa about 69,800 KRW |
| 10–15만원 | Shure SRH440A | about 149,000 KRW |
| 15–20만원 | HD 560S deal/history range | Danawa results have shown roughly 168k–210k depending snapshot |
| 20–25만원 | Audio-Technica ATH-R50x | about 249,000 KRW |
| 25–30만원 | AKG K371 / FT1 PRO conditional | K371 about 260k; FT1 PRO card price about 285k |
| 30–35만원 | FiiO FT1 PRO normal | about 314k |

Upper references also visibly sold in Korea:
- Sony MDR-M1 around 370k
- Sony MDR-MV1 around 500k
- Meze 105 AER around 576k
- Audeze MM-100 around 640k
- Austrian Audio Hi-X65 around 699k

They remain in discovery because Step 2 does not eliminate by price.

## Merged Candidate Pool

The original pass registered 43 candidates. The supplemental review added 15 more; 58 are currently registered in data/candidates.csv.

Each row preserves:
- Discovery_Brand
- Discovery_Community
- Discovery_KoreaMarket

This is not a recommendation list.

## Access Limitations

Naver Shopping / Blog:
- original-page access is limited in the current web path
- snippets or Naver Pay entries surfaced through other sites are not counted as direct Naver verification
- later price work will use DIRECT / LIMITED evidence status explicitly

Enuri:
- indexed results were less consistent than Danawa during this discovery pass
- it will be retried in Step 4 for price cross-checking

## Step 2 Gate

- [x] 2A completed
- [x] 2B completed
- [x] 2C completed
- [x] recent recommendations separated from long-running references
- [x] duplicates merged
- [x] every candidate retains discovery-route flags
- [x] no early final ranking created

Step 2 remains REVIEW after supplemental correction. The supplemental source evidence is in E0054–E0079.

Next after approval: Step 3 — Product Status & Lifecycle.
