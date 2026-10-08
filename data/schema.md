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
  - CURRENT = 제조사 공식 채널에서 현재 제품으로 판매/홍보/지원되는 상태. 실제 생산 지속이나 새 재고의 제조일은 보장하지 않음.
  - DISCONTINUED = 제조사 또는 한국 공식 지원 페이지가 명시적으로 단종 표시.
  - UNKNOWN = 현재 신품 생산/판매 또는 단종을 확정할 신뢰할 근거 부족.
- Official_KR_Distribution: TRUE/UNKNOWN (공식 국내 제품 페이지/모델 취급이 확인되는 경우만 TRUE, 브랜드 유통사만 존재한다면 UNKNOWN)
- Parts_Availability: OFFICIAL_PARTS/REPLACEABLE/UNKNOWN (한국 내 즉시 재고 보장은 아님)
- Inventory_Age_Risk: HIGH/MEDIUM/LOW/UNKNOWN (추정 위험도는 근거와 함께, 실제 제조일 미확인 시 오인 금지)
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
  - LISTED는 사이트가 표시한 판매 제시가격이며 **재고 보유나 실시간 결제 가능 보장 아님**.
  - DEAL은 카드/회원/쿠폰/포인트 등 조건부 할인액이며 일반 최저가와 별도.
  - 표시가격이 품절/오픈박스/리퍼/한정판뿐이라면 해당 조건을 Conditions/Notes에 명시하고 새 제품 비교요약에서 제외.
  - Checked_Date는 연구 조사일(페이지 조회일)이며 원자료 갱신일·장바구니 가격 확인과 다를 수 있음.
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
- Normal_Price_Basis: 서로 다른 출처에서 반복 확인된 비조건부 표시가격의 중심 추정에만 값을 채움; 실제 과거 거래가격이나 장기 통상가 확정 아님
- Comparison_Scope: OFFICIAL_ONLY/MIXED/IMPORT_ONLY/UNKNOWN
- Price_Stability: HIGH/MEDIUM/LOW/UNKNOWN (장기 가격 시계열 없으면 UNKNOWN)
- Sources_Count: 후보별 조사에서 사용한 별개의 출처 포털/도메인 수(판매자 수와 다름)
- Confidence
- Notes

## evidence.csv

후보가 아직 존재하지 않는 Step 0/1의 근거도 기록할 수 있도록 `Subject_Type`과 `Subject_ID`를 사용한다.

- Evidence_ID
- Subject_Type: BASELINE/BRAND/CANDIDATE/MARKET/METHOD
- Subject_ID
  - BASELINE 예: `H7_AE5`
  - BRAND 예: `Sennheiser`
  - CANDIDATE 예: `C001`
  - MARKET 예: `KR_HEADPHONE_MARKET`
- Stage
- Evidence_Type: USER_CONTEXT/OFFICIAL/MEASUREMENT/PRO_REVIEW/COMMUNITY/KR_REVIEW/PRICE
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

`USER_CONTEXT`는 현재 장비 연결 방식이나 사용자가 직접 보고한 청취 체감처럼 공개 웹 출처가 아닌 프로젝트 입력에 사용한다. 공개 저장소에는 민감정보를 넣지 않는다.

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
