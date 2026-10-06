Status: NOT_STARTED
Stage: 9
Depends on: Step 4, Step 8

# Step 9 — Value Curve

## Objective

국내 실판매가와 H7 대비 체감 개선폭을 결합해 최소비용, 가성비 최적점, 지출 상한선을 찾는다.

## Inputs

- Step 4 가격 데이터
- Step 8 변화 벡터
- data/prices.csv
- data/evaluations.csv

## Exact Tasks

1. 각 후보의 통상가와 현재가를 별도로 놓고 교체가치를 비교한다.
2. 가격 증가에 따른 체감 개선의 한계효용을 분석한다.
3. 최소 비용으로 확실한 개선이 시작되는 지점을 찾는다.
4. 가격 대비 개선폭이 가장 큰 구간을 찾는다.
5. 추가 지출 대비 개선폭이 급격히 감소하는 상한선을 찾는다.
6. 일시 특가일 때만 가치가 생기는 제품을 별도 표시한다.

## Minimum Coverage

- 통상가 기준 분석과 현재 특가 기준 분석을 구분
- 동가격대 직접 경쟁 제품을 반드시 비교
- 가격차가 작을 때 신형/AS/착용감 차이를 함께 고려

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/09_value_analysis/result.md
- 가치곡선 및 역할별 후보군

## Completion Gate

- [ ] 최소비용 업그레이드 지점이 확인되었다.
- [ ] 가성비 최적점이 확인되었다.
- [ ] 지출 상한선 또는 상한선 없음이 근거와 함께 설명되었다.
- [ ] 특가 의존 후보가 구분되었다.

## Prohibited Shortcuts

- 가장 좋은 제품을 자동으로 가성비 1위로 만들지 않는다.
- 가격대별로 억지로 하나씩 추천하지 않는다.
- MSRP 할인율을 가치 계산에 넣지 않는다.

## Handoff

- Step 10에 역할별 유력 후보를 전달한다.
- 가격 변동 시 재평가가 필요한 후보를 표시한다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
