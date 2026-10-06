# Data Directory

구조화 데이터는 사람이 읽는 연구 보고서와 분리해 관리한다.

## Files

- `candidates.csv` — 제품 마스터 및 상태
- `prices.csv` — 판매처별 국내 가격 원자료 스냅샷
- `price_summary.csv` — 후보별 통상가/현재 최저가/특가 요약
- `evidence.csv` — 모든 근거 출처 레지스트리
- `evaluations.csv` — 음질/착용/H7 대비 평가
- `schema.md` — 필드 정의와 허용값

원자료 행은 가능한 한 삭제하지 않고 상태/시점을 추가해 추적성을 유지한다.
