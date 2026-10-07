# Step 0 — Baseline Result

Date: 2026-10-07
Status: REVIEW

## 1. Reference System

현재 비교 기준은 다음과 같이 고정한다.

- **Headset:** Creative Sound BlasterX H7 Tournament Edition
- **Connection:** H7 TE 3.5mm analog → Sound BlasterX AE-5 headphone output
- **DAC / amplifier:** AE-5 ESS ES9016K2M + Xamp
- **Primary listening mode:** AE-5 Direct Mode를 중요한 기준으로 사용
- **Alternative mode:** 필요 시 AE-5 SBX/effects 사용
- **H7 internal USB DAC/DSP:** 현재 3.5mm 경로에서는 사용하지 않음

중요: H7 TE 자체 USB DSP 상태의 평가와 현재 AE-5 아날로그 연결 상태의 평가를 혼합하지 않는다.

근거: E0001, E0002, E0003, E0004, E0005

---

## 2. Hardware Baseline

### H7 Tournament Edition

공식 사양:
- Closed-back over-ear gaming headset
- 50mm neodymium dynamic driver
- 20Hz–20kHz
- 32Ω
- 118dB/mW @ 1kHz
- USB 및 3.5mm analog 지원

Creative의 공식 364g 표기는 마이크/USB 케이블/아날로그 케이블 포함 무게다. 독립 측정 자료는 헤드폰 자체를 약 290g으로 기재하므로 두 수치를 직접 비교하지 않는다.

### AE-5

공식 사양:
- ESS ES9016K2M DAC
- Xamp discrete headphone amplifier
- Output impedance: 1Ω
- Supported headphone impedance: 16–600Ω
- 232mW @ 16Ω
- 46.8mW @ 600Ω

**Baseline interpretation:** H7 TE의 32Ω 부하는 AE-5의 정상 구동 범위 안에 충분히 들어온다. 독립 측정상 H7 TE의 임피던스 곡선도 비교적 평탄하므로, 현재 조합에서 앰프 출력 임피던스 상호작용 때문에 주파수응답이 크게 변할 가능성은 낮다.

따라서 이후 업그레이드 조사에서 현재 시스템의 주된 한계는 **AE-5의 구동력 부족보다 H7 TE 자체 드라이버/튜닝/구조** 쪽으로 본다.

근거: E0004, E0006

---

## 3. Connection-Mode Caveat

H7 TE는 연결 방식에 따라 성향이 달라질 수 있다.

- H7 자체 USB 연결: 내부 DAC/DSP 및 Creative 보정 가능
- 3.5mm analog: H7 자체 USB DSP를 우회
- 현재 시스템: 3.5mm analog + AE-5

Sound Blaster Command의 Direct Mode는 적용된 오디오 효과를 비활성화하고 소스를 직접 출력한다.

따라서 **현재 Direct Mode 기준은 H7 TE의 패시브 아날로그 특성 + AE-5 DAC/amp 특성**으로 보는 것이 적절하다. SBX를 켠 경우에는 AE-5의 DSP 효과가 추가된 별도 상태로 취급한다.

근거: E0001, E0005, E0006

---

## 4. Tonal / Technical Baseline

### Bass quantity
**Baseline:** 다소 많음 / 따뜻한 성향

독립 패시브 측정에서는 약 80–300Hz 구간의 저역 상승이 관찰된다.

### Bass quality
**Baseline:** 보통

양감은 있으나 독립 측정/청취평에서는 tight한 저역보다는 다소 두껍고 느슨한 성향으로 평가된다.

### Midrange / vocal presence
**Baseline:** 약점 후보

패시브 측정에서 bass-to-presence 영역의 큰 하강이 관찰되며, 일부 전문 리뷰에서도 중역이 덜 두드러진다고 평가한다.

따라서 향후 후보에서 **보컬 자연스러움, 중역 존재감, 대사 명료도**가 개선되는지를 중요하게 본다.

### Treble
**Baseline:** 존재감은 있으나 finesse는 제한적

측정/리뷰를 종합하면 고역 존재감 자체는 부족하지 않지만, 세밀함과 공기감은 상급 Hi-Fi 헤드폰 기준으로 약점이 될 수 있다.

### Resolution / fine detail
**Baseline:** 게이밍 헤드셋으로는 양호, 업그레이드 여지 큼

일부 리뷰는 높은 선명도와 분리를 평가하지만, 측정 리뷰에서는 고역 강조로 인한 'detail impression'과 실제 미세 뉘앙스를 구분한다.

향후 후보는 단순히 고역이 밝은 제품이 아니라 **실제 미세정보, 악기 texture, 복잡한 구간의 분리**가 좋아져야 한다.

### Separation
**Baseline:** 비교적 강점

전문 리뷰에서 복잡한 게임/영화 장면에서도 효과음 분리가 좋은 편으로 평가된다.

### Imaging
**Baseline:** 게임용으로 준수

3.5mm 사용에서도 방향 정보가 괜찮다는 리뷰가 있으나, 경쟁 FPS가 사용자 핵심 용도는 아니므로 과대가중하지 않는다.

