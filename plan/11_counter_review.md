Status: NOT_STARTED
Stage: 11
Depends on: Step 10

# Step 11 — Counter Review

## Objective

최종 후보 각각에 대해 의도적으로 반대 근거를 찾아 확증편향을 줄이고 최종 결론을 검증한다.

## Inputs

- Step 10 finalists
- 모든 이전 단계 결과
- 최신 가격/제품 상태

## Exact Tasks

1. 각 후보에 대해 왜 사면 안 되는가를 별도로 조사한다.
2. 최근 경쟁 신제품과 가격 변화를 재검색한다.
3. 숨겨진 QC, 장시간 착용, AS, 패드/부품 문제를 재검토한다.
4. 추천 근거가 특정 리뷰어/커뮤니티에 편중됐는지 확인한다.
5. 치명적 문제 발견 시 해당 단계로 되돌려 재평가한다.
6. 최종 추천과 불확실성을 정리한다.

## Minimum Coverage

- 최종 후보마다 최소 하나의 반대 가설을 검증
- 최신 시장가격 재확인
- 최근 경쟁제품 누락 여부 재검색
- 기존 근거와 독립적인 부정적 자료 탐색

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/11_counter_review/result.md
- 최종 recommendation summary
- decisions/decision_log.md 필요 시 갱신

## Completion Gate

- [ ] 모든 최종 후보의 반대 근거가 검토되었다.
- [ ] 치명적 문제 발생 시 재평가가 완료되었다.
- [ ] 최종 결론의 Confidence와 불확실성이 명시되었다.
- [ ] 최종 구매 판단에 필요한 가격 조건이 명시되었다.

## Prohibited Shortcuts

- 기존 추천을 방어하기 위해 반대 근거를 축소하지 않는다.
- 새로운 치명적 정보를 발견하고도 이전 결론을 유지하지 않는다.
- 최종 가격을 재확인하지 않고 종료하지 않는다.

## Handoff

- 최종 결과를 사용자에게 공유한다.
- 향후 가격 변화 시 어떤 조건에서 재검토할지 남긴다.
- 프로젝트 STATUS를 완료 또는 모니터링 상태로 갱신한다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
