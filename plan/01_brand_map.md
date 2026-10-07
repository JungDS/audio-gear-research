Status: IN_PROGRESS
Stage: 1
Depends on: Step 0

# Step 1 — Brand Map

## Objective

특정 제조사 편향 없이 현재 헤드폰/헤드셋 시장에서 조사할 가치가 있는 브랜드와 현행 라인업을 지도화한다.

## Inputs

- Step 0 결과
- RULES.md
- 브랜드 공식 사이트 및 국내 유통 정보

## Exact Tasks

1. 음향 전문 브랜드와 음질 평가가 좋은 게이밍 브랜드를 폭넓게 수집한다.
2. 브랜드별 현재 보급형·중급형·대표 가성비·주력 모델을 확인한다.
3. 최근 2~3년 출시 제품과 장기 현역 모델을 구분한다.
4. 국내 정식 유통/AS 존재 여부를 1차 확인한다.
5. 브랜드별 후보 편중 여부를 점검한다.

## Minimum Coverage

- 목표 브랜드 수 약 12~15개를 기본으로 하되 시장 상황에 따라 조정
- Sennheiser, Beyerdynamic, Audio-Technica, AKG, Sony, FiiO, HIFIMAN, Philips, Shure 등 주요 범주 누락 여부 확인
- 국내에서 의미 있는 신흥/가성비 브랜드 추가 탐색
- 최근 브랜드 라인업은 공식 사이트와 최신 시장 자료로 교차확인

자료가 부족한 경우 억지로 숫자를 채우지 않고 `Evidence insufficient`와 이유를 기록한다.

## Required Outputs

- research/01_brand_map/result.md
- data/evidence.csv 갱신

Step 1은 브랜드 지도를 만드는 단계이며 `data/candidates.csv`에는 아직 후보 제품을 등록하지 않는다. 후보 등록은 Step 2에서 시작한다.

## Completion Gate

- [ ] 주요 음향 브랜드가 충분히 포함되었다.
- [ ] 각 브랜드의 현행 주요 제품군을 확인했다.
- [ ] 특정 제조사가 이유 없이 과대표집되지 않았다.
- [ ] 신형/구형 라인업이 구분되었다.

## Prohibited Shortcuts

- 브랜드 인지도 자체를 음질 점수로 사용하지 않는다.
- 이 단계에서 특정 제품을 후보 DB 또는 최종 후보로 확정하지 않는다.
- 공식 MSRP를 제품 급의 근거로 사용하지 않는다.

## Handoff

- Step 2A가 사용할 브랜드 및 라인업 목록을 전달한다.
- 시장/커뮤니티 기반 탐색에서 누락 여부를 검증할 수 있도록 브랜드 범위를 기록한다.

완료 후 이 파일의 Status를 `REVIEW`로 변경하고 사용자 검토를 거친 뒤에만 `COMPLETED`로 변경한다.