### Soundstage
**Baseline:** 밀폐형 기준 보통~양호

분리감은 장점이지만 물리적으로 밀폐형이며, 이후 오픈형/대형 드라이버 제품과 비교할 때 공간 확장 가능성이 큰 영역이다.

근거: E0006, E0007, E0008

---

## 5. Comfort / Isolation / Durability Baseline

### Comfort
**Baseline:** 강점

복수 전문 리뷰와 사용자 의견에서 장시간 착용 편의성이 반복적으로 긍정 평가된다.

따라서 새 제품이 음질은 좋아도 착용감이 명확히 나빠지면 강한 감점 요인으로 본다.

### Isolation
**Baseline:** 밀폐형의 높은 차음성이 장점

외부 소음을 줄이고 영화/게임 몰입에 유리하다. 오픈형 후보는 음질/공간감이 좋아져도 이 부분은 trade-off로 기록한다.

### Long-term material durability
**Baseline:** 노후 제품에서 주의

장기 사용자 사례에서 leather-effect material flaking이 보고되었다. 단일 사례이므로 보편적 결함으로 단정하지 않지만, 현재 제품 세대의 나이와 패드/표면재 노화는 교체 가치를 높이는 요소가 될 수 있다.

근거: E0007, E0008, E0009, E0010

---

## 6. Use-case Baseline

| Use case | Current baseline | Main reason |
|---|---|---|
| Music | 보통~양호 | 저역/에너지와 분리는 괜찮지만 중역 자연스러움·미세 뉘앙스·공기감에 업그레이드 여지 |
| General games | 양호 | 분리, 이미징, 밀폐 몰입감이 강점 |
| Animation | 보통~양호 | 대사는 충분히 들리지만 보컬/중역 자연스러움 개선 여지 |
| Movies | 양호 | 저역 임팩트, 분리, 차음이 유리 |
| Everyday listening | 양호 | 착용감 강점; 유선 여부는 사용자에게 중요하지 않음 |
| Competitive FPS | 참고만 | 현재도 충분히 기능하나 사용자 우선순위가 낮음 |

이 평가는 절대 점수가 아니라 향후 후보의 **변화 방향을 측정하기 위한 출발점**이다.

---

## 7. User-Priority Profile for Later Steps

숫자 가중치는 사용하지 않고 다음 우선순위 계층으로 고정한다.

### Tier A — 핵심
1. H7 + AE-5보다 실제로 들었을 때 분명한 음질 향상
2. Resolution / separation / natural midrange / bass quality / soundstage 개선
3. 음악·일반 게임·애니메이션·영화 전반에서의 범용성

### Tier B — 중요
4. 장시간 착용감
5. 현재 한국 실판매가 대비 업그레이드 가치
6. AS / 부품 / 제품 현재성

### Tier C — 낮은 우선순위
7. 경쟁 FPS 특화
8. 무선 편의성
9. 마이크
10. RGB / gaming-specific feature

---

## 8. Upgrade Threshold

향후 제품은 단순히 '좋은 헤드폰'이 아니라 다음을 만족해야 의미 있는 교체 후보가 된다.

- 핵심 음질 항목 여러 개에서 **UP2(확실한 개선) 이상**이 기대되거나,
- 한두 핵심 항목에서 **UP3(매우 큰 개선)**이 있으면서 다른 핵심 항목이 크게 악화되지 않고,
- 착용감이 현재 H7 TE 대비 지나치게 나빠지지 않아야 한다.

특히 다음 변화는 높은 가치로 본다.

- 중역/보컬 자연스러움 상승
- 실제 resolution 상승
- bass quantity가 아니라 bass quality 상승
- 더 넓고 자연스러운 soundstage
- 복잡한 음악/영화에서 separation 개선
- 고역의 거친 느낌 감소
- 장시간 착용감 유지 또는 개선

---

## 9. Baseline Confidence

- Current configuration: **HIGH**
- Official hardware specifications: **HIGH**
- AE-5 driving compatibility: **HIGH**
- H7 passive tonal characterization: **MEDIUM**
- Comfort characterization: **MEDIUM-HIGH**
- Long-term material durability: **LOW-MEDIUM**
- Use-case baseline: **MEDIUM**

가장 큰 불확실성은 H7 TE 패시브 측정 자료가 제한적이고, 많은 전문 리뷰가 USB/DSP 또는 혼합 사용 조건을 포함한다는 점이다. 따라서 이후 비교에서는 특정 리뷰의 절대 점수보다 **H7 대비 변화 방향**을 중심으로 판단한다.

---

## 10. Step 0 Gate

- [x] H7 + AE-5 기준 환경이 명확히 정의되었다.
- [x] 비교 항목이 빠짐없이 고정되었다.
- [x] 강점/약점이 근거와 함께 기록되었다.
- [x] 사용자 우선순위가 현재 대화 기준으로 정리되었다.

Step 0은 사용자 검토를 위해 **REVIEW** 상태로 전환한다.
