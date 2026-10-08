Status: REVIEW
Stage: 6
Depends on: Step 5

# Step 6 — Audio Performance Analysis

## Objective

생존 후보의 실제 음향 성능을 객관적 측정과 복수 청취평으로 심층 비교한다.

## Inputs

- Step 5 생존 후보
- Step 0 baseline
- data/evidence.csv
- 측정/전문 리뷰 자료

## Exact Tasks

1. 주파수응답과 저역 확장을 확인한다.
2. 왜곡, 채널 매칭, 감도/임피던스 특성을 가능한 범위에서 확인한다.
3. 해상력, 분리도, 이미징, 사운드스테이지, 다이내믹, 보컬, 저역 질감, 고역 피로도에 대한 전문 청취평을 수집한다.
4. 측정과 청취평이 일치하는 부분과 충돌하는 부분을 분리한다.
5. 음악·영화·애니메이션·일반 게임에 대한 적합성을 분석한다.
6. 음향 전반과 용도별 평가에 각각 Confidence를 기록한다.

## Minimum Coverage

- 가능한 경우 독립 측정 자료 2개 이상
- 전문 청취평 2개 이상 또는 동급의 충분한 비교 자료
- 자료가 풍부한 제품과 부족한 제품의 Confidence를 차등 적용
- 단일 사이트 점수를 그대로 종합점수로 사용하지 않음

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/06_audio_analysis/result.md
- data/evaluations.csv 음향/용도 항목 및 Audio_Confidence, Use_Case_Confidence
- data/evidence.csv

## Completion Gate

- [x] 29개 PASS의 FR·저역·중역·고역·왜곡·채널 매칭을 동일 항목으로 기록하고 근거 부족은 UNKNOWN.
- [x] 측정, 실제 청취평, 제조사 사양을 구분해 출처별 기록.
- [x] 측정 규격 차이, 신형 자료 부족, 리뷰 불일치, FT3 리비전과 MK2 임피던스 논쟁을 기록.
- [x] 음악·애니 대사·영화·일반 게임의 잠정 적합성과 실제 청취 테스트 미완료를 분리.
- [x] 객관적 근거 확신과 사용자 용도 추정 확신을 별도로 기록.

## Prohibited Shortcuts

- RTINGS 또는 특정 리뷰어 하나의 총점을 그대로 순위로 사용하지 않는다.
- 고역 강조를 해상력과 자동 동일시하지 않는다.
- 측정으로 직접 알 수 없는 체감을 측정치만으로 단정하지 않는다.

## Actual outputs (2026-10-09)

- `research/06_audio_analysis/result.md`: 핵심 12개 음향 성향 및 평가 충돌
- `research/06_audio_analysis/acoustic_matrix.csv`: 전체 PASS 29개 모델과 출처/측정/청취/충돌/Confidence
- `research/06_audio_analysis/additional_17.md`: 나머지 17개 비교분석
- `research/06_audio_analysis/metadata_corrections.md`: FT1 PRO 출시연도, FT3 임피던스별 리비전, AR5000 MK2 사양 충돌
- `data/evaluations.csv`: PASS 29개 구조화 평가, H7 비교 필드 UNKNOWN 유지
- `data/evidence.csv`: E0227–E0288(62개 출처 기록)

독립 측정자료가 충분하지 않은 모델(특히 신형/전문 제품)은 LOW로 표시했다. `Independent_Source_2`의 출처가 공식 매뉴얼이거나 같은 RTINGS 비교이면 **독립된 두 번째 측정실로 계산하지 않는다**. 수치적 객관 평가를 억지로 채우지 않는다.

Step 6 조사 결과는 REVIEW 상태이며 사용자가 승인하기 전 Step 7로 이동하지 않는다.

## Handoff

- Step 8이 사용할 음향 평가와 Confidence를 전달한다.
- Step 7 결과와 결합하기 전 최종 추천은 하지 않는다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
