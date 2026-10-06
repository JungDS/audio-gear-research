Status: NOT_STARTED
Stage: 5
Depends on: Step 3, Step 4

# Step 5 — Preliminary Filter

## Objective

정밀 음질 분석 전에 명백히 부적합하거나 가격 경쟁력이 없는 후보를 제거하되 모든 탈락 근거를 보존한다.

## Inputs

- Step 3 제품 상태
- Step 4 국내 가격
- Step 0 사용자 기준
- data/candidates.csv

## Exact Tasks

1. 오픈/밀폐, 드라이버, 임피던스, 감도, 무게 등 기본 적합성을 확인한다.
2. AE-5로 현실적으로 구동 가능한지 확인한다.
3. 마이크/무선 등 불필요 기능 비용 때문에 음질 가성비가 크게 떨어지는 후보를 식별한다.
4. 현행 경쟁 제품과 비교해 가격이 과도하게 높은 후보를 식별한다.
5. 탈락 사유를 decisions/rejected_products.md에 기록한다.
6. 가격 하락이나 신정보 발생 시 재검토할 조건을 명시한다.

## Minimum Coverage

- 모든 후보에 PASS/HOLD/REJECT 상태 부여
- REJECT 제품은 최소 하나의 명시적이고 검증 가능한 사유 기록
- 애매한 제품은 REJECT 대신 HOLD 사용

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/05_pre_filter/result.md
- data/candidates.csv 상태 갱신
- decisions/rejected_products.md

## Completion Gate

- [ ] 모든 후보가 PASS/HOLD/REJECT로 분류되었다.
- [ ] 탈락 제품이 삭제되지 않았다.
- [ ] REJECT 사유와 재검토 조건이 기록되었다.
- [ ] 정밀 음질평가 없이 단순 스펙 숫자로 탈락시킨 후보가 없다.

## Prohibited Shortcuts

- 드라이버 크기나 주파수 범위로 음질을 추정해 탈락시키지 않는다.
- 오래된 제품이라는 이유만으로 자동 탈락시키지 않는다.
- 좋아 보이는 제품을 이 단계에서 최종 1위로 확정하지 않는다.

## Handoff

- Step 6과 Step 7에 PASS 및 필요한 HOLD 후보를 전달한다.
- 탈락 이력을 유지해 동일 제품 중복 조사를 방지한다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
