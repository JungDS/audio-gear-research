Status: COMPLETED
Stage: 9
Depends on: Step 4, Step 8

# Step 9 — Value Curve

## Objective

국내 실판매가와 H7 대비 체감 개선폭을 결합해 최소비용, 가성비 최적점, 지출 상한선을 찾는다.

## Inputs

- Step 4 가격 데이터
- Step 8 변화 벡터
- data/price_summary.csv
- data/evaluations.csv

## Exact Tasks

1. 각 후보의 통상가와 현재가를 별도로 놓고 교체가치를 비교한다.
2. 변화 벡터와 가격차를 이용해 명백히 열위인 후보와 Pareto 우위 후보를 식별한다.
3. 최소 비용으로 확실한 개선이 시작되는 지점을 찾는다.
4. 가격 상승 대비 실질 개선이 가장 큰 구간을 찾는다.
5. 추가 지출 대비 개선폭이 급격히 감소하는 상한선을 찾는다.
6. 일시 특가일 때만 가치가 생기는 제품을 별도 표시한다.
7. 정밀한 수치 근거가 없는 경우 임의의 100점 환산이나 소수점 가성비 점수를 만들지 않는다.

## Minimum Coverage

- 통상가 기준 분석과 현재 특가 기준 분석을 구분
- 동가격대 직접 경쟁 제품을 반드시 비교
- 가격차가 작을 때 신형/AS/착용감 차이를 함께 고려
- 가격과 성능 모두에서 지배되는 후보가 있는지 확인
- 주관적 차이를 과도하게 수치화하지 않음

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/09_value_analysis/result.md
- 최소비용/가성비 최적점/지출 상한선 후보군
- 후보별 통상가 조건과 특가 조건

## Completion Gate

- [x] 반복 행사 189,000원 HD560S를 현재 근거상 가장 낮은 신뢰 가능한 업그레이드 후보 가격으로 확인(직접 A/B 아님).
- [x] 음악/일반 게임/영화의 서로 다른 장점별로 약 19~32만원 가격대가 비교 유력 구간임을 확인(단일 만능 1위 없음).
- [x] 객관적 절대 지출 상한은 근거 부족으로 설정하지 않았고, 35~50만원 이상 추가 지출의 성능 입증 부담을 별도 설명했다.
- [x] 젠하이저 10월 판매가격, 6/7월 반복 특가, HD600 행사 품절, FT1 PRO 조건부 카드 할인 및 포칼 장기 할인 별도 기록.
- [x] 20개 비교쌍에서 구매조건·특성·성능 근거를 검토. 전면적 엄격 Pareto 열위 확정 0건, 후순위 후보 별도 표시.
- [x] 가짜 정밀 점수/음질 향상률/임의 성능 점수 사용하지 않았다.

## Prohibited Shortcuts

- 가장 좋은 제품을 자동으로 가성비 1위로 만들지 않는다.
- 가격대별로 억지로 하나씩 추천하지 않는다.
- MSRP 할인율을 가치 계산에 넣지 않는다.
- 근거 없는 체감 점수 120/145 같은 숫자를 만들어 계산하지 않는다.

## Actual Outputs (2026-10-09)

- `research/09_value_analysis/result.md`: 가격대별 교체 가치 분석과 근거, 29개 전수 판단
- `research/09_value_analysis/value_matrix.csv`: 29개 가격·H7 예상 개선·판단조건
- `research/09_value_analysis/paired_comparisons.csv`: 동가격대/상위단 비교 20건과 상쇄 장점
- `research/09_value_analysis/price_refresh.csv`: 최근 10월 행사, 판매처, 재고·갱신시차 17건
- `data/evidence.csv`: 신규 시장가 E0356–E0369
- `data/price_summary.csv` Step 4 시점 데이터는 이력 보존. Step 9 행사 시나리오는 별도 관리함.

2026-10-09 사용자 승인으로 COMPLETED. handoff.md 작성 후 Step 10 시작.

## Handoff

- Step 10에 역할별 유력 후보를 전달한다.
- 가격 변동 시 재평가가 필요한 후보를 표시한다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
