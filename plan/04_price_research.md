Status: COMPLETED
Stage: 4
Depends on: Step 3

# Step 4 — Korean Market Price Research

## Objective

후보별 한국 시장의 판매처 가격 원자료를 수집하고, 이를 바탕으로 실제 통상가, 현재 최저가, 조건부 특가와 가격 안정성을 요약한다.

## Inputs

- Step 3 후보 및 유통 상태
- data/prices.csv
- data/price_summary.csv
- 국내 가격비교/쇼핑몰 자료

## Exact Tasks

1. 네이버쇼핑 가격과 판매처 구성을 확인한다.
2. 다나와 최저가와 가능한 경우 가격 추이를 확인한다.
3. 에누리로 교차확인한다.
4. 쿠팡, 11번가, G마켓/옥션, 공식스토어, 전문몰을 필요한 경우 확인한다.
5. 카카오 톡딜이나 카드/쿠폰가는 조건부 특가로 분리한다.
6. 정식유통/병행수입/해외직구 가격을 분리한다.
7. 관측한 판매처별 가격은 `data/prices.csv`에 원자료로 기록한다.
8. 여러 판매처의 반복 가격과 가격 추이를 바탕으로 통상 실판매가를 판단한다.
9. 통상가/현재 최저가/특가는 `data/price_summary.csv`에 후보별로 요약한다.
10. 확인 날짜, 배송비, 쿠폰/회원/카드 조건과 접근 제한을 기록한다.

## Minimum Coverage

- 가능한 후보는 가격비교 사이트 2개 이상 교차확인
- 현재 최저가가 유난히 낮으면 판매조건/유통형태 추가 검증
- 통상가와 일회성 특가를 분리
- 가격 추이를 제공하는 사이트가 있으면 변동성 확인
- 직접 접근하지 못한 가격은 Access limited로 근거 상태 기록

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/04_price_research/result.md
- data/prices.csv
- data/price_summary.csv
- data/evidence.csv

## Completion Gate

- [x] 판매처별 가격 원자료 133건이 기록되었다.
- [x] MSRP/표시 정가와 가격비교 판매가가 분리되었다.
- [x] 비교 가능한 표시 최저가 47개, 복수 경로 가격대 중심값 7개, 조건부 특가 20개를 구분했다. 통상가 근거 부족은 UNKNOWN.
- [x] 국내 정품 표기/해외구매를 구분했다. 실제 판매자 정식유통 권한 미확인은 명시했다.
- [x] 가격 확인일, 자료 갱신시차, 카드/회원 조건, 배송비 미확인과 품절을 기록했다.
- [x] 서로 다른 비교 출처로 검증한 7개만 통상 표시가격 근삿값을 산정하고, 나머지는 UNKNOWN과 Confidence를 기록했다.

## Prohibited Shortcuts

- 공식 할인율을 가성비 점수로 사용하지 않는다.
- 한 판매처만 보고 시장가를 확정하지 않는다.
- 쿠폰/카드/회원 전용 가격을 일반 통상가로 기록하지 않는다.
- 검색결과에 노출된 가격만으로 직접 확인한 판매가처럼 기록하지 않는다.
- 이 단계에서 음질 순위를 변경하지 않는다.

## Handoff

- Step 5와 Step 9가 사용할 price summary를 전달한다.
- 가격 변동이 큰 후보는 재확인 필요 표시를 남긴다.

Step 4 결과: `research/04_price_research/result.md`. 원자료 `data/prices.csv` 133건, 후보별 `data/price_summary.csv` 62행, Step 4 근거 E0143~E0199.

2026-10-09 사용자 승인에 따라 **COMPLETED**. `research/04_price_research/handoff.md`를 기록하고 Step 5를 시작한다. 가격은 직접 결제 확인이 아닌 온라인 표시/인덱스 스냅샷이므로 실제 구매 전 재확인해야 한다.
