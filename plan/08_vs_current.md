Status: IN_PROGRESS
Stage: 8
Depends on: Step 6, Step 7

# Step 8 — Direct Comparison vs H7 + AE-5

## Objective

각 후보가 현재 H7 + AE-5 대비 실제로 무엇을 얼마나 개선하거나 악화하는지 변화 벡터로 비교한다.

## Inputs

- Step 0 baseline
- Step 6 음향 분석
- Step 7 착용/QC 분석
- 현재 사용자 우선순위

## Exact Tasks

1. 각 후보를 해상력, 분리도, 이미징, 공간감, 다이내믹, 보컬, 저역 질, 고역 품질, 착용감으로 비교한다.
2. 음악, 일반 게임, 애니메이션, 영화 용도별 차이를 비교한다.
3. 성능 변화는 ↑↑↑/↑↑/↑/→/↓/↓↓/↓↓↓로 표현하고 데이터에는 UP3/UP2/UP1/SAME/DOWN1/DOWN2/DOWN3으로 기록한다.
4. 저음 **양감**은 우열이 아니라 변화이므로 MORE/SAME/LESS로 별도 기록한다.
5. 좋은 제품과 실제 업그레이드 제품을 구분한다.
6. 핵심 항목 개선이 작은 제품은 명확히 표시한다.
7. 비교 전체의 Confidence를 기록한다.

## Minimum Coverage

- 모든 생존 후보에 동일 비교항목 적용
- 변화 벡터마다 Step 6/7 근거와 연결
- 사용자의 현재 체감과 외부 자료가 충돌하면 불확실성 표시
- data/evaluations.csv의 H7 비교 필드와 result.md 항목 일치

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/08_vs_current/result.md
- data/evaluations.csv의 H7 비교 필드
- H7_Comparison_Confidence

## Completion Gate

- [ ] 모든 후보에 동일한 변화 벡터가 작성되었다.
- [ ] 핵심 용도별 개선/악화가 명확하다.
- [ ] 저음 양감 변화와 저음 품질 우열이 분리되었다.
- [ ] 체감 향상이 애매한 후보가 별도 표시되었다.
- [ ] 단순 절대성능과 교체가치가 분리되었다.
- [ ] 비교 Confidence가 기록되었다.

## Prohibited Shortcuts

- 종합점수 하나로 차이를 숨기지 않는다.
- 가격을 아직 체감 차이 자체에 섞지 않는다.
- 무선/마이크 기능을 음질 개선으로 계산하지 않는다.
- 저음이 많아졌다는 이유만으로 개선으로 판단하지 않는다.

## Handoff

- Step 9에 가격과 독립된 업그레이드 크기를 전달한다.
- Step 9에서 가격을 결합해 가치 분석을 수행한다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
