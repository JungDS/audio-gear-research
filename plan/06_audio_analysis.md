Status: NOT_STARTED
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
6. 항목별 Confidence를 기록한다.

## Minimum Coverage

- 가능한 경우 독립 측정 자료 2개 이상
- 전문 청취평 2개 이상 또는 동급의 충분한 비교 자료
- 자료가 풍부한 제품과 부족한 제품의 Confidence를 차등 적용
- 단일 사이트 점수를 그대로 종합점수로 사용하지 않음

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/06_audio_analysis/result.md
- data/evaluations.csv 음향 항목
- data/evidence.csv

## Completion Gate

- [ ] 핵심 음향 항목이 동일한 기준으로 비교되었다.
- [ ] 객관/주관 근거가 구분되었다.
- [ ] 충돌하는 근거와 불확실성이 기록되었다.
- [ ] 사용자 용도별 평가가 포함되었다.

## Prohibited Shortcuts

- RTINGS 또는 특정 리뷰어 하나의 총점을 그대로 순위로 사용하지 않는다.
- 고역 강조를 해상력과 자동 동일시하지 않는다.
- 측정으로 직접 알 수 없는 체감을 측정치만으로 단정하지 않는다.

## Handoff

- Step 8이 사용할 음향 평가와 Confidence를 전달한다.
- Step 7 결과와 결합하기 전 최종 추천은 하지 않는다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
