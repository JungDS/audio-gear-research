Status: REVIEW
Stage: 10
Depends on: Step 9

# Step 10 — Finalists

## Objective

실제로 구매 검토할 가치가 있는 소수의 최종 후보를 역할별로 선정한다.

## Inputs

- Step 9 가치 분석
- Step 8 H7 비교
- Step 3 제품 현재성
- Step 7 착용/QC

## Exact Tasks

1. 역할이 겹치지 않는 최종 후보를 선정한다.
2. 최소비용 확실한 업그레이드 후보를 검토한다.
3. 전체 가성비 최적 후보를 검토한다.
4. 추가 지출 가치가 있는 상한선 후보를 검토한다.
5. 필요한 경우 특정 성향 특화 후보를 별도로 둔다.
6. 각 후보의 핵심 장점, 약점, 적정 구매가격을 정리한다.

## Minimum Coverage

- 후보 수를 억지로 채우지 않음
- 역할이 사실상 동일한 후보 중복 제거
- 각 후보에 추천 조건과 비추천 조건 모두 기록

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/10_finalists/result.md
- 최종 후보 목록 및 적정 구매가격

## Completion Gate

- [x] 핵심 후보 4개 역할 분리(오픈형 저비용·밀폐형 영화·오픈 평판형·보컬 참조).
- [x] 모델별 긍정 근거, 불이익, 구매/비구매 조건을 기록했다.
- [x] H7 패시브 아날로그 대비 예측 개선 방향과 직접 A/B 불확실성을 구분했다.
- [x] 핵심 4개 + 대안 2개 + 고가 실청 검증 2개 및 신규 HD650 반론 대상을 기록했다.

## Prohibited Shortcuts

- 반론검증 전에 최종 구매 결론으로 확정하지 않는다.
- 브랜드 선호로 후보를 추가하거나 제거하지 않는다.
- 실제 가격을 무시하고 절대성능만으로 후보를 선정하지 않는다.

## Actual outputs (2026-10-09)

- `research/10_finalists/result.md` — 핵심 최종 검토 4개, 대안 2개, 고가 장기 실청 후보 2개
- `research/10_finalists/shortlist.csv` — 제품별 역할·가격조건·장단점·Step11 반론
- `research/10_finalists/market_gates.csv` — 한국 판매조건/품절/특가 반품 제한
- `data/evidence.csv` — Step10 근거 E0370–E0385
- 미포함 HD650 행사물량 품절 및 HD600 경쟁자 문제를 Step11 검증 항목으로 기록

**REVIEW:** 사용자 승인 전에는 Step11 반론검증을 시작하지 않는다.

## Handoff

- Step 11에 최종 후보와 추천 논리를 전달한다.
- 각 후보가 탈락할 수 있는 핵심 리스크 가설도 함께 넘긴다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
