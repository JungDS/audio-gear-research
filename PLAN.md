# Master Research Plan

이 파일은 **전체 프로젝트의 지도와 단계 상태 요약만 관리한다.**  
각 단계의 실제 실행 절차는 `plan/` 아래 상세 파일이 유일한 기준이다.

## Project Goal

한국 시장에서 실제 구매 가능한 헤드폰/헤드셋 중 **Creative Sound BlasterX H7 Tournament Edition + Sound BlasterX AE-5**보다 음악, 일반 게임, 애니메이션, 영화 및 일상 감상에서 체감 가능한 향상을 제공하는 제품을 찾는다.

## Status Source of Truth

- 현재 작업 위치의 기준: `STATUS.md`
- 개별 단계 상태의 기준: 해당 `plan/XX_*.md` 첫 줄
- 아래 Master Index의 Status는 **요약 미러**이며 단계 파일과 항상 함께 갱신한다.
- 상태가 충돌하면 단계 파일을 우선하고, `PLAN.md`와 `STATUS.md`를 즉시 동기화한다.

## Master Index

| Step | Stage | Status | Depends on | Detail |
|---:|---|---|---|---|
| 0 | Baseline | COMPLETED | Setup | [plan/00_baseline.md](plan/00_baseline.md) |
| 1 | Brand Map | COMPLETED | 0 | [plan/01_brand_map.md](plan/01_brand_map.md) |
| 2 | Candidate Discovery | COMPLETED | 1 | [plan/02_candidate_discovery.md](plan/02_candidate_discovery.md) |
| 3 | Product Status & Lifecycle | COMPLETED | 2 | [plan/03_product_status.md](plan/03_product_status.md) |
| 4 | Korean Market Price Research | COMPLETED | 3 | [plan/04_price_research.md](plan/04_price_research.md) |
| 5 | Preliminary Filter | COMPLETED | 3, 4 | [plan/05_pre_filter.md](plan/05_pre_filter.md) |
| 6 | Audio Performance Analysis | COMPLETED | 5 | [plan/06_audio_analysis.md](plan/06_audio_analysis.md) |
| 7 | Comfort, QC & Durability | COMPLETED | 5 | [plan/07_comfort_quality.md](plan/07_comfort_quality.md) |
| 8 | Direct Comparison vs H7 + AE-5 | COMPLETED | 6, 7 | [plan/08_vs_current.md](plan/08_vs_current.md) |
| 9 | Value Curve | IN_PROGRESS | 4, 8 | [plan/09_value_analysis.md](plan/09_value_analysis.md) |
| 10 | Finalists | NOT_STARTED | 9 | [plan/10_finalists.md](plan/10_finalists.md) |
| 11 | Counter Review | NOT_STARTED | 10 | [plan/11_counter_review.md](plan/11_counter_review.md) |

## Global Stage Procedure

모든 단계는 다음 순서로 진행한다.

1. `STATUS.md` 확인
2. 현재 단계의 `plan/XX_*.md` 확인
3. `RULES.md`에서 관련 전역 규칙 확인
4. 현재 단계 Input 확인
5. Exact Tasks 순서대로 수행
6. 근거를 `data/evidence.csv`에 기록
7. 구조화 데이터와 `research/XX_*/result.md` 갱신
8. Completion Gate 전부 점검
9. 사용자에게 단계 결과 공유
10. 사용자 피드백 반영
11. `templates/handoff_template.md` 형식으로 `research/XX_*/handoff.md` 작성
12. 단계 파일, `STATUS.md`, Master Index 상태를 함께 갱신

## State Transition Rule

`NOT_STARTED → IN_PROGRESS → REVIEW → COMPLETED`

필요한 경우:
- 외부 자료 접근, 정보 부족 등으로 진행 불가: `BLOCKED`
- 사용자 검토 후 보완 필요: `REVIEW` 유지
- Gate 미충족: 다음 단계 진입 금지

## Return Rule

후속 단계에서 치명적인 오류 또는 새로운 경쟁제품이 발견되면 이전 단계로 되돌아갈 수 있다.  
되돌아간 이유와 영향 범위는 `decisions/decision_log.md`에 기록한다.

## No Early Conclusion Rule

후보 수집 및 중간 분석 중 특정 제품이 매우 좋아 보여도 Step 10 이전에는 최종 추천으로 확정하지 않는다.
