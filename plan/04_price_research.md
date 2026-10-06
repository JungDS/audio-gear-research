Status: NOT_STARTED
Stage: 4
Depends on: Step 3

# Step 4 — Korean Market Price Research

## Objective

후보별 한국 시장의 실제 통상가, 현재 최저가, 조건부 특가와 가격 안정성을 확인한다.

## Inputs

- Step 3 후보 및 유통 상태
- data/prices.csv
- 국내 가격비교/쇼핑몰 자료

## Exact Tasks

1. 네이버쇼핑 가격과 판매처 구성을 확인한다.
2. 다나와 최저가와 가능한 경우 가격 추이를 확인한다.
3. 에누리로 교차확인한다.
4. 쿠팡, 11번가, G마켓/옥션, 공식스토어, 전문몰을 필요한 경우 확인한다.
5. 카카오 톡딜이나 카드/쿠폰가는 조건부 특가로 분리한다.
6. 정식유통/병행수입/해외직구 가격을 분리한다.
7. 통상 실판매가를 여러 판매처의 반복 가격대로 판단한다.
8. 확인 날짜와 조건을 기록한다.

## Minimum Coverage

- 가능한 후보는 가격비교 사이트 2개 이상 교차확인
- 현재 최저가가 유난히 낮으면 판매조건/유통형태 추가 검증
- 통상가와 일회성 특가를 분리
- 가격 추이를 제공하는 사이트가 있으면 변동성 확인

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/04_price_research/result.md
- data/prices.csv
- data/evidence.csv

## Completion Gate

- [ ] MSRP와 실판매가가 분리되었다.
- [ ] 통상가/현재 최저가/조건부 특가가 구분되었다.
- [ ] 정식유통/병행/직구가 구분되었다.
- [ ] 가격 확인일과 주요 조건이 기록되었다.

## Prohibited Shortcuts

- 공식 할인율을 가성비 점수로 사용하지 않는다.
- 한 판매처만 보고 시장가를 확정하지 않는다.
- 쿠폰/카드/회원 전용 가격을 일반 통상가로 기록하지 않는다.
- 이 단계에서 음질 순위를 변경하지 않는다.

## Handoff

- Step 5와 Step 9가 사용할 가격 기준을 전달한다.
- 가격 변동이 큰 후보는 재확인 필요 표시를 남긴다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
