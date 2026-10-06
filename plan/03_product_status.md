Status: NOT_STARTED
Stage: 3
Depends on: Step 2

# Step 3 — Product Status & Lifecycle

## Objective

후보의 출시 시점, 생산 상태, 후속 모델, 국내 유통, AS와 소모품 수급을 검증한다.

## Inputs

- Step 2 merged candidate pool
- 제조사 공식 제품/지원 페이지
- 국내 공식 유통 정보

## Exact Tasks

1. 출시연도와 가능하면 출시월을 확인한다.
2. 현행 생산/단종/재고 판매 여부를 확인한다.
3. 후속 모델이나 리비전이 있는지 확인한다.
4. 국내 정식 유통과 보증 경로를 확인한다.
5. 이어패드와 케이블 등 주요 소모품 교체 가능성과 공급 상태를 확인한다.
6. 오래된 재고품일 가능성이 있는 모델을 표시한다.

## Minimum Coverage

- 모든 후보에 Release Year와 Current/Discontinued 상태 기록
- 모든 후보에 Successor/Revision 여부 기록
- 가능한 모든 후보에 국내 AS/부품 상태 기록
- 확인이 불가능한 항목은 UNKNOWN으로 명시

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/03_product_status/result.md
- data/candidates.csv 갱신
- data/evidence.csv 갱신

## Completion Gate

- [ ] 모든 후보의 출시 시점과 현행 여부가 기록되었다.
- [ ] 후속 제품 여부가 기록되었다.
- [ ] 국내 유통/AS/소모품 상태가 가능한 범위에서 확인되었다.
- [ ] 구형 재고 리스크가 별도 표시되었다.

## Prohibited Shortcuts

- 구형이라는 이유만으로 자동 탈락시키지 않는다.
- 공식 판매 페이지가 남아 있다는 이유만으로 현행 생산이라고 단정하지 않는다.
- 병행수입과 정식유통을 동일하게 취급하지 않는다.

## Handoff

- Step 4가 가격 조사 시 정식유통/병행수입을 구분할 수 있게 상태정보를 전달한다.
- Step 5의 신형 우선 원칙 적용에 필요한 출시/후속정보를 전달한다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
