Status: NOT_STARTED
Stage: 5
Depends on: Step 3, Step 4

# Step 5 — Preliminary Filter

## Objective

정밀 음질 분석 전에 **명백한 기술적·구매 가능성 문제**만 걸러내고, 성능을 확인해야 판단 가능한 후보는 보존한다.

## Inputs

- Step 3 제품 상태
- Step 4 국내 가격
- Step 0 사용자 기준
- data/candidates.csv

## Exact Tasks

1. 오픈/밀폐, 드라이버, 임피던스, 감도, 무게 등 기본 적합성을 확인한다.
2. AE-5로 현실적으로 구동 가능한지 확인한다.
3. 국내에서 실제 구매가 가능한지와 유통/AS 리스크를 확인한다.
4. 사용자 목적과 명백히 충돌하는 기술적 조건이 있는지 확인한다.
5. 가격이 높아 보이더라도 아직 음향 성능을 심층평가하지 않았다면 REJECT하지 않고 HOLD 또는 PASS로 남긴다.
6. REJECT는 구매 불가, 기술적 부적합, 중복/잘못된 모델 식별 등 객관적으로 설명 가능한 사유에 한해 적용한다.
7. 탈락 사유를 decisions/rejected_products.md에 기록한다.
8. 가격 하락이나 신정보 발생 시 재검토할 조건을 명시한다.

## Minimum Coverage

- 모든 후보에 PASS/HOLD/REJECT 상태 부여
- REJECT 제품은 최소 하나의 명시적이고 검증 가능한 사유 기록
- 가격/성능 판단이 필요한 애매한 제품은 REJECT 대신 HOLD 사용
- 가격이 높다는 이유만으로 REJECT된 후보가 없는지 재검토

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/05_pre_filter/result.md
- data/candidates.csv 상태 갱신
- decisions/rejected_products.md

## Completion Gate

- [ ] 모든 후보가 PASS/HOLD/REJECT로 분류되었다.
- [ ] 탈락 제품이 삭제되지 않았다.
- [ ] REJECT 사유와 재검토 조건이 기록되었다.
- [ ] 단순 스펙 숫자로 음질을 추정해 탈락시킨 후보가 없다.
- [ ] 가격만으로 정밀 음질평가 전에 탈락시킨 후보가 없다.

## Prohibited Shortcuts

- 드라이버 크기나 주파수 범위로 음질을 추정해 탈락시키지 않는다.
- 오래된 제품이라는 이유만으로 자동 탈락시키지 않는다.
- 가격이 비싸 보인다는 이유만으로 REJECT하지 않는다.
- 좋아 보이는 제품을 이 단계에서 최종 1위로 확정하지 않는다.

## Handoff

- Step 6과 Step 7에 PASS 및 성능 확인이 필요한 HOLD 후보를 전달한다.
- 탈락 이력을 유지해 동일 제품 중복 조사를 방지한다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
