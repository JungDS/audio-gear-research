# Data Schema

## Common Conventions

- 날짜: `YYYY-MM-DD`
- 알 수 없음: `UNKNOWN`
- 해당 없음: `N/A`
- Boolean: `TRUE/FALSE`
- Confidence: `HIGH/MEDIUM/LOW/UNKNOWN`
- 후보 상태: `DISCOVERED/PASS/HOLD/REJECT/FINALIST`
- 유통: `OFFICIAL/PARALLEL/IMPORT/MIXED/UNKNOWN`
- Candidate ID: `C001`, `C002` ...
- Price ID: `P0001`, `P0002` ...
- Evidence ID: `E0001`, `E0002` ...
- CSV 필드에 쉼표/줄바꿈이 들어가면 표준 CSV quoting을 사용한다.

## candidates.csv

- Candidate_ID
- Brand
- Model
- Release_Year
- Revision
- Lifecycle_Status: CURRENT/DISCONTINUED/UNKNOWN
- Successor_Model
- Form: OPEN/CLOSED/SEMI_OPEN/UNKNOWN
- Driver_Type
- Weight_g
- Impedance_Ohm
- Sensitivity
- Official_KR_Distribution
- Parts_Availability
- Inventory_Age_Risk: HIGH/MEDIUM/LOW/UNKNOWN
- Discovery_Brand
- Discovery_Community
- Discovery_KoreaMarket
- Candidate_Status
- Rejection_Reason
- Reconsideration_Condition
- Last_Checked
- Notes

## prices.csv

판매처에서 관측한 **원자료**를 행 단위로 기록한다.

- Price_ID
- Candidate_ID
- Checked_Date
- Source
- Seller
- Distribution_Type
- Price_Type: LISTED/DEAL
- Price_KRW
- Shipping_KRW
- Conditions
- Historical_Context
- Source_URL
- Notes

## price_summary.csv

Step 4에서 원가격 스냅샷을 종합해 후보별 시장가격을 요약한다.

- Candidate_ID
- As_Of_Date
- Normal_Price_KRW
- Current_Low_Price_KRW
- Deal_Price_KRW
- Normal_Price_Basis
- Comparison_Scope: OFFICIAL_ONLY/MIXED/IMPORT_ONLY/UNKNOWN
- Price_Stability: HIGH/MEDIUM/LOW/UNKNOWN
- Sources_Count
- Confidence
- Notes

## evidence.csv

- Evidence_ID
- Candidate_ID
- Stage
- Evidence_Type: OFFICIAL/MEASUREMENT/PRO_REVIEW/COMMUNITY/KR_REVIEW/PRICE
- Source_Name
- Title
- Published_Date
- Checked_Date
- Access_Status: DIRECT/LIMITED/SECONDARY_ONLY
- URL
- Claim
- Direction: POSITIVE/NEGATIVE/NEUTRAL/MIXED
- Confidence
- Notes

## evaluations.csv

절대평가 필드:
- Candidate_ID
- Tonality
- Resolution
- Separation
- Imaging
- Soundstage
- Dynamics
- Bass_Quantity
- Bass_Quality
- Vocal
- Treble_Fatigue
- Music
- General_Gaming
- Animation
- Movies
- Comfort
- QC_Durability
- Parts_Support
- AE5_Compatibility
- Audio_Confidence
- Use_Case_Confidence
- Comfort_Confidence
- QC_Confidence

H7 + AE-5 대비 개선량:
- H7_Resolution_Delta
- H7_Separation_Delta
- H7_Imaging_Delta
- H7_Soundstage_Delta
- H7_Dynamics_Delta
- H7_Bass_Quantity_Change
- H7_Bass_Quality_Delta
- H7_Vocal_Delta
- H7_Treble_Quality_Delta
- H7_Music_Delta
- H7_General_Gaming_Delta
- H7_Animation_Delta
- H7_Movies_Delta
- H7_Comfort_Delta
- H7_Comparison_Confidence
- Overall_Upgrade_Confidence
- Notes

성능 Delta는 `UP3/UP2/UP1/SAME/DOWN1/DOWN2/DOWN3/UNKNOWN` 중 하나를 사용한다.

`H7_Bass_Quantity_Change`는 양의 증감이지 성능 우열이 아니므로 `MORE/SAME/LESS/UNKNOWN`을 사용한다.
