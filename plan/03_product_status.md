Status: COMPLETED
Stage: 3
Depends on: Step 2

# Step 3 — Product Status & Lifecycle

## Objective

후보의 출시 시점, 생산 상태, 리비전, 후속 모델, 국내 유통, AS와 소모품 수급을 검증한다.

## Inputs

- Step 2 merged candidate pool
- 제조사 공식 제품/지원 페이지
- 국내 공식 유통 정보

## Exact Tasks

1. 출시연도와 가능하면 출시월을 확인한다.
2. 현행 생산/단종/재고 판매 여부를 확인한다.
3. 리비전 변경과 후속 모델이 있는지 확인한다.
4. 국내 정식 유통과 보증 경로를 확인한다.
5. 이어패드와 케이블 등 주요 소모품 교체 가능성과 공급 상태를 확인한다.
6. 오래된 생산/재고품일 가능성을 직접 확정할 수 있는지 확인하고, 불가능하면 정황상 재고 노후 위험도를 HIGH/MEDIUM/LOW/UNKNOWN으로 기록한다.
7. 오래된 모델은 신품 생산 지속 여부와 실제 재고 연령을 구분한다.

## Minimum Coverage

- 모든 후보에 Release Year와 Current/Discontinued 상태 기록
- 가능한 경우 Revision 기록
- 모든 후보에 Successor 여부 기록
- 가능한 모든 후보에 국내 AS/부품 상태 기록
- Inventory Age Risk 기록
- 확인이 불가능한 항목은 UNKNOWN으로 명시

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/03_product_status/result.md
- data/candidates.csv 갱신
- data/evidence.csv 갱신

## Completion Gate

- [x] 모든 후보의 출시 시점(확인 불가 시 UNKNOWN)과 현행 상태가 기록되었다.
- [x] 확인 가능한 리비전/후속 제품이 기록되고 확인 불가는 UNKNOWN으로 남겼다.
- [x] 국내 유통/AS/소모품을 공식 자료로 확인 가능한 범위에서 기록하고 나머지는 UNKNOWN으로 남겼다.
- [x] 단종 모델의 구형 재고 가능성을 분리 표시하고 재고 제조일은 추정하지 않았다.
- [x] 실제 생산일을 모르는 경우 추정과 사실을 구분했다.

## Prohibited Shortcuts

- 구형이라는 이유만으로 자동 탈락시키지 않는다.
- 공식 판매 페이지가 남아 있다는 이유만으로 현행 생산이라고 단정하지 않는다.
- 병행수입과 정식유통을 동일하게 취급하지 않는다.
- 판매 중이라는 사실만으로 재고 생산연도를 추정해 확정하지 않는다.

## Handoff

- Step 4가 가격 조사 시 정식유통/병행수입을 구분할 수 있게 상태정보를 전달한다.
- Step 5의 신형 우선 원칙 적용에 필요한 출시/리비전/후속정보를 전달한다.

Step 3 조사 보고서는 `research/03_product_status/result.md`에 기록했다. 62개 중 CURRENT 47 / DISCONTINUED 2 / UNKNOWN 13; 국내 모델별 공식 유통 TRUE 22 / UNKNOWN 40. 이 불확실성은 후속 단계의 핵심 리스크이며, 사용자가 다음 단계 진행을 승인하여 2026-10-09 COMPLETED로 처리했다. `research/03_product_status/handoff.md` 작성 완료.
