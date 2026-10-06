# audio-gear-research

Evidence-based research for audio gear upgrades and purchasing decisions.

## Current Project

현재 사용 중인 **Creative Sound BlasterX H7 + Sound Blaster AE-5** 조합보다 음악, 일반 게임, 애니메이션, 영화 및 일상 감상에서 **체감 가능한 업그레이드**가 되는 헤드폰/헤드셋을 한국 시장 기준으로 찾는다.

이 프로젝트는 출시가나 명목 할인율이 아니라 실제 국내 판매가, 객관적 측정, 전문 리뷰, 장기 사용자 후기, 착용감, QC, AS, 소모품 수급과 제품 현재성을 함께 평가한다.

## Start Here

새 작업 세션에서는 다음 순서로 읽는다.

1. [STATUS.md](STATUS.md) — 현재 위치와 다음 작업
2. 현재 단계의 `plan/XX_*.md` — 해당 단계의 상세 실행 명세
3. [RULES.md](RULES.md) — 전역 평가 규칙
4. 필요한 경우 [PLAN.md](PLAN.md) — 전체 프로젝트 지도와 전후 단계
5. 관련 `research/`, `data/`, `decisions/` 자료

## Repository Structure

- `PLAN.md` — 전체 연구 단계의 Master Index
- `RULES.md` — 모든 단계에 적용되는 고정 규칙
- `STATUS.md` — 현재 진행상태와 다음 액션
- `CHANGELOG.md` — 방법론 및 구조 변경 이력
- `plan/` — 단계별 상세 실행 명세
- `research/` — 단계별 조사 결과
- `data/` — 후보, 가격, 근거, 평가의 구조화 데이터
- `decisions/` — 판단 변경과 탈락 기록
- `templates/` — 반복 조사에 사용하는 템플릿

## Stage Status

각 단계 파일의 첫 줄은 다음 상태 중 하나를 사용한다.

- `NOT_STARTED`
- `IN_PROGRESS`
- `BLOCKED`
- `REVIEW`
- `COMPLETED`

Gate가 모두 충족되기 전에는 `COMPLETED`로 변경하지 않는다.

## Public Repository Policy

이 저장소는 Public이다.

다음 정보는 기록하지 않는다.

- 개인 식별정보
- 계정/로그인 정보
- 비공개 문서나 비공개 URL
- 주문번호, 주소, 전화번호 등 구매자의 개인정보
- API key, token, cookie 등 인증정보

연구에 필요한 하드웨어 환경과 공개 자료만 기록한다.
