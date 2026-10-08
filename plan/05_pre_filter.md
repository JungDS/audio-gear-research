Status: COMPLETED
Stage: 5
Depends on: Step 3, Step 4

# Step 5 — Preliminary Filter

## Objective

심층 음질 분석 비용을 절감하면서 **H7 + AE-5 대비 실질적 음질 개선 가능성이 있는 후보**를 최대한 보존한다. 비싸다는 이유만으로 탈락시키지 않되, 충분한 근거가 있는 **명백한 가격 대비 성능 열위**는 초기 단계에서 제외할 수 있다.

## Inputs

- Step 0 H7 + AE-5 Baseline
- Step 3 제품 상태 및 국내 유통 위험
- Step 4 한국시장 정품/수입 분리 가격 스냅샷
- data/candidates.csv 및 data/evidence.csv
- 제조사 연결/구동 조건, 간이 독립 측정/전문 비교 자료

## Exact Tasks

1. 62개 후보 전체의 연결 방식, AE-5 호환성, 구동 가능성, 구매 가능성을 점검한다.
2. 국내 정품과 해외구매·리퍼를 구분하고 가격 확신도가 낮으면 보수적으로 해석한다.
3. 정밀 평가 이전에 비용이 낮은 **동일 용도·가격대 경쟁 제품 간 간이 음질 비교**를 수행한다. 드라이버 크기, 헤드폰 브랜드, MSRP를 음질 근거로 사용하지 않는다.
4. PASS / HOLD / REJECT를 부여한다.
   - PASS: 기술적으로 적합하며 정밀 평가할 가치가 있음.
   - HOLD: 기술·유통·가격·비교 성능에 중요한 확인 필요 사항이 있으나 향후 구매 가치가 남음. 적절한 검증 비용/우선순위를 명시.
   - REJECT: 명백한 구매/호환 불가·동일 SKU 중복·확실한 실사용 부적합 **또는 근거 충분한 가격 대비 성능 열위**.
5. **가성비 열위 REJECT의 필수 요건:** 같은 사용 조건에서 (a) 비교할 실제 후보, (b) 가격의 유통/보증/상태를 맞춘 비교, (c) 적어도 두 개 독립적인 적합한 성능 근거 또는 동급의 강한 측정+실청취 비교, (d) 핵심 음향/착용/기능 면에서 중요한 보완 장점이 없는지 검토. 하나라도 불충분하면 HOLD.
6. 절대가격만 높음, 고가 미래 구매 후보, 출시가 높음, 특정 브랜드 등급은 REJECT 사유로 금지한다.
7. REJECT마다 상대 Candidate_ID, 가격 비교 기준, 성능 비교 항목, Evidence_ID/URL, Confidence, 재검토 조건을 `decisions/rejected_products.md`에 기록하고 `data/candidates.csv`에도 상태와 이유를 보존한다.
8. 연구 비용 절감을 위해 **PASS 우선 심층 분석, HOLD는 의문점이 해소되거나 경쟁구도가 달라질 때 단계적 조사**한다. HOLD를 무기한/임의로 삭제하지 않는다.
9. Step 6 이후 심층 조사나 새 가격/자료가 초기 판단과 충돌하면 재검토한다. 최종 가성비 곡선과 Pareto 비교는 Step 9에서 수행한다.

## Minimum Coverage

- 모든 후보에 PASS/HOLD/REJECT 상태 부여
- REJECT는 직접 검증 가능한 기술/구매 불가 사유 또는 복수 독립 근거에 의한 확실한 가격 대비 성능 열위
- 조건이 불명확하면 HOLD; 높은 가격만으로 REJECT 0건
- 최신 한국 가격이 불확실하면 실제 가격 비교 결론을 보류
- REJECT 포함 모든 후보의 원본 데이터 보존

## Required Outputs

- research/05_pre_filter/result.md
- data/candidates.csv 상태 갱신
- data/evidence.csv: 판정에 직접 쓰인 출처 보강
- decisions/rejected_products.md: 상대 제품·근거·재검토 조건

## Completion Gate

- [x] 62개 후보가 PASS 29 / HOLD 33 / REJECT 0으로 분류되었다.
- [x] 탈락 제품 없음. 최초 후보 62개 ID와 데이터는 모두 유지했다.
- [x] 동급 조건·복수 독립 근거를 충족하는 가격/성능 열위 REJECT가 없어 탈락시키지 않았고 비교 검토 내용을 기록했다.
- [x] 높은 가격만으로 REJECT한 후보는 0개다.
- [x] 모든 HOLD에 검증 질문·비교 후보·관련 출처와 HIGH/MEDIUM/LOW 조사 우선순위를 남겼다.
- [x] 사용자 검토 및 다음 단계 승인 완료.

## Prohibited Shortcuts

- 고가라는 이유만으로 배제 금지
- 싸다고 무조건 통과 금지
- 드라이버 크기/주파수 범위/단일 종합 리뷰점수로 열위 판정 금지
- 단일 추천글이나 커뮤니티 투표만으로 REJECT 금지
- 최신 리비전/연결방식/유통형태가 다른 모델을 동일조건이라고 가정 금지
- 정밀 Step 6/8/9 완료 전 최종 추천 순위 확정 금지

## Actual Outputs (2026-10-09)

- `research/05_pre_filter/result.md` — 62개 전체 검토, 9개 직접 비교 사례, 기술/유통 조건
- `research/05_pre_filter/triage.csv` — 후보 ID별 판정·우선순위·비교 상대·근거·재확인 조건
- `data/candidates.csv` — PASS 29 / HOLD 33 / REJECT 0
- `data/evidence.csv` — Step 5 근거 E0200~E0226
- `decisions/rejected_products.md` — 근거 없는 탈락 0건 기록

2026-10-09 사용자 승인으로 COMPLETED. 연구 handoff를 기록하고 Step 6을 시작했다.

## Recorded Results

- `research/05_pre_filter/result.md`: 62개 전수 분석 및 직접 비교
- `research/05_pre_filter/triage.csv`: 후보별 우선순위와 질문
- `data/candidates.csv`: PASS 29, HOLD 33, REJECT 0
- `data/evidence.csv`: E0200–E0226
- `decisions/rejected_products.md`: 확정 탈락 0건 및 판정 기준
- User review: approved 2026-10-09. Handoff written.

## Handoff

- PASS 및 검증 가치가 남아 있는 HOLD는 Step 6/7에 전달하되, 조사 우선순위와 확인할 의문점을 명확히 한다.
- REJECT의 근거와 재진입 조건을 보존해 후속 재검색 비용을 줄인다.
- 사용자 승인 후에만 COMPLETED로 변경한다.
