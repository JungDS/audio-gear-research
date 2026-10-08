Status: REVIEW
Stage: 2
Depends on: Step 1

# Step 2 — Candidate Discovery

## Objective

서로 독립적인 세 경로에서 후보를 수집하고 중복을 병합해 편향이 적은 후보 풀을 만든다.

## Inputs

- Step 1 브랜드 지도
- RULES.md
- data/candidates.csv

## Exact Tasks

1. 2A Brand-based: 브랜드별 현행/주요 제품에서 후보를 수집한다.
2. 2B Community/Expert-based: Reddit, Head-Fi, ASR, Headphones.com, RTINGS, 네이버 블로그/카페/쇼핑 리뷰, 국내 음향 커뮤니티 및 최근 추천 자료에서 반복 언급 제품을 수집한다.
3. 2C Korea-market-based: 네이버쇼핑, 다나와, 에누리 등의 인기/판매/가격대별 제품을 역탐색한다.
4. 2025~2026년 추천/비교 자료를 우선 검색하고, 오래된 자료는 장기 평판과 측정 보조자료로 구분한다.
5. 검색어를 best overall뿐 아니라 music, movie, general gaming, comfort, value, upgrade from gaming headset 등으로 다양화한다.
6. 네이버의 '2026 헤드폰/헤드셋 추천·순위' 유형 자료는 후보 발견용으로 활용하되 광고/제휴/SEO 가능성을 고려해 최종 성능 근거로 단독 사용하지 않는다.
7. 세 후보군을 병합하고 중복을 제거하되 discovery source는 모두 보존한다.
8. 너무 비싼 제품도 초기 발견 단계에서는 즉시 제거하지 말고 가격 범위 초과로 표시한다.

## Minimum Coverage

- 세 경로 2A/2B/2C를 모두 수행
- 커뮤니티는 Reddit와 Head-Fi 또는 동급 대형 커뮤니티를 포함
- 전문 출처는 측정/리뷰 사이트를 복수 포함
- 국내 발견 경로는 네이버 계열 자료와 한국 음향/쇼핑 자료를 함께 확인
- 한국 시장은 네이버쇼핑·다나와·에누리 중 접근 가능한 출처를 최대한 확인
- 최근 추천 자료는 2025~2026을 우선
- 최초 후보 풀은 충분히 넓게 구성하며 특정 숫자 달성을 위해 품질 낮은 제품을 채우지 않음

자료가 부족하거나 직접 접근이 제한된 경우 억지로 대체하지 않고 `Evidence insufficient` 또는 `Access limited`와 이유를 기록한다.

## Required Outputs

- research/02_candidate_discovery/result.md
- data/candidates.csv
- data/evidence.csv

## Completion Gate

- [x] 2A 완료
- [x] 2B 완료
- [x] 2C 완료
- [x] 최근 추천자료와 장기 현역자료가 구분되었다.
- [x] 중복 후보가 병합되었다.
- [x] 모든 후보에 발견 경로가 기록되었다.
- [x] 조기 최종 순위를 만들지 않았다.
- [x] 최초 브랜드 목록에 종속된 편향을 재점검했다.
- [x] 일반 소비자용/게이밍용 후보의 독립적 발견 경로를 보강했다.
- [x] 기존 후보의 ID·기록을 보존했다.

## Prohibited Shortcuts

- Reddit 인기만으로 후보 가치를 확정하지 않는다.
- 네이버 '추천 순위' 글 하나를 성능 근거로 사용하지 않는다.
- 브랜드 지도에 없다는 이유로 새로운 유력 제품을 배제하지 않는다.
- 가격을 정확히 확인하기 전에 저렴/비싸다고 단정하지 않는다.
- 접근하지 못한 원문을 읽었다고 기록하지 않는다.

## Handoff

- Step 3에 merged candidate pool을 전달한다.
- 각 후보가 어떤 경로에서 발견됐는지 유지한다.
- 최근 자료와 오래된 장기평판 자료를 구분해 전달한다.

최초 43개 후보는 보존했고, 편향 점검 후 일반 소비자·게이밍·국내 시장 역검색으로 19개를 추가하여 **총 62개(C001~C062)**를 기록했다.

추가 보고서: `research/02_candidate_discovery/supplemental_review.md`
근거: `data/evidence.csv` E0054~E0088

보완 범위는 최초 15개 브랜드로 제한하지 않았으며, 원문 접근 불가 네이버 및 확인이 불완전한 에누리 자료는 한계로 명시했다. 사용자가 보완 결과를 검토한 후에만 `COMPLETED`로 변경하고 Step 3으로 진행한다.
