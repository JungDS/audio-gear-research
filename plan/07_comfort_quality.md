Status: COMPLETED
Stage: 7
Depends on: Step 5

# Step 7 — Comfort, QC & Durability

## Objective

장시간 착용감, QC, 내구성, 패드와 부품 문제를 실사용 자료 중심으로 검증한다.

## Inputs

- Step 5 생존 후보
- 커뮤니티 장기 후기
- 국내 실사용 후기
- 공식 부품/보증 자료

## Exact Tasks

1. 측압, 정수리 압박, 무게 배분을 조사한다.
2. 이어컵 깊이와 귀 접촉 문제를 확인한다.
3. 패드 열감, 안경 착용, 2시간 이상 사용 후 피로도를 확인한다.
4. 패드 열화, 힌지, 케이블, 드라이버 편차 등 반복 QC 이슈를 조사한다.
5. 교체 패드/케이블 가격과 구입 가능성을 확인한다.
6. 개인 체형 차이와 반복적인 구조적 문제를 구분한다.

## Minimum Coverage

- Reddit 또는 동급 대형 커뮤니티 장기 사용 사례 확인
- Head-Fi 또는 동급 전문 커뮤니티 자료 확인 가능 시 포함
- 국내 사용자 리뷰 가능한 경우 복수 확인
- 문제 주장은 반복 횟수와 출처 독립성을 함께 고려

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/07_comfort_quality/result.md
- data/evaluations.csv 착용/QC 항목
- data/evidence.csv

## Completion Gate

- [x] 29개 PASS 장시간 착용·측압·컵 깊이·안경/열감 특성과 근거 부족을 기록했다.
- [x] 제조사 공식 인정·서로 다른 사용자 보고·일화·자료 부족을 구분했다.
- [x] 공식 교체부품과 국내 재고/가격 확인 여부를 분리했다.
- [x] 29개 모델에 착용감·QC 별도 Confidence를 기록했다.

## Prohibited Shortcuts

- 무게 숫자만으로 편안함을 판정하지 않는다.
- 단일 불만 후기를 구조적 결함으로 일반화하지 않는다.
- 초기 착용감과 장시간 착용감을 혼동하지 않는다.

## Actual Outputs (2026-10-09)

- `research/07_comfort_quality/result.md`: 29개 결과 및 QC 위험·부품·국내 서비스 교차분석
- `research/07_comfort_quality/comfort_qc_matrix.csv`: 후보별 장시간 착용·안경·열감·측압·부품·QC 종류
- `data/evaluations.csv`: 29개 Comfort/QC/Parts 및 별도 Confidence 보강
- `data/evidence.csv`: E0289–E0352 (64건 근거)
- `data/candidates.csv`: FT1 PRO 출시연도 2024 정정, FT3 버전 불명확 표기
- `research/06_audio_analysis/metadata_corrections.md`: 과거 미해결 사항 일부 정리

사용자 승인으로 2026-10-09 COMPLETED. `research/07_comfort_quality/handoff.md` 작성 후 Step 8에 진행한다.

## Handoff

- Step 8에 착용감/QC 평가를 전달한다.
- 치명적 QC 문제 발견 시 Step 5 재검토 후보로 표시한다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
