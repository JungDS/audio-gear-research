# Data Schema

## Common Conventions

- 날짜: `YYYY-MM-DD`
- 알 수 없음: `UNKNOWN`
- 해당 없음: `N/A`
- Boolean: `TRUE/FALSE`
- Confidence: `HIGH/MEDIUM/LOW/UNKNOWN`
- 후보 상태: `DISCOVERED/PASS/HOLD/REJECT/FINALIST`
- 유통: `OFFICIAL/PARALLEL/IMPORT/MIXED/UNKNOWN`

## candidates.csv

- Candidate_ID: 고유 식별자
- Brand
- Model
- Release_Year
- Lifecycle_Status: CURRENT/DISCONTINUED/UNKNOWN
- Successor_Model
- Form: OPEN/CLOSED/SEMI_OPEN/UNKNOWN
- Driver_Type
- Weight_g
- Impedance_Ohm
- Sensitivity
- Official_KR_Distribution
- Parts_Availability
- Discovery_Brand
- Discovery_Community
- Discovery_KoreaMarket
- Candidate_Status
- Rejection_Reason
- Reconsideration_Condition
- Last_Checked
- Notes

## prices.csv

- Price_ID
- Candidate_ID
- Checked_Date
- Source
- Seller
- Distribution_Type
- Price_Type: NORMAL/CURRENT_LOW/DEAL
- Price_KRW
- Shipping_KRW
- Conditions
- Historical_Context
- Source_URL
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
- URL
- Claim
- Direction: POSITIVE/NEGATIVE/NEUTRAL/MIXED
- Confidence
- Notes

## evaluations.csv

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
- H7_Resolution_Delta
- H7_Separation_Delta
- H7_Soundstage_Delta
- H7_Bass_Quantity_Delta
- H7_Bass_Quality_Delta
- H7_Vocal_Delta
- H7_Comfort_Delta
- Overall_Upgrade_Confidence
- Notes

H7 Delta는 `UP3/UP2/UP1/SAME/DOWN1/DOWN2/DOWN3/UNKNOWN` 중 하나를 사용한다.
